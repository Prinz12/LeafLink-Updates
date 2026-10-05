# Wall Control 0.5.0 Beta – Direktfunk-Erstaufnahme

Fabrikneue Lüfter lassen sich am Nextion-Touchdisplay oder über die Weboberfläche
hinzufügen: physisches Kopplungsfenster per kurzem Tastendruck öffnen,
Gerätekennung wählen, individuellen Einrichtungscode eingeben und eine
bestehende oder neue Gruppe bestätigen. Das Kopplungsfenster dauert drei Minuten.
Der Code kommt vom Geräteetikett; dessen Fertigungsabruf erfolgt ausdrücklich
über USB/UART. Bestehende Lüfter und ihre Einstellungen bleiben erhalten.

Wall Control überträgt die Funkkonfiguration verschlüsselt und meldet Erfolg
erst nach einer frischen Rückmeldung des richtigen Geräts im Direktfunknetz.
Der Lüfter speichert die Konfiguration verschlüsselt und authentifiziert.
Unterbrochene Aufnahmen werden nach einem Neustart erneut geprüft. Der
anschließende Betrieb benötigt kein Heim-WLAN und keinen dauerhaften Access Point.

Für LILYGO T-Display mit ESP32 und 16 MiB Flash sowie Nextion NX4827K043_011.
**HMI 302 bleibt unverändert; für die neue Bedienung genügt das ESP32-Update.**
Die ESP32-Datei wird auf Modell, Größe und SHA-256 geprüft; eine
Herausgebersignatur ist bei Wall Control weiterhin nicht implementiert.

**Beta-Grenze:** Der komplette Aufnahmeablauf wurde noch nicht mit einem
fabrikneuen realen Lüfter Ende zu Ende geprüft. Die fünf vorhandenen,
eingerichteten Geräte werden dafür nicht zurückgesetzt. Passende LeafLink-
Firmware 3.2.2 Beta auf dem Lüfter ist erforderlich; Originalhersteller-Firmware
unterstützt den neuen Kopplungsweg nicht.

Lüfter-OTA über reinen Direktfunk ist nicht enthalten. Lüfter-Updates benötigen
WLAN oder den dokumentierten kabelgebundenen Serviceweg. Der Service-AP des
Displays ist zeitlich begrenzt und ermöglicht dessen eigene Web-/Dateiupdates.

Geprüft auf LILYGO und Nextion: Firmware 0.5.0, HMI 302, Kryptografie-Selbsttest, echter Aufnahme-Assistent und Abbruch, Sperre konkurrierender Netzänderungen, fünf vorhandene Lüfter weiterhin erreichbar, gespeicherte Gruppen und Einstellungen erhalten. Controller 43, Aufnahme 37, Funkwurzel 10 und Routing 7 Prüfungen bestanden. Die vollständige Erstaufnahme eines fabrikneuen Lüfters steht noch aus.
