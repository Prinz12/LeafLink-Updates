# LeafLink 3.3.36 Beta – Lebensdauerstatistik über Repeater

Behebt gemeinsam mit App 3.3.42 den fehlenden Abruf unter „Lebensdauer & Nutzung“
bei Repeatern. Die Firmware überträgt die aktuellen Zähler über die vorhandene
verschlüsselte LeafLink-Verbindung. Die Zähler liefen bisher bereits weiter;
der direkte HTTP-Abruf der App war im Repeaterbetrieb nicht erreichbar.

Zuerst App 3.3.42 aktualisieren, anschließend die betroffenen Repeater auf
Firmware 3.3.36. Ein reines Gateway-Update reicht für diese Korrektur nicht.
Bei automatischer Rollenwahl empfiehlt sich derselbe Stand auf allen Lüftern.
Ältere direkt per WLAN erreichbare Firmware bleibt über ihren bisherigen
Statistikabruf lesbar. Gespeicherte Zähler, Kopplungen, Einstellungen und
Hausplan werden durch diese Korrektur nicht zurückgesetzt.

Signiertes Hardware-Anwendungsupdate für ESP8266 mit 4 MiB und A/B-Layout 2.
Die bisherigen Repeater-OTA-Verbesserungen sind enthalten. Bei sehr alter
Repeaterfirmware mit Speichermangel kann die Erstaktualisierung weiterhin
einmalig Routerbetrieb erfordern.

205 Firmware-Hosttests, 73 native Regressionstests, Protokollvergleich,
Hardwarebuild und Stackprüfung bestanden. Android-Build, Lint, Hosttests und
Emulatorprüfung bestanden, einschließlich des echten Firmware-Antwortformats.
Die neue Statistikabfrage wurde noch nicht an einem physischen Repeater geprüft.
