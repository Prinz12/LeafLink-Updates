# Wall Control 0.6.8 Beta – Gateway für sichere App-Sitzungen

Leitet das neue geschützte App-Protokoll an Lüfter weiter. Die direkte Wall-Bedienung, das Funknetz und vorhandene Zuordnungen bleiben erhalten. Für LILYGO T-Display ESP32 mit vorhandenem 16-MiB-Layout; reguläres App-Slot-Update. Die unveränderte TFT-Datei liegt der Vollständigkeit halber bei.

## Reihenfolge für dieses Sicherheitsupdate

1. Bei App-Zugriff über die Wall zuerst **Wall Control 0.6.8 Beta** aktualisieren.
2. Alle betroffenen Lüfter auf **Firmware 3.3.25 Beta** bringen: signiertes Hardware-A/B-Image über die vorhandene Web-Serviceoberfläche oder den verifizierten A/B-Installer installieren und den bestätigten Start prüfen. Kein Vollflash, kein Zurücksetzen.
3. Danach **Android 3.3.27** über den App-Updatekanal installieren. Die App als Update installieren, nicht deinstallieren.

**Alte und neue App-/Lüfterstände sind für die geschützte Steuerung nicht kompatibel.** Die alte App kann nach dem Firmwarewechsel auch die abschließende OTA-Statusprüfung nicht mehr ausführen. Deshalb diesen Übergang über die Web-Serviceoberfläche bzw. den verifizierten A/B-Installer durchführen. Eine bereits aktualisierte App kann alte Lüfter nicht per App-OTA aktualisieren; in diesem Fall ebenfalls den Web-/A/B-Weg verwenden.

Kopplungen, Gerätecodes, Gruppen, WLAN-Einstellungen und vorhandene Wall-Zuordnungen bleiben erhalten. Kein erneutes Anlernen erforderlich. HAPLA-Geräte bleiben unterstützt. Das Nextion-Display bleibt bei HMI 302; kein TFT-Update erforderlich.

Zusammengehörige Versionen: [Firmware 3.3.25 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.25-beta), [Android 3.3.27](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.27), [Wall 0.6.8 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.8-beta).

## Prüfung

Neue App-Sitzungen erhalten einen frischen authentifizierten Schlüsselkontext. 290 Verschlüsselungen mit Paketverlust, über 40 separaten App-Prozessneustarts und simulierten Firmware-Neustarts ergaben kein doppeltes Schlüssel/Nonce-Paar. Replay-, Manipulations-, Zählergrenzen-, Kopplungs-, Wall-, Build- und Android-Emulatorprüfungen bestanden. Kein Live-Hardwaretest dieses Builds. Die Veröffentlichung installiert nichts automatisch.
