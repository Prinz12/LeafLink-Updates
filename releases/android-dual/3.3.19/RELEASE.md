# LeafLink Android 3.3.19

Mehrere Lüfter lassen sich zuverlässiger nacheinander einrichten, auch wenn gleichzeitig mehrere Einrichtungsnetze „LeafLink“ sichtbar sind.

- QR-Code: Die App verbindet gezielt mit dem Lüfter vom Geräteetikett.
- Manuelle Eingabe: Vierstellige Gerätenummer und Gerätecode eingeben. Die App sucht den passenden Lüfter; bei einer mehrdeutigen Gerätenummer wird der QR-Code benötigt. Für diesen Suchweg benötigt Android die genaue Standortfreigabe und eingeschaltete Standortdienste.
- „Weiteren Lüfter hinzufügen“ behält Ziel-WLAN und Passwort für die laufende Einrichtungsrunde im Arbeitsspeicher. Beim Schließen der Einrichtung werden sie verworfen.
- Vorübergehend verlorene Identitätsantworten vor der Gruppenzuordnung werden begrenzt erneut abgefragt. Schreibbefehle werden dabei nicht blind wiederholt.
- Verbindungsfehler werden nicht mehr pauschal als verweigerte Android-Freigabe bezeichnet.

Auf einem Samsung-Handy mit fünf nacheinander eingerichteten zusätzlichen Lüftern geprüft, einschließlich QR-Code, manueller Eingabe und Vorschlägen für freie Partnerplätze. Alle drei Lüfterpaare wurden danach vollständig angezeigt. Automatisierte Setupprüfungen, Emulator und Release-Lint bestanden.

App-Version 3.3.19, Versionscode 28. Installation über die bestehende App erhält Kopplungen, Einstellungen und Hausplan. Keine neue Firmware erforderlich. Den Einrichtungsmodus am gewünschten Lüfter unmittelbar vor der Kopplung aktivieren.
