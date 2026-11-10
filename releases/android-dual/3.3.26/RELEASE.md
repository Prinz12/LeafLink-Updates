# LeafLink Android 3.3.26 – Gerätesuche über VPN

Die App lädt bei der Suche mehrere Geräteübersichten nach. Eine erfolgreiche,
aber unvollständige erste Übersicht beendet die Suche nicht mehr. Zuletzt
antwortende Geräte werden bevorzugt, die Quellen wechseln zwischen Suchläufen.
Neue IP-Adressen werden weiterhin durch eigene Geräteantworten bestätigt.

Die vorhandenen Begrenzungen, Kopplungen, Löschentscheidungen und die Erkennung
nicht erreichbarer Geräte bleiben erhalten. Die adaptive Sommermessung aus
3.3.25 bleibt enthalten.

Eine doppelte IP-Zuordnung von VPN-Handy und Lüfter muss im Router behoben werden.
Diese App-Version garantiert keine Behebung eines solchen Adresskonflikts.
Für den Fernneustart ohne Tastendruck am Lüfter ist Firmware 3.3.23 Beta nötig.

Prüfung: Android-Hosttests, Release-Build und Lint, 65 Discovery-Prüfungen im
Emulator, Signatur und Release-Dateien. Installation durch den Nutzer;
keine Installation auf dem Handy und kein VPN-Praxistest dieses Builds.

Paket de.prinz.leaflink, Versionscode 35, Android 6.0 oder neuer. Update über
die vorhandene App; App-Daten bleiben erhalten.
