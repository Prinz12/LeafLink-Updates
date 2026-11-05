# LeafLink Android 3.3.1 – Diagnose und Anleitung für die geschützte Kopplung

- Bei einer fehlenden Antwort nennt die App den betroffenen Einrichtungsschritt: Gerätecode prüfen, Kopplung speichern oder Handy anmelden.
- Die Anleitung beschreibt das geschützte LeafLink-WLAN und das dreiminütige Kopplungsfenster.
- Diagnosemeldungen enthalten keine Gerätecodes, Schlüssel oder WLAN-Passwörter.
- Bestehende App-Daten, Gruppen, Hausplan und Handyzugänge bleiben bei der Updateinstallation erhalten. HAPLA verwendet weiterhin seinen eigenen Einrichtungsweg.

## Firmware-Korrektur

Der Fehler „Geschützter Lüfter antwortet nicht“ wurde auf einer ESP8266-Testplatine auf einen überlaufenden Funktionsstack in der Firmware zurückgeführt. Die zugehörige Firmwarekorrektur ist in **LeafLink 3.3.1** enthalten. Das App-Update allein installiert keine Lüfterfirmware. Die geschützte LeafLink-Verbindung setzt die Sicherheitsumstellung ab Firmware 3.3.0 und eine Kopplung mit dem individuellen Gerätecode voraus; für die korrigierte ESP8266-Verbindung ist Firmware 3.3.1 erforderlich.

Die Hinweise zur Übernahme vorhandener Wall-Anlagen aus [Version 3.3.0](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.0) gelten weiterhin. Eine vollständige Anlagenmigration und die physischen Sicherheitsfreigaben sind gesondert zu prüfen.

## Installation und Prüfung

In LeafLink **App-Update** öffnen, nach Updates suchen, herunterladen und die Android-Installation bestätigen. Als Update über die vorhandene App installieren.

Paket `de.prinz.leaflink`, versionCode 10, Android ab API 23, unverändertes Release-Signaturzertifikat. Hosttests, Android-Builds, Lint und API-23-Emulatorprüfungen einschließlich Android Keystore und geschützter Einrichtung sind bestanden. Die signierte APK wurde zusätzlich datenerhaltend auf einem Samsung SM-S918B installiert und zurückgelesen.
