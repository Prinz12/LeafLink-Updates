# LeafLink Lüfter-Firmware 4.0.0

Die Browseroberfläche läuft per HTTPS direkt am Lüfter. Gerätestatus und Einstellungen erfordern eine Anmeldung. Über die gekoppelte App lässt sich ein verlorenes Bediengerät sperren. Erreichbare Lüfter wechseln sofort den Netzschlüssel. Ausgeschaltete Lüfter bleiben in der App zur Nachholung sichtbar.

Zuerst die LeafLink-App 4.0.0 installieren, anschließend die Lüfter-Firmware aktualisieren.

**Browserzugang ohne USB einrichten.** Nach dem Update auf dem gekoppelten Android-Gerät, das die Anlage verwalten soll, die Gerätedetails des Lüfters öffnen. **Browserzertifikat einrichten oder erneuern** wählen und bestätigen. Die App stellt das Zertifikat über WLAN aus und prüft den HTTPS-Zugang direkt am Lüfter.

**Weitere Bediengeräte.** In der App **Stammzertifikat exportieren** wählen. Die öffentliche Datei `LeafLink-CA.crt` auf jedem gewünschten Bediengerät als vertrauenswürdige CA im Betriebssystem bzw. Browser installieren. Vorher den SHA-256-Fingerabdruck vergleichen. Den angezeigten Gerätenamen im lokalen Netz öffnen. Die Einrichtung benötigt keinen PC. Das Administratorgerät wird zum Erneuern der Zertifikate benötigt.

**Verlust oder Wechsel des Administrators.** Gehen Bediengerät oder App-Daten verloren, das Einrichtungs-WLAN am Lüfter vor Ort öffnen und die Einrichtung mit dem neu gekoppelten Administratorgerät wiederholen. Anschließend dessen Stammzertifikat auf den Bediengeräten installieren.

Diese signierte Firmware ist für LeafLink-Lüfter mit ESP8266, 4 MiB Flash und vorhandenem A/B-Bootlayout 2 bestimmt. Die App prüft das Firmware-Abbild vor der Übertragung. Bei Gateway-Lüftern mit 4.0.0 erfordern spätere direkte Firmware-Updates ein gültiges Gerätezertifikat.

Das zur Firmware gehörende LGPL-Paket steht bei den Downloads dieser Version.
