# Kaervax OS — Product Catalog System

## Purpose

Maintain a canonical product representation that can be transformed for different channels.

## Canonical product

Minimum fields:

- product_id
- SKU(s)
- name
- short description
- full description
- media references
- price
- cost reference
- stock reference
- variants
- status
- channel eligibility
- fulfillment profile

## Source-of-truth rule

The canonical catalog is authoritative for internal product identity. Channel listings are projections/adaptations.

## SKU rules

- stable IDs
- no reuse of retired IDs
- variant relationships explicit
- channel SKU mappings explicit
- inventory ownership explicit

## Change management

A material product change should record:
- what changed
- why
- effective date
- affected channels
- responsible operator
- rollback/reference information

## MVP

Start with a structured file/table or lightweight database. Do not build a complex PIM unless manual synchronization becomes a measurable bottleneck.
