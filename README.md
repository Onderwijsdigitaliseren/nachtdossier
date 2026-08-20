# Het Nachtdossier

Een schil rond losse interactieve moordmysteries. Elke zaak is een op zichzelf staand HTML-bestand; `index.html` is alleen de recherchekamer die ernaar linkt.

## Zaken
**Lade I · Murdoku's** (plattegrond-dossiers)
- `nachtportier.html` — De Nachtportier (vijf zaken, 1949–1954)
- `grondplan.html` — Het Grondplan (reeks, 1957–1961)

**Lade II · Moordzaken** (verhaalgedreven)
- `MERIDIAAN___Nachtdossier44-C.html` — Villa Meridiaan
- `nachtfrequentie.html` — Nachtfrequentie (92.4 FM)
- `nachttrein212.html` — Nachttrein 212 (Amsterdam · Wenen)

**Lade III · Puzzelkamers** (puzzelgedreven)
- `schakelkamer.html` — De Schakelkamer (Dossier P1, 1963)
- `ravenhorst.html` — Ravenhorst (landhuis)
- `de-lichttafel.html` — De Lichttafel (sterrenwacht, 1957)

**Lade IV · Kruisroosters** (rasterdossiers)
- `de-zwarte-kolom.html` — De Zwarte Kolom (drie nachten, november 1958)

## Online zetten (GitHub Pages)
1. Zet alle bestanden in de root van je repo.
2. Repo → **Settings → Pages** → Source: `Deploy from a branch`, branch `main`, map `/root`.
3. Na een minuut staat de schil op `https://<gebruiker>.github.io/<repo>/`.

## Nieuwe zaak toevoegen
Open `index.html`, zoek de `ZAKEN`-array bovenin de `<script>` en voeg één object toe:

```js
{ type: "verhaal", nummer: "Zaak 03", titel: "...", omschrijving: "...", bestand: "jouwbestand.html", stempel: "Onopgelost" }
```

`type` bepaalt de lade: `"murdoku"` (Lade I), `"verhaal"` (Lade II), `"puzzel"` (Lade III) of `"kruisrooster"` (Lade IV). De volgorde van de laden staat in de `KASTEN`-array.

Zet het bijbehorende `.html`-bestand ernaast. Klaar.

## Koffiekas (donaties)
De koffiekas onderaan de pagina wijst naar `https://ko-fi.com/kellievdk`.
Wil je ooit een andere link (bijv. een Stripe Payment Link)? Open `index.html`, zoek `KOFFIE_LINK` bovenin de script-sectie en vervang de URL. Leeg laten = koffiekas onzichtbaar.
