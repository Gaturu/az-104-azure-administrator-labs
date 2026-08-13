# Security Rules

This is a public-learning repository.

## Never commit

- Passwords
- Client secrets
- API keys
- Access keys
- Private keys
- Connection strings
- SAS tokens
- Tenant secrets
- Subscription credentials
- Personal access tokens

## Before every push

```bash
git status
git diff --cached
```

Search for suspicious strings where appropriate.

## Use placeholders

```text
<YOUR_SUBSCRIPTION_ID>
<YOUR_TENANT_ID>
<YOUR_RESOURCE_GROUP>
<YOUR_STORAGE_ACCOUNT>
<YOUR_CLIENT_ID>
<YOUR_SECRET>
```

If a secret is accidentally committed, assume it is compromised and rotate/revoke it immediately. Removing it from the latest commit does not make the credential safe.
