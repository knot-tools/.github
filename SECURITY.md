# Security Policy

*🇬🇧 English · [🇫🇷 Politique de sécurité en français](SECURITY.fr.md)*

This policy applies to all repositories of the **knot-tools** organisation.

## Reporting a vulnerability

Please report security issues **privately** — do not open a public GitHub issue, do not post on a forum, do not chat about it on a public channel.

| Channel | Address |
|---|---|
| **Email** | **`security@knot.tools`** |
| Machine-readable contact | [`https://knot.tools/.well-known/security.txt`](https://knot.tools/.well-known/security.txt) (RFC 9116) |
| Preferred languages | English, French |

If you can, please include:

- **Affected component** (e.g. *Knot Core*, version or commit SHA, deployment context)
- **Reproduction steps**, ideally with a minimal proof of concept
- **Impact assessment** (data exposure, privilege escalation, denial of service, integrity loss…)
- **Suggested mitigation** if you have one
- **Logs** — *redact every secret, token and personal datum before sending*

## What you can expect from us

- **Acknowledgement within 72 hours** of business days from a real human (no autoresponder).
- A **triage decision** (confirmed / informational / out of scope) within 7 business days.
- A **fix or mitigation timeline** communicated explicitly. Critical issues get top priority.
- **Public credit** in release notes if you wish, with the wording you prefer; full anonymity if you prefer that.
- **Coordinated disclosure** — we will agree on a disclosure date with you before any public communication. We support **CVE** registration when warranted.

## Scope

| In scope | Out of scope |
|---|---|
| Knot Core (Dolibarr module) source and runtime | Dolibarr core itself (please report to the [Dolibarr security policy](https://github.com/Dolibarr/dolibarr/security)) |
| Knot Pro Pack connectors | Underlying SaaS providers contacted by connectors (Stripe, Google, Telegram, etc.) |
| Knot License backend (`license.knot.tools`) | Third-party hosting platforms (your own server, Plesk, OVH, IONOS…) |
| `knot.tools` website and `.well-known/security.txt` | Generic web vulnerability scanner output without a working PoC |
| Brand assets and trademark misuse | Social engineering against unrelated third parties |

Please **do not** run automated scanners against `knot.tools` or `license.knot.tools`. We will not act on bulk findings without a clear PoC and meaningful impact statement.

## Safe harbour

We will **not** pursue legal action against researchers who:

- Make a good-faith effort to comply with this policy.
- Avoid privacy violations, service disruption, and destruction of data.
- Give us a reasonable time to fix before any public disclosure.
- Limit testing to systems they own or have explicit permission to test.

## Cryptographic disclosure

If you discover an issue that compromises a **signing key** (release manifests, licence chain), we will treat it as **critical** regardless of exploitability. Reach us as fast as possible — we keep contingency plans for key rotation.

## Hall of fame

We are happy to credit researchers who help us. Please tell us how you would like to be credited (real name, alias, link to your profile, or anonymous).

---

*Last reviewed: 2026-05-14.*
