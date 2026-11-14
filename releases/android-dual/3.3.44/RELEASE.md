# LeafLink Android 3.3.44 – Android 16 und zuverlässige Kommunikation

Die App verwendet jetzt Android 16 als Zielversion (`targetSdk 36`).
**Voraussetzung: Android 9 oder neuer (API 28).**

- System-Zurück führt aus Hauptseiten wieder zur Startseite und aus
  Netzwerkdetails zunächst zur Netzwerkübersicht. Die neue Android-
  Zurück-Schnittstelle bleibt mit dem bisherigen Verhalten auf Android 9
  kompatibel.
- Kopfzeilen, Navigation und Netzwerkübersicht berücksichtigen Systemleisten
  und Kameraausschnitte. Smartphone-, Tablet- und Querformatansichten wurden
  geprüft.
- Enthält die Kommunikationsverbesserungen der App 3.3.43: gezielte
  Wiederholungen von Leseabfragen, geprüfte Antwortzuordnung und geordnete
  Befehlswarteschlangen bei vorübergehenden Funkverlusten.

Tests auf Android 9, Android 16 und einem echten Android-17-Handy bestanden.
Im Verbindungstest mit zwölf Lüftern waren 240 von 240 authentifizierten
Abfragen und 231 von 231 HTTP-Abfragen erfolgreich, ohne Lüfterneustart.
Einzelne UDP-Pakete können weiterhin verloren gehen; der Test bestätigt keine
unbegrenzte Langzeitstabilität. Der Flottentest verwendete Firmware 3.3.42 Beta.

Als Update ohne Deinstallation installieren. Kopplungen, Einstellungen und
Hausplan bleiben erhalten. Wer bereits App 3.3.44 installiert hat, verwendet
dieselbe geprüfte APK. Diese Veröffentlichung enthält ausschließlich das
App-Update; Firmware wird separat aktualisiert.
