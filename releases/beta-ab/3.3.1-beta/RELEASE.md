# LeafLink 3.3.1 Beta – geschützte Kopplung und ESP8266-Stackkorrektur

Behebt den Fehler „Geschützter Lüfter antwortet nicht“ bei der Einrichtung und Neustarts bei anschließenden Geräteabfragen. SHA256, HMAC und AES-GCM laufen auf einem separaten BearSSL-Stack; große Kopplungs- und Rollbackpuffer sind vom Paketverteiler getrennt. Bei Speichermangel wird die Anfrage abgelehnt. Authentifizierung und Replay-Schutz bleiben aktiv.

## Installation und Sicherheitsumstellung

- Zuerst die [Android-App 3.3.1](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.1) installieren. Unter **Firmware-Updates** die Option **Beta-Versionen anzeigen** aktivieren und nach Updates suchen.
- Für ESP8266 ESP-12F mit 4 MiB Flash, Hardwareprofil und bereits vorhandenem A/B-Layout 2. Das signierte BIN ist ein Anwendungsupdate, kein Vollflash und kein Paket für Originalfirmware oder das frühere Safe-Profil.
- Beim Wechsel von 3.2.x gehört die Gerätecode-Kopplung zur Sicherheitsumstellung: Einrichtung am Lüfter physisch öffnen, in der App **Lüfter koppeln** wählen und den individuellen Gerätecode eingeben oder scannen. Den Code vor dem Update bereithalten. Bestehende WLAN- und Gerätedaten werden beim A/B-Update erhalten.
- Bereits unter 3.3.0 gespeicherte Handyzugänge bleiben erhalten. Ältere ungeschützte Steuerprogramme sind mit der neuen Geräteauthentifizierung nicht kompatibel.
- Bei vorhandener Wall Control die Sicherheitsumstellung der gesamten Anlage vorbereiten: kompatible Wall-Control-Firmware 0.6.0 und Übernahme ihres Funknetzschlüssels sind Teil der Migration. Dieses Lüfterupdate aktualisiert die Wall Control nicht. Die vorhandene Wall-Zuordnung wird nicht absichtlich gelöscht; die vollständige Anlagenmigration ist gesondert zu prüfen.

## Prüfstand

Identisches signiertes Paket auf einer echten Testplatine mit Samsung SM-S918B und App 3.3.1 geprüft: Gerätecode, Kopplung, Handyanmeldung, Funknetzschlüssel, verschlüsselte WLAN-Übertragung, WLAN-Rückkehr und Raumzuordnung erfolgreich. Zwei anschließende Messreihen mit insgesamt 126 frischen Statusabfragen waren ohne Anfragefehler oder Neustart; echte Sensormesswerte erschienen in der App. Beim Einrichtungsübergang wurde ein geplanter Neustart zur Netzwerkwiederherstellung beobachtet.

211 Firmware-Hosttests, 44 native Testprogramme, 957 Wall-Kryptografieprüfungen, unabhängige AES-GCM-Vektoren sowie Speicherfehler-, Replay- und Manipulationsprüfungen bestanden. Codec-Interoperabilität, Hardware-Build, Android-Hosttests, Build/Lint und API-23-Emulatorprüfungen bestanden. Langzeitbetrieb, vollständige Wall-Anlagenmigration und TÜV-Prüfung sind dadurch nicht ersetzt.

Profil: **hardware** · Kanal: **beta-ab** · Layout: **2**. Für diese Version wird kein Safe-Paket veröffentlicht.
