# HDTP — Human Delegated Trust Protocol

HDTP lets one person's AI agent communicate with another person's agent, on terms both people set.

It is built from mutual TLS, X.509 certificates and MCP tools, with one addition: a sealed envelope that carries identity and confidentiality across a link whose TLS is terminated before it reaches the recipient.

- **The identity is the person's; the host serves it.** An identity is the fingerprint of a self-signed root certificate held in the person's wallet. A host — their own machine or a provider — holds a leaf certificate the root issued for one address. Contacts pin the root, so a person can move hosts without losing them.
- **Your agent is an MCP server.** Sending a message is calling the other party's `send_message` tool. Everything a contact may do is a tool, visible and callable only as your permission settings for that contact allow.
- **Contacts are vCards; invites are short URLs.** Cards travel over the channels people already use, and adding a contact is always a human approval.
- **No directory, no relay, no log.** Every relationship starts from a card or an invite.

## Where to go

| | |
|---|---|
| The protocol and whitepaper | [hdtp.io](https://hdtp.io) |
| The specification, its test vectors and SEPs | [hdtp-spec](https://github.com/humandelegatedtrustprotocol/hdtp-spec) |
| Documentation | [docs.hdtp.io](https://docs.hdtp.io) |
| The self-hosted node | [hdtp.dev](https://hdtp.dev) |
| Hosted HDTP identities | [batondeck.com](https://batondeck.com) |

Version 1.0.0. HDTP was formerly named PACT.

Security reports: security@hdtp.io
