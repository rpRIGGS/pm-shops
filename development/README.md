# PM Shops — PowerMoves RP development

This repository is a PowerMoves RP-specific fork of [qbcore-framework/qb-shops](https://github.com/qbcore-framework/qb-shops). The fork exists solely to add server-specific integrations while retaining the upstream QBCore resource's core behavior.

## Compatibility contract

- GitHub repository branding does **not** change the FiveM runtime resource name. Keep the original resource folder and event/export names for drop-in use.
- Preserve upstream configuration, user-facing behavior, dependencies, attribution, and license.
- Add features in a backward-compatible, opt-in manner wherever possible. Standard QBCore operation must not require PowerMoves-only resources.
- PowerMoves RP uses QBCore, qb-target, and a customized drag-and-drop qb-inventory replacement that preserves QBCore compatibility; ox_lib may be used when needed. Do not introduce ox_target or ox_inventory dependencies.
- Validate changes against the installed server versions before declaring compatibility; the fork itself does not guarantee tested drop-in behavior.

## Scope

shop stock limits, stock decrements, restock triggers, shop delivery locations, and Marlowe lobby display inventory.

Documentation in this folder is planning/reference material, not a claim that the integrations are already implemented.

## November 2026 implementation status

Added GetDeliveryStop and RestockFromJetsam server exports, plus SetShopList event for the companion Jetsam trucker fork. The original resource name remains qb-shops. The new restock export avoids an additional shop delivery cash reward. Changes are committed but not yet tested in FiveM. Existing standalone shop delivery and payment events remain and should be reviewed before deployment. Future Marlowe wine and wholesale features are not implemented.
