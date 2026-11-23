![KOBOLD – Mail Thread Analyzer für Windows. Der Kobold hält einen offenen Briefumschlag.](./thes4int-kobold-banner.png)

# THΞ S4INT · KOBOLD

**KOBOLD** unterstützt Helpdesk und Security-Teams bei der Erstprüfung verdächtiger E-Mails. Die Windows-App analysiert exportierte `.eml`- und `.msg`-Dateien und fasst Befunde für die Übergabe zusammen.

## Funktionen

- Absender, Antwortadressen, Mail-Header, Links, QR-Codes und Anhänge prüfen.
- Anhänge lokal mit YARA-X, Microsoft Defender und ClamAV scannen. Optional vorhandene VirusTotal-Berichte per SHA-256 abfragen.
- Mailverläufe und manuell ausgewählte Referenzmails auf Änderungen bei Antwortdomains, Linkzielen und Zahlungsdaten vergleichen.
- Gemeinsame Antwortadressen, Linkhosts und identische Anhänge über mehrere Mails erkennen.
- Ticketbefunde kopieren und HTML-Fallberichte exportieren.
- Prüfstatus je Anhang und Engine einsehen, lokale Engines testen und Begriffe im Glossar nachschlagen.

## Entwicklungsstand

**v0.4.7** · Entwickelt von **TheS4int**.

Die Analyse läuft standardmäßig lokal. Ist VirusTotal aktiviert, sendet KOBOLD den SHA-256 des Anhangs zur Abfrage eines vorhandenen Berichts. „Ohne Treffer“ bezieht sich auf die tatsächlich ausgeführten Prüfungen.
