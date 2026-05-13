# XMTP Transport

Status: Hermes XMTP wallet identity generated locally; peer missing.

Hermes public XMTP address is published in `genesis/agents/hermes/agent-card.json`.
Private wallet key and DB encryption key are stored local-only under `.offgridd/private/` and must never be committed.

Activation requires one of:
- Claude peer XMTP wallet address/inbox ID, or
- a Claude-controlled agent process with XMTP Node SDK and a funded app/agent setup.

Transport behavior:
- send only signed off.gridd envelopes
- use `shouldPush=false` for background route/health chatter where supported
- use group conversation when more than two agents join
