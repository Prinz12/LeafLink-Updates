# LeafLink Android 3.3.61 – Sommermessung in Stunden

Die adaptive Sommermessung bleibt für beide Luftrichtungen erhalten und darf je Messrunde bis zu 250 Sekunden dauern. Bei stabiler Temperatur endet sie früher; ohne Stabilität gibt es keine neue Kühlfreigabe. Die feste Messdauer bleibt unverändert.

Das Intervall zwischen vollständigen Messzyklen ist in ganzen Stunden von 1 bis 12 einstellbar, Standard 1 Stunde. Es zählt ab Messende bzw. Abbruch. Alte Sekundenintervalle werden auf eine Stunde umgestellt; die übrigen Einstellungen bleiben erhalten.

Während der Kühlung laufen die Sensorabfragen weiter. Die aktuelle Außenluft am Zuluftlüfter wird mit der aktuellen Raumluft am Abluftlüfter verglichen. Erreichte Wunschtemperatur, fehlender Kühlvorteil, Sensorfehler oder veraltete Werte stoppen die Kühlung. Stundenintervalle machen alte Messwerte nicht länger gültig.

Für diese Sommerfunktion müssen alle Gruppenlüfter Firmware 3.3.61 Beta verwenden. Gemischte alte/neue Sommergruppen pausieren. Die Bedienung erfolgt mit App 3.3.61 oder Wall 0.6.10 und über die Lüfter-Webseiten. Die vorhandenen Kopplungen, Räume und WLAN-Einstellungen bleiben erhalten. App als Update installieren, nicht deinstallieren. Das Nextion-HMI bleibt bei 302; kein Displayupdate notwendig.

Firmware-, Protokoll-, Android-, Wall- und Browserprüfungen bestanden, einschließlich Stundenintervalle, Migration, 250-s-Abbruch und frische Messwerte bei mehrstündiger Kühlung. Emulatorprüfung der App-Bedienung bestanden. Kein physischer Lüftertest dieses Builds und keine Installation auf Nutzergeräten. Temperaturstabilität beweist keine vollständige thermische Angleichung des Speichers.
