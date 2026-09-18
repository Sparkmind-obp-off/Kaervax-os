# Kaervax OS — Marketplace Operations

## Supported initial marketplaces

The architecture should support marketplace-specific adapters. Initial candidates include:

- Shopee
- TikTok Shop

Availability, features, API access and commercial rules must be verified against current official platform documentation before implementation.

## Listing lifecycle

```
Draft → QA → Published → Monitored → Updated
                    ↓
                  Paused
```

## Listing checklist

- correct SKU
- title
- description
- images/video
- price
- stock state
- shipping/fulfillment configuration
- variants
- policy compliance
- tracking metadata
- customer-support path

## Marketplace operating controls

- never store credentials in repository
- maintain account ownership records outside source code
- record listing changes
- keep product data canonical
- prevent accidental price/stock overwrite
- distinguish platform data from internal data
- handle API limitations explicitly

## Manual-first principle

If a marketplace cannot be integrated reliably, operate it manually using the same canonical catalog and SOPs until evidence justifies an integration.
