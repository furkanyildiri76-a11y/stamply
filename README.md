# Stamply – öffentliche Website

Responsive, deutschsprachige Marketing-Website für Stamply. **Statisches HTML/CSS/JavaScript**, ohne Framework, Datenbank oder Build-Prozess. Direkt GitHub- und Webhosting-fähig.

## Lokal ansehen

`index.html` im Browser öffnen. Alternativ im Projektordner:

```bash
python3 -m http.server 8080
```

Danach `http://localhost:8080` öffnen.

## Auf GitHub hochladen

1. Neues Repository auf github.com erstellen (z. B. `stamply-website`).
2. Alle Dateien aus diesem Ordner in das Repository hochladen (inklusive `assets`).
3. Optional lokal Git verwenden:

```bash
git init
 git add .
 git commit -m "Initial Stamply website"
 git branch -M main
 git remote add origin https://github.com/DEIN-NAME/stamply-website.git
 git push -u origin main
```

## Hosting

- **GitHub Pages:** Repository → Settings → Pages → Deploy from branch → `main` → `/ (root)`. Für GitHub Pages ist die Seite sofort geeignet.
- **Netlify / Cloudflare Pages:** GitHub-Repository verbinden; Build-Command leer lassen, Ausgabeordner `/` bzw. Projekt-Root.
- **Klassisches Webhosting:** Inhalt des Ordners per FTP/SFTP in das öffentliche Webverzeichnis hochladen.

## Vor dem Livegang UNBEDINGT ändern

- `hello@stamply.example` in `index.html` durch eine echte Kontaktadresse ersetzen. Der CTA öffnet derzeit nur ein E-Mail-Programm; **es gibt noch keine echte Registrierung oder Warteliste**.
- `impressum.html` und `datenschutz.html` durch rechtlich geprüfte Texte ersetzen; insbesondere bei Sitz der Gesellschaft in Malta.
- Google Fonts im CSS auf lokale Schriften umstellen oder die externe Einbindung datenschutzrechtlich prüfen.
- Markenlogo, Domain, endgültige Preisangaben und Steuerausweisung prüfen.
- QR-Grafik im Aufstellerbereich ist **nur eine nicht scanbare Designillustration**.

## Was noch NICHT implementiert ist

Kein Login, keine Zahlungen, keine Wallet-Karten, keine QR-Generierung, keine Datenbank, keine Mitarbeiter-Scannerfunktion und keine echte Bestellabwicklung. Diese Funktionen gehören zur späteren SaaS-Plattform und benötigen sichere Backend-Dienste.

## Dateien

- `index.html` – Startseite, Funktionen, Preise, FAQ, CTA
- `styles.css` – Responsive Design
- `script.js` – Mobiles Menü und Jahreszahl
- `assets/favicon.svg` – Vorläufiges Icon
- `impressum.html`, `datenschutz.html` – ausdrücklich unvollständige Platzhalter
