# Malerei Hartl – Maler (Konzept)

Live: https://sakasolutions.github.io/malereihartl/

## Status: Konzeptseite (fiktiver Betrieb)

Diese Seite ist ein **Design-Konzept von SAKA Solutions** für Werbung auf TikTok/Instagram und als Beispiel für Interessenten. Der Betrieb ist erfunden.
- `<meta name="robots" content="noindex, nofollow">` **bleibt drin**, solange der Betrieb fiktiv ist (sonst indexiert Google einen erfundenen Betrieb).
- Kontaktdaten sind Platzhalter (`000`-Nummern, `…-beispiel.de`, „Beispielstraße“).
- Im Footer steht „Design-Konzept von SAKA Solutions, fiktiver Beispielbetrieb“. Nicht entfernen.
- Fotos: Unsplash (freie Lizenz).
- Wird daraus eine echte Kundenseite: `noindex` entfernen, echte Daten, echte Fotos und echte Google-Bewertungen einsetzen, Impressum/Datenschutz verlinken.

## Diese Seite

- **Branche:** Maler, fiktive „Malerei Hartl“, Heidenheim an der Brenz.
- **Vorlage:** Dribbble „Painting Services Landing Page“ von Framdex („Colorix“), nur der Hero war vorgegeben, der Rest im selben Stil ergänzt.
- **Farben:** Orange `#FF6B1A`, Schrift `#16141B`, Hintergrund `#FFFBF7`, Pfirsich-Töne `#FDF4EC` / `#FBE8D8` / `#F8D6BA`. Schrift: Plus Jakarta Sans.
- **Aufbau:** Topbar → Navigation mit orangem Pill-Button → warmer Hero mit Malerin (Foto blendet weich in den Hintergrund) → 6 Leistungskarten → Vorher/Nachher-Schieberegler (gleiches Wohnzimmer, „Vorher“ per CSS-Filter vergilbt) → Projekte → Ablauf in 4 Schritten → Bewertungen (Beispiel) → FAQ → Kontakt (mailto) → Footer.
- **Kontakt-Platzhalter:** 07321 000 222, info@hartl-beispiel.de.
- **Hinweis:** Abschnitte blenden beim Scrollen dezent ein. Falls der Inhaber das als zu viel Bewegung empfindet: entfernen.

## Arbeitsweise (gilt für Mac, Web und Handy)

- **Zu Beginn:** `git pull`, damit du auf dem neuesten Stand bist (es wird von mehreren Geräten aus gearbeitet).
- **Diese Datei ist das gemeinsame Gedächtnis.** Chats werden nicht zwischen Geräten synchronisiert. Wenn eine grundsätzliche Entscheidung getroffen wird (Farben, Stil, Inhalte, Regeln, was der Kunde will oder nicht will), trage sie unten unter **Entscheidungen & Verlauf** mit Datum ein und committe sie zusammen mit der Änderung.
- **Veröffentlichung:** GitHub Pages aus Branch `main`, Ordner `/ (root)`. Alles, was auf `main` landet, ist nach ein bis zwei Minuten live.
- **Aufbau:** eine einzige `index.html` mit Inline-CSS und -JS, Bilder in `img/`. Kein Framework, kein Build-Schritt.
- **Alle Farben** stehen als CSS-Variablen in `:root`. Neue Farben nur dort anlegen.

## Stil-Regeln des Inhabers (Sinan, SAKA Solutions)

- **Ruhig und seriös statt verspielt.** Keine Laufbänder/Ticker, keine schwebenden oder wippenden Elemente, keine Hover-Effekte mit Anheben/Zoomen, keine dekorativen „Chips“ um Personen herum. Erlaubt: dezente Farbübergänge, Aufklappen von FAQ/Menü/Reitern.
- **Farben nie selbst erfinden:** immer aus einer Vorlage (Dribbble-Shot) oder aus bestehenden Markenfarben ableiten. Abgelehnt wurden z. B. Dunkelgrün + Senfgelb und erdig-matte Kombinationen.
- **Personen im Hero:** sauber angeordnet (zentriert, nichts über dem Gesicht, Kopf unter der Navigation). Lieber weglassen als verspielt.
- **Keine erfundenen Bewertungen** als echt ausgeben: Bewertungen sind als „Beispielbewertung“ markiert, keine vollen Namen.
- **Handy zuerst prüfen:** Bei 375 px darf nichts breiter als der Bildschirm sein (`document.documentElement.scrollWidth === innerWidth`). Grid-Spalten mit `minmax(0,1fr)` statt `1fr`, wenn darin scrollende Leisten stecken.
- **Navigation** bleibt am Desktop (1200–1440 px) einzeilig (`white-space: nowrap`).
- **Sprache:** Deutsch, echte Texte, kein Lorem ipsum.

## SEO-Standard

`lang="de"`, Title ca. 55–60 Zeichen mit Leistung + Ort, Meta-Description ca. 150 Zeichen, Canonical, Open Graph, genau eine H1 mit Keyword + Ort, saubere H2/H3, Alt-Texte, width/height an Bildern, `loading="lazy"` unterhalb des sichtbaren Bereichs, JSON-LD passend zur Branche (plus FAQPage, wenn es eine FAQ gibt).

## Entscheidungen & Verlauf

- 2026-09-21: Seite nach Vorlage gebaut, Desktop vom Inhaber abgenommen.
