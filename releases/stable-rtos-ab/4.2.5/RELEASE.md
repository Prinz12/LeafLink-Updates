# LeafLink RTOS-Flottenfirmware 4.2.5

Bei einem Repeater-Update hält der Lüfter Gateway, direkten Funknachbarn und Funkkanal für die Übertragung fest. Bei längerem Funkverlust beendet er die Updatesitzung. Der bestätigte Firmwarestand bleibt aktiv.

Die automatische Netzwerkwahl berücksichtigt Paketverluste und Antwortzeiten, wenn das Gateway die neue Messung unterstützt. Der Lüfter testet in diesem Fall den alternativen ESP-NOW-Pfad und übernimmt ihn bei besserer gemessener Qualität.

Die Firmware kann komprimierte Repeater-Updates empfangen. LeafLink für Android 4.2.5 nutzt LZ4, sobald der Lüfter die Unterstützung meldet. Ältere Firmware lässt sich über den bisherigen Übertragungsweg aktualisieren.

Das signierte Flottenpaket ist für kompatible LeafLink-Lüfter mit ESP8266, 4 MiB Flash und A/B-Layout 2 vorgesehen. Die App prüft den Ausgangsstand, das Hardwareprofil und die Signatur. Je nach Ausgangsstand kann ein Zwischenupdate erforderlich sein.

In LeafLink **Firmware-Updates** öffnen, **Version prüfen** und **Geräte prüfen** wählen. Nach dem Neustart zeigt die App den bestätigten Firmwarestand an.
