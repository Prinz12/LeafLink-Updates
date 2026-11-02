# LeafLink 3.2.9 Beta – Start mit älterer Wall-Direktkopplung

Ein Lüfter mit älterer gespeicherter Direktkopplung stellte den Funk wieder her,
kennzeichnete den laufenden Betrieb aber nicht als Direktbetrieb. Damit konnte
die A/B-Startbestätigung trotz funktionierendem Funk ausbleiben. 3.2.9 setzt
diese Kennzeichnung auch im älteren Startpfad.

Die Startprüfung wird nicht gelockert: gültiges Journal, initialisierter Funk,
gesunder Programmlauf, externe Bestätigung und dauerhaftes Speichern bleiben
erforderlich. WLAN-Daten, Gruppen und Kopplung werden nicht gelöscht.

Enthält die gemeinsame Netzauswahl aus 3.2.8 mit Wall Control 0.5.10.
Die Wiederverbindungszeiten wurden in diesem Update nicht verändert.
Signiertes A/B-Anwendungsupdate für 4-MB-ESP8266, Layout 2. Regulärer OTA-Weg
und Rückfall bleiben erhalten. Das passende Hardware-/Safe-Profil verwenden.

Profil: **hardware**.
