# Kaervax OS — Security & Access Contract

## Rules

1. No API keys, passwords, session cookies, access tokens or private credentials in Git.
2. Secrets belong in the appropriate secret manager/platform configuration.
3. Least privilege by default.
4. Separate development, staging and production credentials.
5. Never ask an agent to print secrets into logs.
6. External account ownership must remain with the business owner.
7. Record integrations as references, not credential values.
8. Destructive operations require explicit safeguards.
9. Audit important changes.
10. Remove access when a partner/operator relationship ends.

## Data classification

### Public
Product facts intended for public distribution.

### Internal
Operational plans, non-public metrics, SOPs.

### Restricted
Customer information, partner commercial terms, financial records.

### Secret
Credentials, tokens, private keys.

Restricted and Secret data must not be committed to this repository.
