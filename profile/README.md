<div align="center">

<a href="https://knot.tools">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/knot-horizontal-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/knot-horizontal-light.png">
    <img alt="Knot Tools — visual workflow automation for Dolibarr" src="assets/knot-horizontal-dark.png" width="520">
  </picture>
</a>

### Visual workflow automation for Dolibarr — and the ecosystem around it.

*🇬🇧 English · [🇫🇷 Lire en français](README.fr.md)*

> **Knot Core — public beta** — product site: **[knot.tools](https://knot.tools)**. Documentation: **[docs.knot.tools](https://docs.knot.tools/)**. **Pro Pack** and **Migration** — private beta via **[knot.tools/beta](https://knot.tools/beta/)**.

[![Status](https://img.shields.io/badge/status-public%20beta-8B5CF6?style=flat-square)](https://github.com/knot-tools/knot-core)
[![CI](https://github.com/knot-tools/knot-core/actions/workflows/ci.yml/badge.svg)](https://github.com/knot-tools/knot-core/actions/workflows/ci.yml)
[![Knot Core](https://img.shields.io/github/v/release/knot-tools/knot-core?label=Knot%20Core&style=flat-square&color=8B5CF6)](https://github.com/knot-tools/knot-core/releases/latest)
[![Dolibarr](https://img.shields.io/badge/Dolibarr-V20%E2%80%93V24-1F2937?style=flat-square)](https://www.dolibarr.org)
[![PHP](https://img.shields.io/badge/PHP-8.1%2B-777BB4?style=flat-square&logo=php&logoColor=white)](https://www.php.net)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![Vue](https://img.shields.io/badge/Vue-3.5-42B883?style=flat-square&logo=vue.js&logoColor=white)](https://vuejs.org)
[![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)
[![Tailwind](https://img.shields.io/badge/Tailwind-3-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![Tests](https://img.shields.io/badge/tests-PHPUnit_·_Vitest_·_Playwright-EC4899?style=flat-square)](#-reliability--quality)
[![Style](https://img.shields.io/badge/style-PSR--12-1F2937?style=flat-square)](https://www.php-fig.org/psr/psr-12/)
[![Licence](https://img.shields.io/badge/Knot%20Core-GPL--3.0-EC4899?style=flat-square)](#-licence)
[![Brand](https://img.shields.io/badge/Knot%20Tools-™-8B5CF6?style=flat-square)](#-trademark)

</div>

---

## 🧰 What we build

A small family of products that turn **Dolibarr** into a real automation platform. **Knot Tools™** is the brand and the umbrella for everything below.

<table>
<tr>
<td width="50%" valign="top">

### 🪢 &nbsp; Knot Core
The visual workflow editor that lives inside Dolibarr. Drag-and-drop canvas, native objects (third-parties, invoices, proposals, projects, stocks, contacts…), execution via the Dolibarr cron, multi-entity, granular permissions, full audit log.

**Open source under GPL-3.0** — source on **[github.com/knot-tools/knot-core](https://github.com/knot-tools/knot-core)**, ZIP at **[knot.tools/downloads](https://knot.tools/downloads/knot-core/latest)**.

</td>
<td width="50%" valign="top">

### 🧩 &nbsp; Knot Pro Pack
Premium connectors that extend the Core palette: outbound HTTP, SaaS APIs (Stripe, Google Workspace, Shopify, …), AI chat nodes including local **Ollama**, SFTP, Telegram, multi-channel alert fan-out.

Plugged in via the public extension manifest, **signed and version-pinned**.

**Commercial extension** — purchase and signed delivery via **[license.knot.tools](https://license.knot.tools)** · overview on **[knot.tools/pro-pack](https://knot.tools/pro-pack/)**.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🚚 &nbsp; Knot Migration
A migration assistant for Dolibarr instances coming from older versions or from other ERPs. Schema mapping, dry-run with diff, idempotent transfers, audit trail.

**Commercial extension** for Dolibarr upgrades — purchase via **[license.knot.tools](https://license.knot.tools)** · overview on **[knot.tools/migration](https://knot.tools/migration/)**.

</td>
<td width="50%" valign="top">

### 🌐 &nbsp; knot.tools
The product website — **Knot Core** download, extension beta signup, documentation links.

Sober, no tracker, no cookie. Reach us at **`contact@knot.tools`** *(human reply, not an autoresponder)*.

</td>
</tr>
</table>

---

## ✨ What sets it apart

<table>
<tr>
<td width="33%" align="center" valign="top">

### 🎨
**Visual editor**

Vue Flow canvas, dark mode, **Cmd+K** palette, undo / redo, keyboard-first UX, multi-tab inspector with live TypeScript validation.

</td>
<td width="33%" align="center" valign="top">

### 🪢
**Native to Dolibarr**

Triggers on Dolibarr **V20–V24** native objects: third-parties, invoices, proposals, projects, stocks, contacts, tickets, agenda, members…

</td>
<td width="33%" align="center" valign="top">

### 🔒
**100% self-hosted**

AES-256-GCM credentials at rest, **SSRF**-hardened HTTP with **DNS-rebinding** mitigation, no mandatory cloud, no telemetry, no phone-home.

</td>
</tr>
<tr>
<td width="33%" align="center" valign="top">

### 🌍
**Multi-entity**

Strict isolation per Dolibarr entity. **Granular permissions** are enforced for every Knot capability, everywhere.

</td>
<td width="33%" align="center" valign="top">

### 🧬
**Resilient by design**

Per-node retry policies, exponential backoff, error routes, idempotency keys, rate-limited webhooks and OAuth, structured execution traces.

</td>
<td width="33%" align="center" valign="top">

### 🌐
**International, day one**

Built-in strings in **FR · EN · ES · IT · PT · DE**. Every user-facing string passes through Dolibarr's translation layer — no hard-coded UI.

</td>
</tr>
</table>

---

## 🔬 Reliability & quality

We treat reliability as a feature, not an afterthought.

<table>
<tr>
<td width="50%" valign="top">

### 🧪 &nbsp; Test suites
**PHPUnit** — 605 tests · 2 013 assertions, with a target coverage of **80 %** on the engine and repository layers.<br>
**Vitest** — frontend unit and component tests on every commit.<br>
**Playwright** — end-to-end editor scenarios on real Dolibarr instances.

</td>
<td width="50%" valign="top">

### 🔁 &nbsp; CI matrix
Backend integration runs against **Dolibarr 20.0–24.0** on **PHP 8.2**, with unit tests on **PHP 8.1 · 8.2 · 8.3**, on every push and pull request, plus a frontend build + Vitest job and a PSR-12 strict style check.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛡️ &nbsp; Hardened by design
Outbound HTTP goes through `Knot\Security\UrlPolicy`: every URL is validated, **private and cloud-metadata IP ranges are blocked**, and the resolved address is pinned through cURL to prevent **DNS-rebinding** attacks.<br>
**Dependency advisories** are continuously monitored (PHP and frontend) so a vulnerable upstream library is caught before it ships.

</td>
<td width="50%" valign="top">

### 🔐 &nbsp; Cryptography & audit
Credentials encrypted at rest with **AES-256-GCM**, never logged, never exported.<br>
Every sensitive action lands in the immutable `llx_knot_audit_log` with full server-side search and CSV export.<br>
Release manifests for the Pro Pack are **Ed25519-signed** and pinned by the Core verifier.

</td>
</tr>
</table>

---

## 📦 Status

🚀 &nbsp; **Knot Core is in public beta under GPL-3.0.** Source, issues, and pull requests: **[github.com/knot-tools/knot-core](https://github.com/knot-tools/knot-core)**. Signed ZIP releases: **[knot.tools/downloads/knot-core/latest](https://knot.tools/downloads/knot-core/latest)**. Documentation: **[docs.knot.tools](https://docs.knot.tools/)**.

🧩 &nbsp; **Pro Pack** and **Migration** are commercial extensions (PolyForm Shield) in **private beta** — access via **[knot.tools/beta](https://knot.tools/beta/)**, purchase via **[license.knot.tools](https://license.knot.tools)**.

📜 &nbsp; **Knot Tools™** is a registered trademark. The product module is referred to simply as **Knot** in technical contexts and **Knot Core** in distribution contexts; the umbrella brand is **Knot Tools**.

---

## 🧭 Find us

| | |
|---|---|
| 🌐 &nbsp; Product website & beta signup | **<https://knot.tools>** |
| 📬 &nbsp; General contact | `contact@knot.tools` |
| 🔐 &nbsp; Vulnerability disclosure | `security@knot.tools` · [security policy](../SECURITY.md) · [`security.txt`](https://knot.tools/.well-known/security.txt) |
| 🤝 &nbsp; Code of conduct | [Contributor Covenant 2.1](../CODE_OF_CONDUCT.md) |
| 🛟 &nbsp; Support | [SUPPORT.md](../SUPPORT.md) |
| ✍️ &nbsp; Contributing | [CONTRIBUTING.md](../CONTRIBUTING.md) |

---

## 🏷️ Trademark

**Knot Tools™** is a trademark filing in progress. You may refer to the project in editorial, technical or comparative contexts. You may not use the mark in a way that suggests endorsement, partnership or origination by Knot Tools without written permission. The Knot logo and brand assets are reproduced from the official brand pack distributed with **Knot Core**.

## 📄 Licence

**Knot Core** is published under **GPL-3.0-or-later**. Other components of the **Knot Tools** ecosystem may be distributed under different terms — consult the corresponding repository when published.

---

<div align="center">

*Knot Tools™ — visual workflow automation for Dolibarr.*<br>
*Made with care, hosted nowhere by default.*

<sub>Made with ❤️ &amp; Grind.</sub>

</div>
