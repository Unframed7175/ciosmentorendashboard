# ciosmentorendashboard — landingspagina

Pagina live op: **https://unframed7175.github.io/ciosmentorendashboard/**

---

## Pagina bijwerken

### Eerste keer instellen

```bash
git clone https://github.com/Unframed7175/ciosmentorendashboard.git
cd ciosmentorendashboard
```

### Bij elke update

1. Open `index.html` in een teksteditor
2. Pas aan wat je wil wijzigen (zie hieronder welke onderdelen waar staan)
3. Commit en push:

```bash
git add index.html
git commit -m "update: [beschrijving van wijziging]"
git push
```

Na de push is de pagina binnen ~1 minuut bijgewerkt.

---

## Wat staat waar in index.html

| Onderdeel | Zoek naar |
|---|---|
| Versienummer in navigatiebalk | `<span class="nav-version">` |
| Download-links macOS arm64 | `aarch64.dmg` |
| Download-links macOS Intel | `x64.dmg` |
| Download-link Windows | `releases/tag/v2.x.x` |
| Installatie-instructies | `<section id="installatie">` |
| Functielijst (doet wel/niet) | `<section id="functies">` |
| Release notes | `<section id="updates">` |

---

## Nieuwe versie uitbrengen — checklist

- [ ] Versienummer bijwerken in `<span class="nav-version">`
- [ ] Download-links aanpassen naar nieuwe versie (3 plekken: macOS arm64, macOS x64, Windows)
- [ ] Nieuwe entry toevoegen bovenaan `<section id="updates">` (kopieer een bestaand blok)
- [ ] `update-badge` ("Nieuwste") verplaatsen naar de nieuwe entry, verwijderen uit de vorige
- [ ] Commit en push
