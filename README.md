# Auto-Service

Web-App für alle Wartungen deiner Autos – mit Teilen, Artikelnummern, Preisen und Erinnerung an den nächsten Service. Läuft offline und lässt sich auf iPhone/iPad als App zum Home-Bildschirm hinzufügen.

## Funktionen
- **Fahrzeuge** mit Kennzeichen, FIN, HSN/TSN, Motorcode, Öl-Spezifikation und Reifengröße
- **Erkennung** von Marke und Modell (ca. 40 Marken offline): Vorschläge beim Tippen, Tippfehler- und Schreibweisen-Korrektur, Marke wird aus dem Modell ergänzt; Kennzeichen, FIN, Reifengröße, Ölviskosität und Baujahr werden ins richtige Format gebracht (jeweils mit „Rückgängig“)
- **Services** mit Datum, km-Stand, Werkstatt, beliebig vielen Teilen (Bezeichnung, Hersteller, Artikelnummer, Menge, Einheit, Preis), Arbeitslohn und Sonstigem – die Summe wird automatisch berechnet
- Bekannte Teile werden vorgeschlagen und füllen Artikelnummer und letzten Preis automatisch aus; „Als Vorlage“ kopiert einen alten Service
- **Herstellerwerte je Modell** (`intervalle.json`): Wartungsintervalle für über 300 Modelle aus Internet-Recherche (Hersteller-Betriebsanleitungen, carwiki.de, repareo.de u. a.), jeweils mit Quelle und Verlässlichkeit. Werden beim Anlegen vorgeschlagen und lassen sich bei vorhandenen Autos übernehmen. Ohne Modelldaten gelten Richtwerte.
- **Wartungsplan** pro Fahrzeug (Ölwechsel, Inspektion, HU/TÜV …) mit Intervall nach Monaten und/oder km
- **Erinnerung**: pro Wartungspunkt einstellbar, wie viele Tage vorher (Standard in den Einstellungen); bei km-Intervallen wird das Datum aus deiner Fahrleistung geschätzt
- Erinnerung als **Kalender-Termin mit Alarm** (.ics), Mitteilungen und App-Badge in der installierten App
- **Teile-Übersicht** mit Suche (Artikelnummer antippen = kopieren)
- **Kosten** pro Jahr, nach Art, Teile vs. Arbeitslohn, pro 100 km
- **Backup** (JSON) und Export als Tabelle (CSV für Excel)
- Update-Hinweis „App aktualisieren“, sobald eine neue Version online ist

## Updates veröffentlichen
Bei jeder Änderung `APP_VERSION` in `index.html` **und** `version.json` auf dieselbe neue Nummer setzen.

Die Daten liegen nur lokal im Browser des Geräts (localStorage).
