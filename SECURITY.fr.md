# Politique de sécurité

*[🇬🇧 Read in English](SECURITY.md) · 🇫🇷 Français*

Cette politique s'applique à tous les dépôts de l'organisation **knot-tools**.

## Signaler une vulnérabilité

Merci de signaler les problèmes de sécurité **en privé** — n'ouvrez pas d'issue publique GitHub, ne postez pas sur un forum, n'en parlez pas sur un canal public.

| Canal | Adresse |
|---|---|
| **Email** | **`security@knot.tools`** |
| Contact lisible par machine | [`https://knot.tools/.well-known/security.txt`](https://knot.tools/.well-known/security.txt) (RFC 9116) |
| Langues préférées | Français, anglais |

Si possible, incluez :

- **Composant affecté** (par ex. *Knot Core*, version ou SHA de commit, contexte de déploiement)
- **Étapes de reproduction**, idéalement avec un proof of concept minimal
- **Évaluation d'impact** (exposition de données, élévation de privilèges, déni de service, perte d'intégrité…)
- **Mitigation suggérée** si vous en avez une
- **Logs** — *expurgez tout secret, token et donnée personnelle avant envoi*

## Ce que vous pouvez attendre de nous

- **Accusé de réception sous 72 heures** ouvrées de la part d'un humain (pas d'autorépondeur).
- Une **décision de triage** (confirmé / informationnel / hors scope) sous 7 jours ouvrés.
- Un **calendrier de correction ou de mitigation** communiqué explicitement. Les problèmes critiques sont prioritaires.
- **Crédit public** dans les notes de version si vous le souhaitez, avec la formulation de votre choix ; anonymat complet si vous préférez.
- **Divulgation coordonnée** — nous conviendrons d'une date de divulgation avec vous avant toute communication publique. Nous soutenons l'enregistrement **CVE** lorsque pertinent.

## Périmètre

| Dans le périmètre | Hors périmètre |
|---|---|
| Knot Core (module Dolibarr), source et runtime | Dolibarr lui-même (voir la [politique de sécurité Dolibarr](https://github.com/Dolibarr/dolibarr/security)) |
| Connecteurs Knot Pro Pack | Fournisseurs SaaS contactés par les connecteurs (Stripe, Google, Telegram, etc.) |
| Backend Knot License (`license.knot.tools`) | Plateformes d'hébergement tierces (votre serveur, Plesk, OVH, IONOS…) |
| Site `knot.tools` et `.well-known/security.txt` | Sortie brute de scanner web sans PoC ni impact démontré |
| Éléments de marque et utilisation de la marque | Ingénierie sociale contre des tiers non liés |

Merci de **ne pas** lancer de scanner automatisé contre `knot.tools` ni `license.knot.tools`. Nous ne traiterons pas les résultats massifs sans PoC clair et impact significatif.

## Engagement de bonne foi

Nous **ne poursuivrons pas** légalement les chercheurs qui :

- Font un effort de bonne foi pour respecter cette politique.
- Évitent toute atteinte à la vie privée, interruption de service ou destruction de données.
- Nous laissent un délai raisonnable pour corriger avant toute divulgation publique.
- Limitent leurs tests à des systèmes leur appartenant ou pour lesquels ils ont l'autorisation explicite.

## Divulgation cryptographique

Si vous découvrez un problème compromettant une **clé de signature** (manifestes de release, chaîne de licence), nous le traiterons comme **critique** indépendamment de l'exploitabilité. Contactez-nous dans les plus brefs délais — nous maintenons des plans de contingence pour la rotation des clés.

## Hall of fame

Nous serons heureux de créditer les chercheurs qui nous aident. Indiquez-nous votre préférence (vrai nom, pseudonyme, lien profil, ou anonyme).

---

*Dernière révision : 14 mai 2026.*
