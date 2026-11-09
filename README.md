# E7 Studio · Website (e7studio.de)

Statische Website: `index.html`, `impressum.html`, `datenschutz.html`, `assets/`.
Kein Build-Schritt nötig.

## Vor dem Hochladen

1. **Impressum und Datenschutz prüfen:** Angaben sind eingetragen. Sobald du eine
   Umsatzsteuer-ID hast, ergänze sie im Impressum.
2. **Schriften lokal ablegen** (wichtig für den Datenschutz, keine Google-Verbindung):
   Sag Claude Code:
   > Lade die variablen Schriften „Plus Jakarta Sans“ und „JetBrains Mono“ (latin, woff2)
   > von Fontsource herunter und speichere sie als
   > `assets/fonts/plus-jakarta-sans-latin-wght-normal.woff2` und
   > `assets/fonts/jetbrains-mono-latin-wght-normal.woff2`.

   Ohne diese Dateien funktioniert die Seite trotzdem, sie nutzt dann die Systemschrift.

## Online stellen mit GitHub Pages

1. Neues **öffentliches** Repo anlegen, z. B. `e7studio-website`
   (GitHub Pages ist im kostenlosen Plan nur für öffentliche Repos verfügbar).
2. Alle Dateien aus diesem Ordner hochladen (inkl. `CNAME`).
3. Im Repo: **Settings → Pages → Build and deployment → Source: „Deploy from a branch“**,
   Branch `main`, Ordner `/ (root)`, speichern.
4. Unter **Custom domain** `e7studio.de` eintragen und speichern.

## Domain bei IONOS verbinden

In IONOS unter **Domains & SSL → e7studio.de → DNS**:

| Typ   | Hostname | Wert                 |
|-------|----------|----------------------|
| A     | @        | 185.199.108.153      |
| A     | @        | 185.199.109.153      |
| A     | @        | 185.199.110.153      |
| A     | @        | 185.199.111.153      |
| CNAME | www      | erw777n.github.io    |

- Einen vorhandenen A-Eintrag für `@` (z. B. die IONOS-Parkseite) ersetzen.
- **MX-Einträge nicht anfassen**, sonst funktioniert info@e7studio.de nicht mehr.
- Nach der DNS-Umstellung (kann bis zu 24 Std. dauern) in GitHub unter
  Settings → Pages **„Enforce HTTPS“** aktivieren.
