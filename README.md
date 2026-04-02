# Cod reducere Lensa — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Lensa** de pe [shopilo.ro](https://shopilo.ro/magazin/lensa.ro). Returneaza **cupoane Lensa** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-lensa](https://shopilo-ro.github.io/cod-reducere-lensa/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-lensa
cd cod-reducere-lensa
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Lensa",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la lentile de contact",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/lensa.ro"
  }
]
```

## Cupoane Lensa disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la lentile de contact | [shopilo.ro](https://shopilo.ro/magazin/lensa.ro) |

Codurile active: **[shopilo.ro/magazin/lensa.ro](https://shopilo.ro/magazin/lensa.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Lensa?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/lensa.ro), adauga produsele in cos pe Lensa, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Lensa?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Lensa?
Pagina [shopilo.ro/magazin/lensa.ro](https://shopilo.ro/magazin/lensa.ro) este actualizata zilnic cu cele mai noi cod reducere Lensa, voucher Lensa si cupon promotional Lensa.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Lensa

Lensa este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/lensa.ro) cele mai bune cod reducere Lensa, cupoane Lensa verificate si voucher Lensa active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-lensa
```

```javascript
const { fetchCoupons } = require('cod-reducere-lensa');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
