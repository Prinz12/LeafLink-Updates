# LeafLink 3.3.59 Beta

Lüfter können den Teststart einer neuen Firmware über eine bestehende Mesh-Kopplung bestätigen. Ein Repeater beantwortet dafür die geschützte Statusabfrage der App. Bei automatischer Rollenwahl versucht der Lüfter zuerst das Router-WLAN. Scheitert dieser Start, kann er den vorhandenen Mesh-Weg mit seiner gespeicherten Adresse verwenden.

Die Startprüfung und die zweiminütige Rückfallfrist bleiben aktiv. Der Slotwechsel und die Bestätigung über Mesh wurden auf einem Lüfter mit der Rolle „Nur Repeater“ geprüft.

Das signierte Paket ist für ESP8266-Lüfter mit 4 MiB Flash und A/B-Layout 2 bestimmt. In LeafLink unter **Firmwareupdate** die Option **Beta-Versionen anzeigen** aktivieren und **Version prüfen** wählen.
