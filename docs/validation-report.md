# Validation Report

## Date

2026-07-21

## Scope

The Devpost candidate was validated through the actual WindWalker builder UI path, not by hand-coded demo files.

## Main Devpost Scenario

Builder URL: https://ww2.d-tok.com/prototype?builder=1

Generated live URL: https://0a91cf12.windwalker-phase2-user-apps.pages.dev

Builder generation and deployment: `test/results/1116-phase2-live-ui-recording-2026-07-21-r5/`

Deployed mobile flow: `test/results/1117-phase2-live-deployed-flow-2026-07-21-r1/`

Validated:

- builder page opens
- natural-language bookstore prompt is entered into the visible builder input
- visible send button is clicked
- generated app appears in the mobile preview tab
- visible deploy button is clicked
- Cloudflare Pages deployment response is captured
- generated deployment URL opens
- deployed app shows the generated storefront
- mock login closes its dialog and changes the header to the buyer account
- catalog navigation, cart, and test checkout modal are exercised

Screenshots:

- `media/screenshots/01-builder-ready.png`
- `media/screenshots/02-prompt-entered.png`
- `media/screenshots/03-generated-preview.png`
- `media/screenshots/04-deployed-home.png`
- `media/screenshots/05-deployed-login-modal.png`
- `media/screenshots/06-deployed-signed-in.png`
- `media/screenshots/07-deployed-test-checkout.png`

Video:

- `media/videos/windwalker-devpost-live-flow-captioned.mp4`

## Result

The actual builder UI generation, deployment response, and deployed app interaction flow passed. The login and checkout flows are explicitly mock/test flows; no production credentials or real payment are required. Production orchestration, service-role code, and private registry data are not included in this repository.
