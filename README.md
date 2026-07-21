# WindWalker

WindWalker is a GPT-powered web app builder for small businesses. It turns natural-language requests into working business web apps such as booking systems, digital storefronts, checkout flows, customer records, and operator dashboards.

The public repository is a sanitized OpenAI Devpost showcase package. It does not include the production prompt orchestration, validation heuristics, deployment infrastructure, private registry data, credentials, or service-role keys.

## Try It Out

| Demo | URL | Scope |
|---|---|---|
| WindWalker Builder | https://ww2.d-tok.com/prototype?builder=1 | Natural-language app generation, preview, and deployment |
| Generated Digital Content Bookstore | https://0a91cf12.windwalker-phase2-user-apps.pages.dev | Generated and deployed through the WindWalker builder UI; storefront, mock login, cart, and test checkout |

## Elevator Pitch

GPT can generate an app. WindWalker helps a non-technical small-business owner launch, fix, operate, and continuously improve that app with lightweight human support.

## What It Shows

- Natural-language business app generation
- React-style high-density UI patterns
- AI chat plus mobile live preview
- Mock authentication and test payment flows
- Booking, checkout, file intake, CRM-style records, and dashboards
- Registry-driven workflow patterns for repeatable small-business use cases
- Human-in-the-loop support as the operational layer after generation

## Why This Matters

Website generation is becoming common. The bottleneck moves to operation: payment issues, booking changes, customer data, maintenance, and confidence. WindWalker focuses on that last mile for small businesses.

The production system is designed as a small-business execution layer:

```text
Natural language -> workflow match -> app artifact -> validation -> deployment -> support loop
```

## Built With

- GPT-5.6 for the final Devpost submission iteration and validation notes
- OpenAI Codex for implementation, repository packaging, validation artifacts, and submission documentation
- React-style browser app artifacts
- Supabase-ready auth/data model
- GCS-ready file storage model
- Cloudflare Pages deployment path
- JavaScript, HTML, CSS

## Public Package Contents

```text
docs/       Devpost story, architecture, security/disclosure notes
demos/      Sanitized demo artifact and demo links
media/      3:2 screenshots and MP4 demo clips
examples/   Demo prompts and test accounts
```

Main demo video:

```text
media/videos/windwalker-devpost-live-flow-captioned.mp4
```

## Devpost Build Record

The final submission pass was completed with GPT-5.6 and OpenAI Codex. The submitted Codex `/feedback` session ID corresponds to that final GPT-5.6 work session. The repository intentionally contains only the public evaluation package: runnable sanitized demos, validation evidence, architecture notes, prompts, and media.

## Disclosure

The full production implementation is not open-sourced. It contains proprietary prompt orchestration, workflow registry data, validation logic, deployment automation, and operational support tooling. Public demos and a sanitized showcase repository are provided for evaluation.
