# LeafLink RTOS 4.2.63

Verliert ein laufendes Lüfterpaar den direkten Taktfunk, kann ein auf demselben Funkkanal erreichbarer dritter Lüfter den Partnertakt vermitteln. Dafür benötigen beide Partner und der vermittelnde Lüfter die neue Funktion. Sobald der Direktfunk mindestens 15 Sekunden stabil war, schaltet der jeweilige Partner mit der nächsten gültigen Taktmeldung zurück. Bei gewöhnlichen WLAN-Gruppen ist nach einem Neustart zunächst direkter Kontakt zwischen den Partnern erforderlich.

Das signierte Flottenupdate ist für kompatible ESP8266-Lüfter mit 4 MiB Flash und A/B-Layout 2 bestimmt. In LeafLink unter **Firmware-Updates → Version prüfen** das Paket laden und **Geräte prüfen** wählen.

**Wartungszähler beim Update:** Die Firmware sichert Filter- und Großwartungslaufzeit alle sechs Motorstunden. Bei einem Neustart kann der seit der letzten Sicherung aufgelaufene Anteil verloren gehen. Wer diese Werte für die Wartung dokumentiert, sollte sie vor dem Update ablesen. Im Gerätetest blieben WLAN, Paarungen, Hausplan und Wartungsintervalle erhalten.
