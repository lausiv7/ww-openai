# Privacy and Security Notes

## Public Repository Policy

This repository is a sanitized showcase package. It intentionally excludes production credentials and proprietary implementation details.

## Not Included

- API keys
- `.env` files
- Supabase service-role keys
- Cloudflare deployment tokens
- GCS credentials
- production prompt orchestration
- private validation logic
- internal workflow registry data
- customer data

## Demo Data

The public demos use mock accounts and test flows. Payment screens are test checkout demonstrations and do not process real payments.

## Production Model

Production deployments should use:

- provider-side authentication
- least-privilege API keys
- row-level security for tenant data
- signed file URLs for private downloads
- payment webhooks for settlement verification
- support logs without exposing private customer content

