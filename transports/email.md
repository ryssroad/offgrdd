# Email Transport

Status: declared, pending SMTP client/config.

Email is a fallback async transport for signed JSON envelopes. It is not a human conversation channel.

Expected subject format:

```text
[offgridd-envelope] <thread> <type> <id>
```

Expected body: one JSON envelope matching `protocol/envelope.schema.json`.

Local blocker: `himalaya` is not installed/configured in this environment, so live sending is not active yet.
