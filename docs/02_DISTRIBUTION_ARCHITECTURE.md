# Kaervax OS — Distribution Architecture

## Channel model

Every channel is represented as a controlled configuration:

- channel_id
- channel_type
- platform
- account/owner reference
- status
- catalog scope
- pricing rules
- fulfillment model
- content requirements
- tracking method
- operational owner
- activation date
- deactivation conditions

## Initial channel families

1. Owned: website, Instagram, WhatsApp and other owned surfaces.
2. Marketplace: Shopee, TikTok Shop and other supported marketplaces.
3. Partner: sellers, resellers, distributors.
4. Creator: creator/affiliate distribution.
5. B2B: direct institutional/commercial accounts.

## Channel lifecycle

```
Candidate → Validating → Active → Optimizing → Scaling
                         ↓
                      Paused
                         ↓
                     Retired
```

## Expansion rule

Do not activate a channel merely because it exists. A channel must have:

- product readiness
- account/access readiness
- listing/content readiness
- fulfillment path
- support path
- measurement method
- explicit owner

## Channel independence

Channel-specific logic belongs in adapters/configuration/playbooks, not in the core product domain.
