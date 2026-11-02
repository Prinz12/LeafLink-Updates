# Wall Control 0.5.9 Beta – Upload-Abbruch und gespeichertes WLAN

Behebt eine blockierte Bedienung nach unterbrochenem Firmware-Upload:
Der Upload wartet maximal 15 Sekunden auf weitere Daten. Danach wird der
Empfang abgebrochen und die Bedienung wieder freigegeben. Ein verwaister
Empfangszustand wird zusätzlich nach 20 Sekunden aufgeräumt. Unvollständige
Dateien werden nicht installiert; bestehende Firmware und Einstellungen bleiben.

Neue Aktion „Gespeichertes WLAN an Lüfter übertragen“ in der Weboberfläche
unter „WLAN und Leaf-Funknetz“. Das Kennwort muss nicht erneut eingegeben
werden und wird nicht an den Browser übertragen.

Am Display: Einstellungen → WLAN → WLAN an Lüfter → Jetzt übertragen.
Das Display nennt vor der Bestätigung die gespeicherte SSID.

Die Aktion nutzt ausschließlich die bereits in Wall Control gespeicherten
Zugangsdaten. Wall Control wird dabei weder neu verbunden noch umkonfiguriert.
Die bisherige Einrichtung eines neuen WLANs mit optionaler Weitergabe bleibt
unter „WLAN einrichten“ verfügbar.

Voraussetzung: eingerichtetes WLAN in Wall Control, bereits authentifiziert
gekoppelte und erreichbare Lüfter, empfohlen LeafLink 3.2.6 Beta. Die
Übertragung läuft verschlüsselt nacheinander. Jeder Lüfter prüft das WLAN
vor dem Speichern. „WLAN geprüft und gespeichert“ bestätigt den Erfolg;
fehlende Antworten und Teilerfolge bleiben sichtbar. Entfernte Lüfter
werden nicht einbezogen. Gruppen und private Funkbindung bleiben erhalten.

Produktionsfunktions- und Displaytests, Desktop-/Mobil-Browsertest sowie
Live-/Read-only-Builds geprüft. Ein tatsächlicher WLAN-Wechsel auf den
physischen Lüftern wurde nicht durchgeführt.

ESP32 LILYGO T-Display, bestehendes 16-MiB-Layout. App-BIN für den regulären
Updateweg, kein Vollflash. Nextion HMI 302 bleibt unverändert kompatibel;
kein TFT-Update erforderlich.
