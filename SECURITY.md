# Security Policy

## Supported version

Only the default branch is maintained.

## Reporting a vulnerability

Do not open a public issue containing credentials, personal information, or
production data. Use GitHub's private vulnerability reporting feature.

Include:

- the affected path or behavior;
- reproduction steps using synthetic data;
- the potential impact;
- any suggested mitigation.

## Publication policy

All examples must use synthetic identities and records. Production data,
customer material, access tokens, private keys, environment files, and internal
documents are prohibited.

Before publication, run:

```bash
bash scripts/security-check.sh
```
