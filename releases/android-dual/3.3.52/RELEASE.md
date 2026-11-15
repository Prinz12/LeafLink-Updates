# LeafLink Android 3.3.52 – Richtiger Updateweg für Gateways und Repeater

Behebt den vorzeitigen Updateabbruch „Repeater nicht bereit für das Update“,
wenn ein direkt erreichbarer Gateway fälschlich über den Repeaterweg behandelt
wurde. Die App wählt den Updateweg anhand der aktuellen Geräteantwort und
prüft die Netzrolle vor der Vorbereitung erneut.

- Gateways verwenden den direkten WLAN-Updateweg, Repeater den Mesh-Weg.
- Veraltete Repeater-Hinweise und kurzzeitig fehlgeschlagene HTTP-Abfragen
  führen nicht mehr zur falschen Zuordnung eines Gateways.
- Geräteidentität und bestehende Kopplung werden beim Wechsel geprüft.
- Nach erfolgreicher Vorbereitung bleibt der Weg für diesen Upload fest;
  unklare Übertragungen werden nicht automatisch erneut gestartet.

Die Korrektur wurde im Emulator und mit einem erfolgreichen Gateway-Update
auf Firmware 3.3.49 Beta geprüft. Einstellungen und Hausplan blieben erhalten.
Diese Veröffentlichung enthält nur die Android-App; die Lüfterfirmware bleibt
unverändert. Bestehende Kopplungen und App-Daten bleiben beim App-Update erhalten.

Android 9 oder neuer (minSdk 28), targetSdk Android 16 (36), Versioncode 62.
Als Update ohne Deinstallation installieren.
