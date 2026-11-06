# LeafLink 3.3.7 Beta – Rückkehr ins gespeicherte WLAN

Behebt einen Fehler nach der QR-Kopplung mit „Gespeichertes WLAN beibehalten“:
Der Lüfter konnte eine WLAN-Verbindung melden, während er für die App und die
lokale Webseite nicht mehr erreichbar war.

Die Firmware bestätigt den Rückkehrbefehl zunächst und führt den Netzwechsel
erst nach Abschluss der geschützten Befehlsverarbeitung aus. Beim Wechsel vom
Einrichtungs-WLAN ins Heim-WLAN wird das Funkmodul vollständig neu initialisiert,
wie bereits bei der Übertragung neuer WLAN-Daten. Schlägt diese Umschaltung fehl,
kehrt das Gerät in den Einrichtungsmodus zurück.

Zusammen mit **Android-App 3.3.5** verwenden. Diese verbessert zusätzlich die
Geräteerkennung bei gefilterten WLAN-Rundrufen und die Befehlswarteschlange.
App und Lüfterfirmware werden getrennt aktualisiert. Vorhandene Kopplungen,
WLAN-Daten, Gruppen, Räume, Hauspläne und Wall-Zuordnungen bleiben erhalten.

Die WLAN-Rückkehr wurde auf einem realen Lüfter geprüft; danach waren Webseite
und direkte App-Kommunikation wieder erreichbar. Stufenänderungen aus der App
wurden auf beiden Lüftern der Testgruppe bestätigt. Die Korrekturen aus 3.3.6 für
den Wall-Netzwechsel bleiben enthalten; Wall Control 0.6.2 bleibt aktuell.

In der App unter **Firmware-Updates** die Beta-Versionen einschließen und erneut
nach Updates suchen. Voraussetzungen: ESP8266 ESP-12F, 4 MiB Flash, Hardwareprofil
und bestehendes A/B-Layout 2. Nur die signierte `firmware.bin` über den regulären
Updateweg verwenden. Ein Werksreset ist nicht erforderlich.
