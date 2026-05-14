<div align="center">

<a href="https://knot.tools">
  <img src="assets/knot-horizontal-light.png#gh-light-mode-only" alt="Knot Tools" width="520">
  <img src="assets/knot-horizontal-dark.png#gh-dark-mode-only" alt="Knot Tools" width="520">
</a>

### Visual workflow automation for Dolibarr — and the ecosystem around it.

*🇬🇧 English · [🇫🇷 Lire en français](profile/README.fr.md)*

[![Status](https://img.shields.io/badge/status-private%20beta-8B5CF6?style=flat-square)](https://knot.tools)
[![Dolibarr](https://img.shields.io/badge/Dolibarr-V20%2B-1F2937?style=flat-square)](https://www.dolibarr.org)
[![PHP](https://img.shields.io/badge/PHP-8.1%2B-777BB4?style=flat-square&logo=php&logoColor=white)](https://www.php.net)
[![Vue](https://img.shields.io/badge/Vue-3-42B883?style=flat-square&logo=vue.js&logoColor=white)](https://vuejs.org)
[![Licence](https://img.shields.io/badge/Knot%20Core-GPL--3.0-EC4899?style=flat-square)](#licence)
[![Brand](https://img.shields.io/badge/Knot%20Tools-™-8B5CF6?style=flat-square)](#trademark)

</div>

---

## What we build

A small family of tools that turn **Dolibarr** into a real automation platform — visual editor, native object support, all self-hosted next to the ERP. **Knot Tools™** covers the product, the brand and the ecosystem around it.

<table>
<tr>
<td width="50%" valign="top">

### 🪢 Knot Core
The visual workflow editor that lives inside Dolibarr. Drag-and-drop canvas, native objects (third-parties, invoices, proposals, projects, stocks…), execution via the Dolibarr cron, multi-entity, granular permissions, audit log. **Open source under GPL-3.0**.

</td>
<td width="50%" valign="top">

### 🧩 Knot Pro Pack
Premium connectors that extend the Core palette: outbound HTTP, SaaS APIs (Stripe, Google Workspace, Shopify, …), AI chat nodes (incl. local **Ollama**), SFTP, Telegram, multi-channel alert fan-out. Plugged into Knot via the public extension manifest.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🚚 Knot Migration
A Dolibarr-to-Dolibarr migration assistant for instances coming from older versions or other ERPs. Schema mapping, dry-run, idempotent transfers, audit. Used internally during onboarding.

</td>
<td width="50%" valign="top">

### 🌐 knot.tools
The product website — beta signup, news, documentation pointers. Sober, no tracker, no cookie. Reach us at **`contact@knot.tools`** *(human reply, not an autoresponder)*.

</td>
</tr>
</table>

---

## Why visual workflows for Dolibarr

<table>
<tr>
<td width="25%" align="center" valign="top">

### 🎨
**Visual editor**

Vue Flow canvas, dark mode, **Cmd+K** palette, undo/redo, keyboard-first.

</td>
<td width="25%" align="center" valign="top">

### 🪢
**Native Dolibarr**

Triggers on V20+ objects: third-parties, invoices, proposals, projects, stocks, contacts…

</td>
<td width="25%" align="center" valign="top">

### 🔒
**100% self-hosted**

Your data stays on your stack. AES-256-GCM credentials, audit log, SSRF-hardened HTTP, no mandatory cloud.

</td>
<td width="25%" align="center" valign="top">

### 🌍
**Multi-entity**

Strict per-entity isolation. Granular Dolibarr permissions enforced everywhere.

</td>
</tr>
</table>

---

## Status

🚀 &nbsp; **Knot is in private beta.** Source code lives in private repositories during the beta. **Knot Core** is destined for public release under **GPL-3.0** once the licence-chain backbone is sealed (planned ahead of the public Pro Pack launch). Public release notes and tester onboarding are published on **[knot.tools](https://knot.tools)**.

🔬 &nbsp; **Tested across the matrix.** Continuous integration runs against **Dolibarr 20 / 21 / 22**, **PHP 8.1 / 8.2 / 8.3**, with PHPUnit, Vitest, PHP_CodeSniffer (PSR-12), `composer audit`, `npm audit` and weekly Gitleaks secret scans.

📜 &nbsp; **Knot Tools™** is a trademark in filing. Use of the mark requires written permission of the rights holder; please write to `contact@knot.tools`.

---

## Find us

| | |
|---|---|
| 🌐 &nbsp; Product website & beta signup | **<https://knot.tools>** |
| 📬 &nbsp; General contact | `contact@knot.tools` |
| 🔐 &nbsp; Vulnerability disclosure | `security@knot.tools` · [security policy](../SECURITY.md) · [`security.txt`](https://knot.tools/.well-known/security.txt) |
| 🤝 &nbsp; Code of conduct | [Contributor Covenant 2.1](../CODE_OF_CONDUCT.md) |
| 🛟 &nbsp; Support | [SUPPORT.md](../SUPPORT.md) |
| ✍️ &nbsp; Contributing | [CONTRIBUTING.md](../CONTRIBUTING.md) |

---

## Trademark

**Knot Tools™** is a trademark in filing. You may refer to the project in editorial, technical or comparative contexts. You may not use the mark in a way that suggests endorsement, partnership, or origination by Knot Tools without written permission. The Knot logo and brand assets are reproduced from the official brand pack distributed with **Knot Core**.

## Licence

**Knot Core** is published under **GPL-3.0-or-later**. Other components of the **Knot Tools** ecosystem may be distributed under different terms — consult the corresponding repository when published.

---

<div align="center">

*Knot Tools™ — visual workflow automation for Dolibarr.*<br>
*Made with care, hosted nowhere by default.*

</div>
