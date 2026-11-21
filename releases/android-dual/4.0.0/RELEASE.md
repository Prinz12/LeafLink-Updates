# LeafLink für Android 4.0.0

Unter **Einstellungen → Gerätezugänge** lässt sich ein verlorenes Bediengerät sperren. Mit Firmware 4.0.0 wechseln erreichbare, gekoppelte Lüfter dabei auf einen neuen Netzschlüssel. Die App zeigt ausstehende Lüfter an und bestätigt den Abschluss nach dem erneuten Kontakt.

Zuerst die App auf allen weiter verwendeten Bediengeräten aktualisieren, anschließend die Lüfter. Für die App ist Android 9 oder neuer erforderlich. Die APK lässt sich über die bestehende Installation installieren.

**Browserzugang ohne USB einrichten.** Nach dem Update auf dem gekoppelten Android-Gerät, das die Anlage verwalten soll, die Gerätedetails des Lüfters öffnen. **Browserzertifikat einrichten oder erneuern** wählen und bestätigen. Die App stellt das Zertifikat über WLAN aus und prüft den HTTPS-Zugang direkt am Lüfter.

**Weitere Bediengeräte.** In der App **Stammzertifikat exportieren** wählen. Die öffentliche Datei `LeafLink-CA.crt` auf jedem gewünschten Bediengerät als vertrauenswürdige CA im Betriebssystem bzw. Browser installieren. Vorher den SHA-256-Fingerabdruck vergleichen. Den angezeigten Gerätenamen im lokalen Netz öffnen. Die Einrichtung benötigt keinen PC. Das Administratorgerät wird zum Erneuern der Zertifikate benötigt.

**Verlust oder Wechsel des Administrators.** Gehen Bediengerät oder App-Daten verloren, das Einrichtungs-WLAN am Lüfter vor Ort öffnen und die Einrichtung mit dem neu gekoppelten Administratorgerät wiederholen. Anschließend dessen Stammzertifikat auf den Bediengeräten installieren.
