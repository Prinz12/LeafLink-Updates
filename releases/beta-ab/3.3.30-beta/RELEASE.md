# LeafLink 3.3.30 Beta – saubere Übergabe zwischen Gateways

Nach einem Gatewaywechsel gibt das alte Gateway die Repeater-Adresse frei,
sobald ein gültiger Beacon oder eine angenommene Bestandsmeldung den neuen
Gateway nennt. Es beendet auch ausstehende Wiederholungen für dieses Gerät.
Bisher konnte es die Adresse noch bis zu 45 Sekunden beanspruchen und so
Anfragen zum falschen Gateway lenken. Andere Repeater bleiben unverändert.

Enthält die adaptive Gatewaywahl und Transportkorrekturen aus 3.3.29.
Für diese Übergabekorrektur müssen die als Gateways betriebenen Lüfter
aktualisiert werden. Repeater können auf 3.3.29 bleiben; Geräte, die später
Gateway werden sollen, sollten ebenfalls aktualisiert werden.

Signiertes Hardware-Anwendungsupdate für ESP8266, 4 MiB, A/B-Layout 2.
Einstellungen, Räume, Kopplungen und Hausplan bleiben erhalten.
