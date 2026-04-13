# Code promo FlixBus, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo FlixBus** depuis [shopilo.fr](https://shopilo.fr/reductions/flixbus.fr). Renvoie les **coupons FlixBus** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-flixbus](https://shopilo-fr.github.io/code-promo-flixbus/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-flixbus
cd code-promo-flixbus
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "FlixBus",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les trajets en bus",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/flixbus.fr"
  }
]
```

## Coupons FlixBus disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les trajets en bus | [shopilo.fr](https://shopilo.fr/reductions/flixbus.fr) |

Codes actifs : **[shopilo.fr/reductions/flixbus.fr](https://shopilo.fr/reductions/flixbus.fr)**

## Questions frequentes

### Comment utiliser un code promo FlixBus ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/flixbus.fr), ajoutez les produits a votre panier sur FlixBus et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons FlixBus ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction FlixBus les plus recents ?
La page [shopilo.fr/reductions/flixbus.fr](https://shopilo.fr/reductions/flixbus.fr) est mise a jour quotidiennement avec les codes promo FlixBus, bons de reduction FlixBus et coupons promotionnels FlixBus les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de FlixBus

FlixBus est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/flixbus.fr), retrouvez les meilleurs codes promo FlixBus, coupons FlixBus verifies et bons de reduction FlixBus actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-flixbus
```

```javascript
const { fetchCoupons } = require('code-promo-flixbus');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
