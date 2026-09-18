# Kaervax OS — Data Model Blueprint

## Core entities

```
Product
SKU
Channel
Listing
Partner
Creator
AffiliateRelationship
Campaign
ContentAsset
OrderReference
OperationalException
MetricSnapshot
Task
AutomationRun
ExpansionProposal
```

## Relationship model

- Product has one or more SKUs.
- SKU can map to multiple channel listings.
- Channel owns/hosts listings.
- Creator/Partner can participate in campaigns.
- Campaign can contain content assets.
- Orders reference channel and SKU where available.
- Exceptions reference orders or operational objects.
- Metrics reference a source and period.
- Expansion proposals reference evidence and target capability.

## Implementation guidance

Use stable internal IDs and external platform IDs as separate fields.

Do not make marketplace IDs the primary identity of Kaervax objects.
