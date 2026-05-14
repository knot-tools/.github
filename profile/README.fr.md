<div align="center">

<a href="https://knot.tools">
  <img src="assets/knot-horizontal-light.png#gh-light-mode-only" alt="Knot Tools" width="520">
  <img src="assets/knot-horizontal-dark.png#gh-dark-mode-only" alt="Knot Tools" width="520">
</a>

### Automatisation visuelle de workflows pour Dolibarr — et l'écosystème autour.

*[🇬🇧 Read in English](README.md) · 🇫🇷 Français*

[![Statut](https://img.shields.io/badge/statut-b%C3%AAta%20priv%C3%A9e-8B5CF6?style=flat-square)](https://knot.tools)
[![Dolibarr](https://img.shields.io/badge/Dolibarr-V20%2B-1F2937?style=flat-square)](https://www.dolibarr.org)
[![PHP](https://img.shields.io/badge/PHP-8.1%2B-777BB4?style=flat-square&logo=php&logoColor=white)](https://www.php.net)
[![Vue](https://img.shields.io/badge/Vue-3-42B883?style=flat-square&logo=vue.js&logoColor=white)](https://vuejs.org)
[![Licence](https://img.shields.io/badge/Knot%20Core-GPL--3.0-EC4899?style=flat-square)](#licence)
[![Marque](https://img.shields.io/badge/Knot%20Tools-™-8B5CF6?style=flat-square)](#marque)

</div>

---

## Ce que nous construisons

Une petite famille d'outils qui transforment **Dolibarr** en véritable plateforme d'automatisation — éditeur visuel, support natif des objets, 100 % self-hosted à côté de l'ERP. **Knot Tools™** désigne le produit, la marque et l'écosystème.

<table>
<tr>
<td width="50%" valign="top">

### 🪢 Knot Core
L'éditeur visuel de workflows à l'intérieur de Dolibarr. Canvas drag-and-drop, objets natifs (tiers, factures, propals, projets, stocks…), exécution via le cron Dolibarr, multi-entité, permissions granulaires, journal d'audit. **Open source sous GPL-3.0.**

</td>
<td width="50%" valign="top">

### 🧩 Knot Pro Pack
Connecteurs premium qui étendent la palette du Core : HTTP sortant, APIs SaaS (Stripe, Google Workspace, Shopify…), nœuds IA (dont **Ollama** local), SFTP, Telegram, fan-out d'alertes multi-canal. Branchés à Knot via le manifest d'extension public.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🚚 Knot Migration
Assistant de migration Dolibarr-vers-Dolibarr pour les instances issues d'anciennes versions ou d'autres ERP. Mapping de schéma, dry-run, transferts idempotents, audit. Utilisé en interne pour l'onboarding.

</td>
<td width="50%" valign="top">

### 🌐 knot.tools
Le site produit — inscription bêta, actualités, pointeurs vers la documentation. Sobre, sans tracker, sans cookie. Contact : **`contact@knot.tools`** *(réponse humaine, pas d'autorépondeur)*.

</td>
</tr>
</table>

---

## Pourquoi des workflows visuels pour Dolibarr

<table>
<tr>
<td width="25%" align="center" valign="top">

### 🎨
**Éditeur visuel**

Canvas Vue Flow, mode sombre, palette **Cmd+K**, undo/redo, raccourcis clavier.

</td>
<td width="25%" align="center" valign="top">

### 🪢
**Natif Dolibarr**

Triggers sur les objets V20+ : tiers, factures, propals, projets, stocks, contacts…

</td>
<td width="25%" align="center" valign="top">

### 🔒
**100 % self-hosted**

Vos données restent chez vous. Credentials AES-256-GCM, audit log, HTTP durci anti-SSRF, aucun cloud obligatoire.

</td>
<td width="25%" align="center" valign="top">

### 🌍
**Multi-entité**

Isolation stricte par entité. Permissions Dolibarr granulaires partout.

</td>
</tr>
</table>

---

## Statut

🚀 &nbsp; **Knot est en bêta privée.** Le code source vit dans des dépôts privés pendant la bêta. **Knot Core** est destiné à une publication open source sous **GPL-3.0** une fois la chaîne de licence scellée (prévu avant le lancement public du Pro Pack). Les notes de version publiques et l'onboarding des testeurs sont publiés sur **[knot.tools](https://knot.tools)**.

🔬 &nbsp; **Testé sur toute la matrice.** L'intégration continue tourne sur **Dolibarr 20 / 21 / 22**, **PHP 8.1 / 8.2 / 8.3**, avec PHPUnit, Vitest, PHP_CodeSniffer (PSR-12), `composer audit`, `npm audit` et un scan hebdomadaire de secrets via Gitleaks.

📜 &nbsp; **Knot Tools™** est une marque en cours de dépôt. L'usage de la marque nécessite l'autorisation écrite du titulaire ; écrivez à `contact@knot.tools`.

---

## Nous trouver

| | |
|---|---|
| 🌐 &nbsp; Site produit & inscription bêta | **<https://knot.tools>** |
| 📬 &nbsp; Contact général | `contact@knot.tools` |
| 🔐 &nbsp; Signalement de vulnérabilité | `security@knot.tools` · [politique de sécurité](../SECURITY.fr.md) · [`security.txt`](https://knot.tools/.well-known/security.txt) |
| 🤝 &nbsp; Code de conduite | [Contributor Covenant 2.1](../CODE_OF_CONDUCT.fr.md) |
| 🛟 &nbsp; Support | [SUPPORT.fr.md](../SUPPORT.fr.md) |
| ✍️ &nbsp; Contribuer | [CONTRIBUTING.fr.md](../CONTRIBUTING.fr.md) |

---

## Marque

**Knot Tools™** est une marque en cours de dépôt. Vous pouvez référencer le projet dans un cadre éditorial, technique ou comparatif. Vous ne pouvez pas utiliser la marque d'une manière qui suggère une recommandation, un partenariat ou une origine Knot Tools sans autorisation écrite. Le logo Knot et les éléments graphiques proviennent du brand pack officiel distribué avec **Knot Core**.

## Licence

**Knot Core** est publié sous **GPL-3.0-or-later**. Les autres composants de l'écosystème **Knot Tools** peuvent être distribués sous d'autres termes — consultez le dépôt correspondant lors de sa publication.

---

<div align="center">

*Knot Tools™ — automatisation visuelle de workflows pour Dolibarr.*<br>
*Conçu avec soin, hébergé nulle part par défaut.*

</div>
