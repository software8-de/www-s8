# Software8

Site für `software8.de`.

Software8 ist die Dachseite für Organisation as Code: ein gemeinnützig
gedachtes Open-Source-Projekt für wiederkehrende Geschäftsprozesse kleiner
und mittlerer Unternehmen. Branchenspezifische Teilprojekte entstehen dort, wo
sich genug Kunden, Partner und Interessierte für ein Vertical finden.

Das erste Vertical ist Notariat8 für Notariat as Code (`notariat8.de`). Weitere
Verticals können etwa für Kanzleien, Steuerbüros oder Immobilienverwaltungen
folgen.

## Deploybarer Root

Dieses Repository enthält die statischen Dateien für diese Website direkt im
Root. GitHub Pages kann deshalb ohne zusätzlichen Build aus `main` und
`/(root)` veröffentlichen.

## CI- und Styleguide-Quelle

Dieses Repo dient zusätzlich als verbindliche CI-Quelle für Software8 und
abgeleitete Vertical-Seiten.

- [styleguide/tokens.css](styleguide/tokens.css) enthält die grundlegenden
  Design Tokens.
- [styleguide/README.md](styleguide/README.md) beschreibt die verbindliche
  Nutzung für Vertical-Projekte.
- [assets/site.css](assets/site.css) nutzt diese Tokens direkt und dient als
  erste Referenzimplementierung.

## Gemeinsame 8-Brand-Assets

Der kanonische Asset-Katalog für alle bestehenden und künftigen `*8`-Repos
liegt in [bild8/www-b8](https://github.com/bild8/www-b8) und wird über
`https://bild8.de/assets/8/` veröffentlicht.

`www-s8` nutzt daraus das `s8`-Icon direkt als Favicon:
`https://bild8.de/assets/8/svg/s8.svg`. Neue Vertical- oder Produkt-Repos
sollen denselben Katalog referenzieren statt eigene 8er-Logo-Kopien zu
pflegen. Lokale Kopien sind nur für Offline- oder Testflächen vorgesehen und
müssen aus `bild8/www-b8` synchronisiert bleiben.

## GitHub Pages

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/(root)`
- Custom domain: `software8.de`

## Pflege

- Inhalte der deutschen Hauptseite stehen in [index.html](index.html).
- Die englische Orientierung steht in [en/index.html](en/index.html).
- Rechtliche Platzhalter stehen in [impressum.html](impressum.html) und
  [datenschutz.html](datenschutz.html).
- Kontakt, Transparenz, Gemeinnützigkeit und Förderung stehen in
  [kontakt.html](kontakt.html), [transparenz.html](transparenz.html),
  [gemeinnuetzigkeit.html](gemeinnuetzigkeit.html) und
  [foerderung.html](foerderung.html).
- Englische Legal-Seiten stehen in [en/imprint.html](en/imprint.html) und
  [en/privacy.html](en/privacy.html).
- Site-spezifische Assets liegen unter [assets/](assets).
- Gemeinsame CI-Vorgaben liegen unter [styleguide/](styleguide).

Vor produktiven Änderungen an Rechtsseiten sollten Impressum, Datenschutz und
Statusangaben rechtlich geprüft werden.
