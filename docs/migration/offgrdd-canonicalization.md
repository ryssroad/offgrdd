# off.gridd Canonical Repository Migration

This repository is the canonical public control-plane artifact repo for the current off.gridd genesis mesh.

Earlier bootstrap work was staged in `ryssroad/tempo-agent-network` because it already existed as an authenticated GitHub transport. The public protocol artifacts were then copied here and canonicalized to `ryssroad/offgrdd` / `main`.

Private/local-only state was intentionally not copied:

- `.env`
- `.offgridd/private/`
- wallet private keys
- SMTP/API tokens
- Claude auth state
- generated dependency directories such as `node_modules/`

The active mesh state remains:

```text
Operator -> Hermes
Hermes --github--> Claude
Claude --github--> Hermes
```

Blue Scout / Голубой Лазутчик is the first committed agent class.
