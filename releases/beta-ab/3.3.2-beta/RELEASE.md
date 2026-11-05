# LeafLink 3.3.2 Beta – OTA-Speicherprüfung

Die A/B-Firmware berücksichtigt jetzt die getrennten Speicherphasen von Upload und Signaturprüfung. Der 4-KiB-Schreibpuffer wird vor der RSA-Prüfung freigegeben. Vor dem ersten Flash-Schreibzugriff wird der verfügbare Speicher zusätzlich geprüft. Signatur, Hash, Profil, Versionsschutz, Bootbestätigung und Motor-Sicherheitsprüfungen bleiben erhalten.

Zuerst [Android-App 3.3.2](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.2) installieren. Sie behebt die falsche Kompatibilitätsanzeige bei WLAN-Geräten mit ruhendem Mesh-Funknetz. Anschließend unter **Firmware-Updates** die Beta-Versionen aktivieren.

## Voraussetzung und Reparatur älterer Firmware

Für ESP8266 ESP-12F mit 4 MiB Flash, Hardwareprofil und bestehendem A/B-Layout 2. Das signierte BIN ist ein Anwendungsupdate, kein Vollflash. Es gibt kein neues Safe-Paket.

Wenn 3.3.0 oder 3.3.1 die Vorbereitung bereits mit „Zu wenig Speicher für sicheres OTA“ abbricht, kann die neue App diese alte Firmware-Sperre nicht beheben. Dann ist einmalig eine datenerhaltende USB-Serviceinstallation mit vorheriger vollständiger Sicherung und Geräteprüfung erforderlich. Kein Löschen der Geräteeinstellungen vornehmen.

Bestehende Handykopplungen und Gerätedaten bleiben beim A/B-Update erhalten. Beim Wechsel von 3.2.x gehört die physisch freigegebene Gerätecode-Kopplung zur Sicherheitsumstellung. Vorhandene Wall-Anlagen benötigen kompatible Wall-Control-Firmware 0.6.0 und die abgestimmte Übernahme des Funknetzschlüssels. Dieses Paket aktualisiert keine Wall Control.

## Prüfstand

211 Firmware-Hosttests, alle 44 nativen Testprogramme, Codec-Interoperabilität, Hardware-Build mit Stackprüfung sowie Android-Hosttests, Build/Lint und API-23-Emulatorprüfungen bestanden. Die Prüfungen ersetzen keinen Langzeitbetrieb, keine vollständige Wall-Anlagenmigration und keine TÜV-Prüfung.

Profil: **hardware** · Kanal: **beta-ab** · Layout: **2**.
