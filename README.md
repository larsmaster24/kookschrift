# Kookschrift

Een Nederlandse receptenapp in één zelfstandig HTML-bestand: recepten met fotobanners,
een boodschappenlijst die zichzelf per winkelgang indeelt, en een handsfree **kookmodus**
met timers per stap.

## Gebruiken

Open [`index.html`](index.html) in een browser. Geen build, geen server, geen dependencies
(alleen Google Fonts). Alles wordt lokaal in de browser bewaard (`localStorage`).

Of host het via GitHub Pages en open de gepubliceerde URL op je telefoon.

## Functies

- **Recepten** — lijst met fotobanner per gerecht, zoeken op naam of ingrediënt,
  filterchips per categorie, favorieten.
- **Porties 1–20** — hoeveelheden schalen mee.
- **Kookmodus** — stap voor stap op volledig scherm, voortgangsbalk, en timers die
  automatisch uit de staptekst worden gehaald ("laat 20 minuten pruttelen" → knop
  *Timer 20:00*). Timers lopen door terwijl je verder gaat; scherm blijft aan waar
  de browser dat toestaat.
- **Boodschappenlijst** — tik ingrediënten aan in een recept; ze komen automatisch in
  de juiste winkelgang (Groente & fruit, Vlees & vis, Zuivel & koeling, Voorraadkast,
  Bakkerij). Afvinken, los toevoegen, afgevinkte wissen.
- **Recept toevoegen/bewerken** — met een ingrediënt-parser (hoeveelheid + eenheid
  vooraan) en een fotokiezer per recept.

## Recepten aanpassen

De ingebouwde recepten staan als `SEED`-array in `index.html`. Recepten die je in de
app zelf bewerkt of toevoegt, krijgen een `userEdited`-vlag en blijven bij updates
staan; onbewerkte ingebouwde recepten volgen de laatste versie in de code.

## Thema

Licht en donker, volgt het systeemthema. Warm "kookschrift"-palet: haverkleurig papier,
aubergine-inkt, saffraan accent, olijfgroen voor de winkelgangen. Koppen in Newsreader,
UI-tekst in Karla.
