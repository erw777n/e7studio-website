# E7 Studio · Website (e7studio.de)

Statische Website, kein Build-Schritt nötig. Gehostet über GitHub Pages.

## Aufbau

Im Hauptordner des Repos:

- `index.html` – Startseite (Kanalo, Coming soon)
- `impressum.html`, `datenschutz.html`
- `404.html` – eigene Fehlerseite
- `robots.txt`, `sitemap.xml` – für Suchmaschinen
- `CNAME` – verbindet die Domain e7studio.de

Im Ordner `assets/`:

- `style.css` – das komplette Design
- `inter-400.woff`, `inter-600.woff`, `inter-700.woff`, `inter-display-700.woff`, `inter-display-800.woff` – Schrift Inter, lokal eingebunden (keine Verbindung zu Google)
- `inter-OFL.txt` – Lizenz der Schrift (SIL Open Font License, frei nutzbar)
- `favicon.svg`, `apple-touch-icon.png` – Symbol im Browser-Tab und auf dem Handy
- `og-image.png` – Vorschaubild für WhatsApp, LinkedIn & Co.

## Aktualisieren über GitHub

1. Im Repo auf der Hauptseite: **Add file → Upload files**, die Dateien aus dem Hauptordner hineinziehen, **Commit changes**.
2. Den Ordner **assets** im Repo anklicken, dort ebenfalls **Add file → Upload files**, alle Dateien aus `assets/` hineinziehen, **Commit changes**.

Gleichnamige Dateien werden dabei automatisch ersetzt. Nach ein bis zwei Minuten ist die neue Version online (Seite mit Strg + F5 neu laden).

## Domain bei IONOS

| Typ   | Hostname | Wert                 |
|-------|----------|----------------------|
| A     | @        | 185.199.108.153      |
| A     | @        | 185.199.109.153      |
| A     | @        | 185.199.110.153      |
| A     | @        | 185.199.111.153      |
| AAAA  | @        | 2606:50c0:8000::153  |
| AAAA  | @        | 2606:50c0:8001::153  |
| AAAA  | @        | 2606:50c0:8002::153  |
| AAAA  | @        | 2606:50c0:8003::153  |
| CNAME | www      | erw777n.github.io    |

MX-, SPF-, DKIM- und DMARC-Einträge (Mail) nicht verändern.
