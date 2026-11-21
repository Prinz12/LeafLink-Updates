# LeafLink Lüfter-Firmware 4.0.0

Die Browseroberfläche läuft per HTTPS direkt am Lüfter. Gerätestatus und Einstellungen erfordern eine Anmeldung. Über die gekoppelte App lässt sich ein verlorenes Bediengerät sperren. Erreichbare Lüfter wechseln sofort den Netzschlüssel. Ausgeschaltete Lüfter bleiben in der App zur Nachholung sichtbar.

**Vor dem Update von 3.x.** Zuerst die LeafLink-App 4.0.0 installieren. Für die bisherige Browserbedienung benötigt jeder Lüfter ein individuelles Gerätezertifikat. Die Werkstatt richtet es einmal per USB mit der lokalen CA der Installation ein. Auf jedem Bediengerät das öffentliche Stammzertifikat dieser CA als vertrauenswürdig einrichten. Für den Aufruf muss der zertifizierte Gerätename im lokalen Netz auflösbar sein. Ein Update allein richtet das Zertifikat nicht ein.

Diese signierte Firmware ist für LeafLink-Lüfter mit ESP8266, 4 MiB Flash und vorhandenem A/B-Bootlayout 2 bestimmt. Die App prüft das Firmware-Abbild vor der Übertragung. Bei Gateway-Lüftern mit 4.0.0 erfordern spätere direkte Firmware-Updates ein gültiges Gerätezertifikat.

Das zur Firmware gehörende LGPL-Paket steht bei den Downloads dieser Version.
