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

**v0.4.7 (Beta)** · Entwickelt von **TheS4int**.

KOBOLD befindet sich in der Beta-Phase. Funktionen und Prüfergebnisse werden weiter getestet und können sich mit kommenden Versionen ändern.

Die Analyse läuft standardmäßig lokal. Ist VirusTotal aktiviert, sendet KOBOLD den SHA-256 des Anhangs zur Abfrage eines vorhandenen Berichts. „Ohne Treffer“ bezieht sich auf die tatsächlich ausgeführten Prüfungen.


## ClamAV beim ersten Start

KOBOLD bringt die ClamAV-Anbindung mit. Das ClamAV-Programm und seine Signaturdatenbank werden separat eingerichtet. Wenn auf Windows x64 eine passende Version verfügbar ist und KOBOLD noch keine eigene Installation hat, erscheint unter **Engines & Einstellungen → ClamAV** ein Installationsangebot. Erst mit **ClamAV installieren** beginnt der Download. **Später** verschiebt die Einrichtung.

Für die Einrichtung und den Signaturdownload ist eine Internetverbindung nötig. Wenn KOBOLD eine bereits vorhandene ClamAV-Installation erkennt, kann es diese für die Anhangsprüfung verwenden.
