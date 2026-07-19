# Validation Report

## Date

2026-07-19

## Scope

The Devpost candidate was validated through the actual WindWalker builder UI path, not by hand-coded demo files.

## Main Devpost Scenario

Builder URL: https://ww2.d-tok.com/prototype?builder=1

Generated live URL: https://bc955fd2.windwalker-phase2-user-apps.pages.dev

Preview gate: `test/results/1114-ui-bookstore-preview-only-2026-07-19-r21-mobile/`

Full UI deploy smoke: `test/results/1114-ui-bookstore-generate-deploy-smoke-2026-07-19-r21-mobile3/`

Deployed mobile flow: `test/results/1114-ui-bookstore-deployed-flow-2026-07-19-r21-mobile/`

Validated:

- builder page opens
- natural-language bookstore prompt is entered into the visible builder input
- visible send button is clicked
- generated app appears in the mobile preview tab
- visible deploy button is clicked
- Cloudflare Pages deployment response is captured
- generated deployment URL opens
- deployed app shows the same generated React storefront
- deployed app shows member login UI and test login state transition
- cart and mock checkout flow are exercised
- Workspace form accepts a test buyer record
- Dashboard displays the saved order record after mock payment

Screenshots:

- `media/screenshots/01-builder-ready.png`
- `media/screenshots/02-prompt-entered.png`
- `media/screenshots/03-generated-preview.png`
- `media/screenshots/04-deployed-home.png`
- `media/screenshots/05-deployed-login-modal.png`
- `media/screenshots/06-deployed-catalog.png`
- `media/screenshots/07-deployed-checkout-modal.png`
- `media/screenshots/08-deployed-dashboard.png`

Video:

- `media/videos/windwalker-devpost-demo-mobile-final.mp4`

## Result

The mobile UI-path preview gate, deployment smoke, and deployed app interaction flow passed. Minor 404 resource warnings in the full smoke are non-blocking static asset requests; the deployed app interaction flow completed without runtime errors. Production credentials and backend service-role code are not included in this repository.
