# Codice sconto Redcare, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Redcare** da [shopilo.it](https://shopilo.it/negozi/redcare.it). Restituisce **coupon Redcare** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-redcare](https://shopilo-it.github.io/codice-sconto-redcare/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-redcare
cd codice-sconto-redcare
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Redcare",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su farmacia online",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/redcare.it"
  }
]
```

## Coupon Redcare disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su farmacia online | [shopilo.it](https://shopilo.it/negozi/redcare.it) |

Codici attivi: **[shopilo.it/negozi/redcare.it](https://shopilo.it/negozi/redcare.it)**

## Domande frequenti

### Come utilizzo un codice sconto Redcare?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/redcare.it), aggiungi i prodotti al carrello su Redcare e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Redcare?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Redcare piu recenti?
La pagina [shopilo.it/negozi/redcare.it](https://shopilo.it/negozi/redcare.it) viene aggiornata quotidianamente con i codici sconto Redcare, voucher Redcare e coupon promozionali Redcare piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Redcare

Redcare e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/redcare.it) trovi i migliori codici sconto Redcare, coupon Redcare verificati e voucher Redcare attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-redcare
```

```javascript
const { fetchCoupons } = require('codice-sconto-redcare');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
