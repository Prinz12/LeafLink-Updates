# LeafLink 3.3.54 Beta – Gruppentakt bei WLAN-Ausfall

Lüftergruppen führen ihren gemeinsamen Takt während kurzer WLAN-Such- und
Verbindungslücken lokal weiter. Die automatische Rückkehr ins WLAN bleibt erhalten.

- Asynchrone WLAN-Suche mit begrenzter Wartezeit statt blockierender Netzsuche.
- Pro Versuch höchstens vier Sekunden Verbindungsaufbau zu einem gefundenen
  Zugangspunkt; zwischen den Versuchen wird der direkte Gruppenfunk fortgesetzt.
- Zusätzliche Zeitangabe im Gruppenstatus: Verspätete Statuspakete starten den
  Zehnsekundentakt nicht mehr fälschlich neu.
- Sofortiger Statusabgleich nach Rückkehr in den Gruppenfunk.
- WLAN-ausgewählte Gruppen mit optionaler Wall-Control-Bindung haben Vorrang vor
  der getrennten Wall-Suche und deren Wiederherstellungsneustart. Explizit
  gewählte Wall-Funk- und feste Gateway-/Repeaterrollen bleiben erhalten.

Für den vollständigen Nutzen alle Lüfter einer Gruppe aktualisieren. Alte
Firmware bleibt protokollkompatibel. Direkte Funkreichweite, gespeicherte
Gruppenpartner und passende Funkschlüssel bleiben erforderlich. Bei dauerhafter
Funktrennung kann keine fortlaufende Gruppensynchronisation garantiert werden.

208 Host-Tests, 83 native Testprogramme, Protokollvergleich mit Android,
Firmware-Builds und Stack-/SDK-Prüfungen bestanden. Die Taktprüfung umfasst acht
simulierte Stunden mit wiederholten Funklücken und Uhrenabweichung. Android-Build,
Lint, Hosttests und Emulatorprüfungen des Updatewegs wurden ebenfalls ausgeführt.
Ein realer WLAN-Abschalt-/Wiederkehrtest auf mehreren Lüftern steht noch aus.

Signiertes Firmware-Update für ESP8266-Hardware mit 4 MiB Flash und bestehendem
A/B-Layout 2. Einstellungen, Kopplungen und Hausplan bleiben erhalten. In der App
Beta-Firmwareupdates aktivieren. Diese Veröffentlichung installiert keine Geräte.
