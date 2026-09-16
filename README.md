# Polymarket Overlap — Smart Money Tracker

Analyseur d'overlap de wallets Polymarket : colle des adresses 0x (ou charge le top des traders), l'outil croise leurs positions **en direct** et classe les marchés par meilleure entrée, avec verdict ACHETER / SUIVRE / ÉVITER, proba estimée vs marché, et simulateur de mise.

**Live : https://sacha9214.github.io/polymarket-overlap/**

![Opportunités détectées sur le top 10 de la semaine](docs/apercu.png)

## Fonctionnalités

- **Presets** : top 50 de la semaine ou top 50 all-time, chargés depuis le leaderboard Polymarket
- **Overlap** : un marché ressort quand au moins deux wallets détiennent la même issue
- **Proba estimée** : part du prix du marché et l'ajuste de ±12 points au plus selon le palmarès réel des wallets (trades clos reconstruits), leur conviction et leur prix d'entrée
- **Verdict par marché** : ACHETER, SUIVRE ou ÉVITER, avec une phrase d'explication et le détail par wallet
- **Filtres et tris** : meilleure entrée, gain potentiel, proba de gagner, échéance, wallets gagnants seulement
- **Simulateur de mise**, rafraîchissement automatique toutes les 60 s, dernière recherche restaurée

Un seul fichier HTML, zéro dépendance. Données via `data-api.polymarket.com` et `gamma-api.polymarket.com`. Pas un conseil financier.

## Licence

[MIT](LICENSE)
