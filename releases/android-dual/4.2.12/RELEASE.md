# LeafLink Android 4.2.12

Die App aktualisiert ältere RTOS-Firmware über gekoppeltes, verschlüsseltes UDP. Auf einem bestätigten RTOS-Gateway mit der korrigierten Firmware verwendet sie bei direkter WLAN-Verbindung bevorzugt HTTPS. Über andere Lüfter laufen Firmware-Updates weiter über verschlüsseltes UDP. Der verifizierte Teststand 4.2.57 unterstützt den regulären Wechsel auf 4.2.58.

Der HTTPS-Upload wartet auf die Empfangsbereitschaft des Lüfters. Nach jedem Update prüft die App den bestätigten Start, das Firmware-Image, die Einstellungen und den Hausplan.

Die App hat die Paketkennung de.prinz.leaflink und den Versionscode 107. Die normale Updateinstallation übernimmt die bestehenden App-Daten.
