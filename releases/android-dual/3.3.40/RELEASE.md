# LeafLink Android 3.3.40 – Weniger OTA-Funkfragmente

Das adaptive Repeater-Update verwendet 592 statt 640 Nutzbytes pro Block.
Dadurch passen die geschützten Daten in vier statt fünf Funkfragmente. Die
Taktung berücksichtigt Antwortstreuung; nach einer Rücknahme wächst das Fenster
erst nach 24 sauberen Blöcken wieder. Maximal zwei ausstehende Blöcke bleiben
erlaubt. Signatur-, Geräte-, Start- und Datenerhaltprüfungen bleiben aktiv.

Am Repeater 1255 wurde dasselbe signierte Image über denselben direkten
Gateway 6469 geprüft: bisher 292,031 Sekunden und 137 Wiederholungen, mit
App 3.3.40 und Gateway-Firmware 3.3.34 nun 261,423 Sekunden und 97 Wiederholungen.
Das sind 29,2 % weniger Wiederholungen bei 10,5 % kürzerer Übertragung.
Imagehash, bestätigter A/B-Start, Repeaterrolle, Einstellungen und Hausplan
wurden geprüft. Das ist ein Gerätevergleich unter wechselnden Funkbedingungen,
kein Langzeitnachweis und keine Aufteilung des Gewinns auf einzelne Änderungen.

Für das gemessene Ergebnis müssen die verwendeten Gateways Firmware 3.3.34
haben. Der Repeater benötigt für das Fenster mindestens 3.3.33; ältere Firmware
verwendet unverändert das bisherige Ein-Block-Verfahren. App-Update ohne
Deinstallation installieren; Kopplungen und Einstellungen bleiben erhalten.
