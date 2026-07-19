# Architecture Summary

## Goal

WindWalker targets small-business web apps, not generic pages. The first product scope is bounded: booking, checkout, CRM records, file intake, customer support, and operator dashboards.

## Pipeline

```text
User request
  -> intent normalization
  -> workflow pattern match
  -> app artifact generation
  -> validation
  -> preview
  -> deployment
  -> support and improvement loop
```

## Public MVP Lane

The Devpost demo uses a no-build browser artifact lane for fast evaluation. The generated app is deployable as static HTML/JavaScript while delegating real data/auth/storage/payment integrations to external infrastructure.

This lane is sufficient for hackathon evaluation:

- mock login
- test checkout
- reservation request
- operator dashboard
- download unlock
- deployment URL

## Production Direction

Production can add stronger layers without changing the product thesis:

- Supabase auth and row-level security
- GCS signed URL file delivery
- payment provider approval and webhook verification
- workflow registry expansion
- React/Flowbite React build lane for complex apps
- support dashboard for customer maintenance

## System Boundary

The public repo excludes:

- production system prompts
- private workflow registry
- validation heuristics
- deployment tokens and service keys
- backend service-role code
- customer data

## Core Thesis

AI democratizes software creation. Operations still require trust. WindWalker captures that trust layer for small businesses through workflow patterns, deployment, validation, and lightweight support.

