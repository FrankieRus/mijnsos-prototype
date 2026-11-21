# mijnSOS.nl Prototypes — Werkafspraken voor Antigravity

Deze repository bevat de drie interactieve mobiele/desktop HTML-prototypes voor **mijnSOS.nl**, gehost op **GitHub Pages**.

## Bestanden & Live URLs
- **`index.html`** — **Prototype A** (Product-first homepage + keuzehulp + vervolgschermen)  
  Live: https://frankierus.github.io/mijnsos-prototype/
- **`prototype2.html`** — **Prototype B** (Warme / begeleide homepage-variant)  
  Live: https://frankierus.github.io/mijnsos-prototype/prototype2.html
- **`prototype3.html`** — **Prototype C** (Referentiekopie van de huidige homepage met CRO-verbeteringen)  
  Live: https://frankierus.github.io/mijnsos-prototype/prototype3.html

Alle HTML-bestanden zijn 100% standalone (alle afbeeldingen zijn als base64 ingebakken).

## Samenwerken via GitHub (belangrijk!)
Meerdere mensen kunnen deze repository onderhouden. Volg daarom altijd deze twee regels:
1. **Altijd eerst synchroniseren:** Voer altijd eerst `git pull` uit voordat u bestanden aanpast, zodat wijzigingen van anderen niet verloren gaan.
2. **Publiceren naar GitHub Pages:** Wanneer de gebruiker vraagt om te *publiceren*, *deployen* of *live te zetten*, voer dan uit:
   ```powershell
   git add .
   git commit -m "Korte beschrijving van de aanpassing"
   git push
   ```
   GitHub Pages zet wijzigingen op `main` binnen ~20–30 seconden automatisch live (gebruik **geen** Netlify).

## Lokaal testen zonder te wachten
Voor snelle preview tijdens het aanpassen:
```powershell
python -m http.server 8080 --bind 127.0.0.1
```
Open daarna `http://localhost:8080/prototype3.html` (of `index.html` / `prototype2.html`). Elke aanpassing is direct zichtbaar na `F5`.

## Ingebouwde modules (altijd intact laten)
- **`<!-- REVIEWS IFRAME OVERLAY ... -->`:** De klikbare review-overlay met de 20 meest recente echte KiyOh-reviews + live KiyOh-tab.
- **`<!-- ELEMENT PICKER / ANNOTATE MODULE -->`:** De knoppen `🎯 Selecteer element` en `📋 Lijst (N)` waarmee de gebruiker elementen kan aanklikken en als prompt in de chat kan plakken.

## Stijl & doelgroep
- Antwoord in helder, beknopt Nederlands.
- De website-teksten op mijnSOS.nl gebruiken de beleefde **`u`-vorm** en zijn gericht op **ouderen (65+) en mantelzorgers**: houd knoppen ruim, teksten duidelijk leesbaar en de mobiele weergave (`375px`) rustig en zonder afkapping.
