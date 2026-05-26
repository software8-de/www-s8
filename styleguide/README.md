# Software8 Styleguide

Dieses Verzeichnis ist die verbindliche CI-Quelle für Software8 und alle
abgeleiteten Vertical-Seiten wie `notariat8.de`.

## Zweck

Software8 stellt die Dachmarke, die Idee von Organisation as Code und den
gemeinsamen visuellen Rahmen. Vertical-Projekte dürfen fachlich und inhaltlich
eigene Schwerpunkte setzen, sollen aber sichtbar zur Software8-Familie gehören.

## Verbindliche Grundlagen

- `tokens.css` definiert Farben, Flächen, Typografie, Radien, Schatten und
  Abstände.
- Neue Landingpages sollen diese Tokens direkt importieren oder synchron daraus
  erzeugte Werte verwenden.
- Lokale Abweichungen sind erlaubt, wenn sie ein Vertical klarer machen; sie
  dürfen die Familienzugehörigkeit nicht aufheben.

## Nutzung

Eine statische Vertical-Seite kann die Tokens so importieren:

```css
@import url("https://software8.de/styleguide/tokens.css");
```

Innerhalb dieses Repos nutzt `assets/site.css` den relativen Import:

```css
@import url("../styleguide/tokens.css");
```

## Gemeinsame 8-Brand-Assets

Alle bestehenden und künftigen `*8`-Repos sollen ihre 8er-Icons aus
[bild8/www-b8](https://github.com/bild8/www-b8) beziehen. Der veröffentlichte
Katalog liegt unter:

```text
https://bild8.de/assets/8/svg/{id}.svg
https://bild8.de/assets/8/png_32/{id}_32.png
https://bild8.de/assets/8/png_192/{id}_192.png
https://bild8.de/assets/8/png_526/{id}_526.png
```

`{id}` steht für `a8`, `b8`, ..., `z8`. Dieses Repo nutzt `s8`; Notariat8/NaC
nutzt `n8`; `www-b8` bleibt Quelle und Auslieferungsort für den Gesamtkatalog.
Repos sollen die CDN-Pfade referenzieren. Lokale Kopien sind nur für
Offline-Oberflächen oder Tests zulässig und müssen aus `www-b8` stammen.

## Nächste Ausbaustufe

Später sollen hier gemeinsame Layout-Templates, Komponentenregeln und
Beispiele für Vertical-Landingpages liegen. `www-s8` bleibt dabei der
kanonische Ort für CI-Entscheidungen.
