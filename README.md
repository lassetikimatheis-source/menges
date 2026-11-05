# MENGES OS

Unabhängiger Konzeptprototyp für eine Praktikumspräsentation. Keine Verbindung zu Systemen der Claus R. Menges GmbH. Sämtliche Namen, Adressen und Verwaltungsdaten in der Demo sind fiktiv. Das Logo stammt von der öffentlich zugänglichen Unternehmenswebsite und dient ausschließlich der visuellen Orientierung des Konzepts.

## Start

Node.js 20.19+ oder 22.12+ erforderlich.

```sh
npm install
npm run dev
```

Anschließend http://127.0.0.1:5173 öffnen. Nach der Installation funktioniert die Anwendung ohne Internet und ohne API-Schlüssel. Alle Bibliotheken und das Logo werden lokal geladen. Änderungen werden im localStorage des jeweiligen Browsers gespeichert. „Demo zurücksetzen“ stellt den Ausgangszustand wieder her. Als feste Präsentationszeit dient der 5. November 2026.

```sh
npm run build
npm run preview
```

## Präsentation in drei Minuten

1. In der Übersicht 160 fiktive Einheiten, offene Meldungen und den Monatsverlauf erläutern.
2. „Neue Schadensmeldung“ öffnen und „Beispiel einsetzen“ wählen.
3. „Mit KI analysieren“ wählen. Kategorie, Priorität, nächste Schritte und den editierbaren Antwortentwurf zeigen. Die Analyse ist eine transparente, lokale Regelsimulation, keine echte KI.
4. Vorgang speichern. Im Dashboard steigt die Zahl offener und dringender Vorgänge. Über Schadensmanagement lassen sich Beschreibung, Titel, Priorität und Status bearbeiten.
5. Eigentümer-Reporting öffnen, November 2026 wählen, Bericht generieren und als PDF exportieren.

Der integrierte Präsentationsmodus führt durch diesen Ablauf. E-Mails werden nicht versendet. Der Posteingang erzeugt bearbeitbare Entwürfe und speichert Statusänderungen. Berichte verwenden den jeweils aktuellen Datenbestand; „offen“ umfasst offene Vorgänge und solche in Bearbeitung. Die Bearbeitungszeit ist die mittlere Kalendertagsdifferenz zwischen Eingang und Abschluss. Aufgaben lassen sich unabhängig von Vorgängen abhaken.

## Technik

React, TypeScript, Vite, Lucide, Recharts und jsPDF. Bewusst ohne Backend oder Registrierung. Responsive CSS, keine externen Fonts oder CDNs. Illustration der Immobilien als lokale CSS-Grafik, keine Fotos echter Demo-Objekte. Für diese rein lokale Anwendung wird Vite statt Next.js verwendet, um Server- und Deployment-Komplexität zu vermeiden.
