# LeafLink Android 3.3.10 – Netzwerkrollen bei gespeicherten Lüftern

Unter **Einstellungen → Gespeicherte Lüfter** zeigt jede Gerätekarte jetzt die tatsächliche Netzwerkrolle, beispielsweise **Automatisch · Router (WLAN)** oder **Automatisch · Repeater über 4811**. Master/Slave für die Lüftungsgruppe bleibt davon getrennt.

Die Anzeige liest die aktuelle Gateway-Übersicht und berücksichtigt auch über Funk erreichbare Lüfter. Nach ausbleibender Bestätigung werden Werte als „zuletzt“ gekennzeichnet. Offline-Geräte behalten eine entsprechend markierte historische Anzeige. Fehlende Angaben älterer Firmware werden nicht als bestätigte Automatik dargestellt. Firmware 3.3.12 ergänzt die vollständige Rolleninformation für diese Übersicht.

Die Rollenabfrage läuft bei geöffneten Einstellungen und pausiert während Firmwareupdates. Die gespeicherten Informationen dienen ausschließlich der Anzeige. Alle neuen Texte sind in den zehn unterstützten Sprachen vorhanden.

Geprüft: Android-Hosttests, Releasebuild und Lint, Rollenparser und tatsächliche Gerätekarten im isolierten Emulator sowie Live-Abfragen mit dem Android-HTTP-Client an zwei realen Platinen. App-Daten, Kopplungen und Hausplan bleiben beim normalen App-Update erhalten.

Android ab Version 6.0. Paket `de.prinz.leaflink`, Versionscode 19, unveränderte App-Signatur. In **App-Update** nach der neuen Version suchen und das Update installieren.
