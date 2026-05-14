# Contribuer à Knot Tools

*[🇬🇧 Read in English](CONTRIBUTING.md) · 🇫🇷 Français*

> Merci d'envisager une contribution. **Knot Tools est en bêta privée** : le code source n'est pas encore public, donc la surface de contribution est actuellement limitée. Ce document décrit ce qui est possible **aujourd'hui** et ce qui le deviendra à la sortie publique de **Knot Core**.

## Aujourd'hui (bêta privée)

### Ce que nous accueillons

- 🐞 **Rapports de bugs** avec étapes de reproduction, détails d'environnement et logs expurgés → email **`contact@knot.tools`**.
- 💡 **Suggestions de fonctionnalités et cas d'usage** → email **`contact@knot.tools`**.
- 🔐 **Signalements de sécurité** → email **`security@knot.tools`** en suivant la [politique de sécurité](SECURITY.fr.md). **Jamais** dans une issue publique.
- 📚 **Retours sur la documentation** si vous êtes bêta-testeur·euse avec accès au dépôt privé → restez sur le canal privé pour le moment, nous reflèterons les corrections sur la documentation publique au fur et à mesure de son ouverture.

### Ce que nous ne pouvons pas encore accepter

- 🚫 **Pull requests externes contre des dépôts privés.** GitHub ne permet pas aux non-membres d'ouvrir des PR contre un dépôt privé. Les contributions deviendront possibles dès que **Knot Core** sera publié sous GPL-3.0.
- 🚫 **Résultats massifs de scanners automatisés** sans proof of concept ni évaluation d'impact.

## Demain (après la sortie publique de Knot Core)

Quand **Knot Core** sera publié publiquement, nous accepterons des pull requests selon les conditions suivantes.

### Style et conventions

- **Backend** : PHP 8.1+, namespace `Knot\`, **PSR-12** strict (ruleset projet dans `phpcs.xml.dist`), `declare(strict_types=1)` partout, type hints, pas de SQL inline en dehors de la couche repository.
- **Frontend** : Vue 3, TypeScript strict, Tailwind avec préfixe `k-`, Vite 8.
- **Tests** : PHPUnit pour le backend (≥ 80 % de couverture sur le moteur), Vitest pour le frontend, Playwright pour l'end-to-end. Tout nouveau code livre ses nouveaux tests.
- **Commits** : **Conventional Commits** (`feat:`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`, `perf:`, `style:`, `build:`, `ci:`). Sujet à l'impératif présent, ≤ 72 caractères, pas de point final.
- **Documentation** : tout changement fonctionnel met à jour `CHANGELOG.md` et tout guide pertinent sous `docs/`.
- **Licences** : toute nouvelle dépendance doit être MIT, Apache-2.0, BSD, ISC, LGPL ou CC0. **Aucun code n8n ni dérivé**, aucun fair-code, aucune SUL, aucune Commons Clause, aucune BSL.

### Intégration continue

Avant de pousser, nous recommandons de lancer en local :

```bash
vendor/bin/phpcs --standard=phpcs.xml.dist class/
vendor/bin/phpcbf --standard=phpcs.xml.dist class/    # auto-fix les choses faciles
vendor/bin/phpunit --no-coverage
cd frontend && npm run build && npm test
```

La matrice CI tourne sur **PHP 8.1 / 8.2 / 8.3** et **Dolibarr 20 / 21 / 22**. Tout échec sur `phpcs`, `phpunit`, `composer audit`, `npm audit` ou Gitleaks bloque le merge.

### Revue de code

- Un·e mainteneur·euse relit chaque PR. Nous visons une première réponse sous 5 jours ouvrés.
- Les discussions restent techniques et respectueuses — voir le [Code de conduite](CODE_OF_CONDUCT.fr.md).
- Nous pouvons demander des modifications, proposer des designs alternatifs ou décliner poliment une PR qui ne s'aligne pas avec la roadmap. Les PR déclinées sont toujours accompagnées d'une raison claire.

### Paternité et licence

En soumettant une contribution à un dépôt Knot Tools, vous acceptez que votre contribution soit publiée sous les termes du dépôt en question. Pour **Knot Core**, il s'agit de **GPL-3.0-or-later**.

### Par où commencer

- La **roadmap** (`docs/roadmap.md` dans le dépôt Knot Core) liste les prochains jalons et les good-first-issues connus.
- La documentation **d'architecture** (`docs/architecture.md`) décrit le moteur, la couche repository et les connecteurs.
- Le **guide d'authoring de connecteurs** (`docs/connector-authoring-guide.md`) vous guide pas à pas dans la création d'un nouveau connecteur.

---

*Dernière révision : 14 mai 2026.*
