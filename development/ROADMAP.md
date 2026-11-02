# PM Shops — development roadmap

## Baseline

- [ ] Audit the original upstream code and record the exact integration contracts.
- [ ] Preserve the original resource name, public events, callbacks, exports, configuration defaults, and stock behavior.

## Planned PowerMoves enhancements

- [ ] Inventory-limited shops retain original purchase behavior and shop configuration.
- [ ] Inspect actual upstream stock update and delivery paths before adding low-stock notifications.
- [ ] Add opt-in PowerMoves restock-order notifications without replacing stock authority.
- [ ] Support Marlowe wine displays and configured external retail locations through stable integration hooks.
- [ ] Preserve compatibility with qb-truckerjob and standard QBCore when custom resources are absent.

## Release checks

- [ ] Existing standard QBCore flows still work with no PowerMoves-only resources installed.
- [ ] Optional integrations fail safely when a peer resource is absent.
- [ ] Server validates inventory, permissions, stock transfers, and fulfillment rather than trusting client messages.
- [ ] Document deployment instructions and compatibility changes before moving to the development server.

Priorities here are exploratory; do not interrupt ongoing pm-marlowe implementation without an explicit development decision.

## Current implementation status

- [x] Companion Jetsam delivery stop lookup and restocking exports.
- [x] Shop-list delivery event.
- [ ] Test stock persistence and integration on FiveM server.
- [ ] Review legacy standalone delivery payment paths.
- [ ] Future Marlowe wholesale and wine displays remain deferred.
