# LeafLink Android 3.3.0 – Gerätecode-Kopplung und geschützte Steuerung

- LeafLink-Lüfter mit individuellem Gerätecode koppeln, wahlweise per Eingabe oder QR-Scan.
- Gerätebezogene, verschlüsselte Steuerbefehle und getrennte Handyzugänge verwalten.
- WLAN-Zugangsdaten verschlüsselt an den Lüfter übertragen.
- Firmware-Updates für die geschützte Verbindung vorbereiten und übertragen.
- Einen bestehenden Wall-Funknetzcode übernehmen und bei der Kopplung das gespeicherte WLAN beibehalten.
- HAPLA-Geräte werden weiterhin über ihren eigenen Protokollpfad unterstützt.

## Voraussetzung für LeafLink-Lüfter

Die LeafLink-Steuerung dieser App setzt **Firmware 3.3.0 und eine einmalige Kopplung mit dem Gerätecode** voraus. LeafLink-Lüfter mit älterer Firmware lassen sich mit der neuen geschützten Steuerung noch nicht bedienen. Das App-Update aktualisiert die Lüfterfirmware nicht automatisch.

Nach dem Firmware-Update die Einrichtung am Lüfter öffnen und in der App **Lüfter koppeln** wählen. Den vorhandenen Gerätecode eingeben oder den QR-Code scannen. Mit **Gespeichertes WLAN beibehalten** kann das vorhandene WLAN weiterverwendet werden.

Für die Übernahme einer Wall-Control-Anlage gehört Wall Control 0.6.0 zur Sicherheitsumstellung. Deren Netzwerkcode zuerst über **Wall-Funknetz übernehmen** importieren und anschließend die Lüfter koppeln. Die praktische Migration einer vollständigen Anlage und die physischen Sicherheitsfreigaben bleiben Teil der Hardwareprüfung.

## Installation und Prüfstand

In der vorhandenen App **App-Update** öffnen, nach Updates suchen, herunterladen und die Android-Installation bestätigen. Als Update über die vorhandene App installieren. Vorhandene App-Daten, Gruppen und Hausplan bleiben erhalten.

Paket `de.prinz.leaflink`, versionCode 9, Android ab API 23, bisheriges LeafLink-Signaturzertifikat. Die APK wurde mit dem Release-Schlüssel signiert. Android-Builds, Lint, Hosttests und Emulatorprüfungen einschließlich des Android Keystore auf API 23 sind erfolgreich.
