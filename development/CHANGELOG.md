# PM Shops — development changelog

## Initial documentation

- Added PowerMoves RP development notes and baseline compatibility rules.
- Recorded roadmap and planned integration boundaries.
- No gameplay code, resource names, events, callbacks, exports, or configuration values changed.

Future entries should record meaningful behavior changes, their compatibility impact, and any required deployment steps.

## November 2026

Added delivery-stop lookup and restocking server exports for the matching Jetsam fork, plus a shop-list event. The new restocking export does not issue the original shop-delivery cash reward. Existing independent delivery paths remain. Not yet live-tested.
