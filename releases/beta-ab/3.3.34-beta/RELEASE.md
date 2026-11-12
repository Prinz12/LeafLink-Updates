# LeafLink 3.3.34 Beta – Geordnete Gateway-Übertragung

Die Gateway-Eingangsqueue arbeitet jetzt strikt in Ankunftsreihenfolge. Ein
neueres Paket kann einen älteren, auf Funkkapazität wartenden Eintrag nicht mehr
überholen. Der Replay-Schutz bleibt unverändert. Die zwei vorhandenen Paketpuffer
bleiben erhalten; hinzu kommen lediglich zwei kleine Queue-Indizes.

Am Repeater 1255 wurde dasselbe signierte Image über denselben direkten
Gateway 6469 geprüft: bisher 292,031 Sekunden und 137 Wiederholungen, mit
App 3.3.40 und Gateway-Firmware 3.3.34 nun 261,423 Sekunden und 97 Wiederholungen.
Das sind 29,2 % weniger Wiederholungen bei 10,5 % kürzerer Übertragung.
Imagehash, bestätigter A/B-Start, Repeaterrolle, Einstellungen und Hausplan
wurden geprüft. Das ist ein Gerätevergleich unter wechselnden Funkbedingungen,
kein Langzeitnachweis und keine Aufteilung des Gewinns auf einzelne Änderungen.

Gateways 9857 und 6469 wurden erfolgreich mit bestätigtem Start und erhaltenen
Einstellungen/Hausplan aktualisiert. 1255 blieb für den Vergleich auf 3.3.33.
Für die Kombination App 3.3.40 und die tatsächlich verwendeten Gateways auf
3.3.34 aktualisieren. Bei wechselnden Gatewayrollen auch die übrigen Lüfter
auf denselben Firmwarestand bringen. Signiertes Hardware-Anwendungsupdate
für ESP8266, 4 MiB, A/B-Layout 2; kein Zurücksetzen erforderlich.
