# Codice sconto Farmacosmo, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Farmacosmo** da [shopilo.it](https://shopilo.it/negozi/farmacosmo.it). Restituisce **coupon Farmacosmo** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-farmacosmo](https://shopilo-it.github.io/codice-sconto-farmacosmo/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-farmacosmo
cd codice-sconto-farmacosmo
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Farmacosmo",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su cosmetici e integratori",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/farmacosmo.it"
  }
]
```

## Coupon Farmacosmo disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su cosmetici e integratori | [shopilo.it](https://shopilo.it/negozi/farmacosmo.it) |

Codici attivi: **[shopilo.it/negozi/farmacosmo.it](https://shopilo.it/negozi/farmacosmo.it)**

## Domande frequenti

### Come utilizzo un codice sconto Farmacosmo?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/farmacosmo.it), aggiungi i prodotti al carrello su Farmacosmo e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Farmacosmo?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Farmacosmo piu recenti?
La pagina [shopilo.it/negozi/farmacosmo.it](https://shopilo.it/negozi/farmacosmo.it) viene aggiornata quotidianamente con i codici sconto Farmacosmo, voucher Farmacosmo e coupon promozionali Farmacosmo piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Farmacosmo

Farmacosmo e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/farmacosmo.it) trovi i migliori codici sconto Farmacosmo, coupon Farmacosmo verificati e voucher Farmacosmo attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-farmacosmo
```

```javascript
const { fetchCoupons } = require('codice-sconto-farmacosmo');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
