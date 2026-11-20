# LeafLink Android 3.3.62 – Doppelte Updateeinträge korrigiert

Die Firmware-Updateliste verwendet die dauerhafte Gerätekennung zur Zuordnung. Nach einem IP-Wechsel erscheint ein bekannter Lüfter einmal statt zusätzlich unter seiner alten Adresse als nicht erreichbar. Die erwartete Gerätekennung wird beim Wiederfinden geprüft. Verschiedene Geräte mit gleicher vierstelliger Lüfternummer bleiben getrennt.

Offene Updateversuche, Übertragungsnachweise und gespeicherte Einstellungen bleiben erhalten. Eine bestätigte neue Adresse ersetzt die alte Route auch im Updateprotokoll, ohne einen erneuten Upload auszulösen. Tatsächlich unerreichbare Geräte bleiben als Fehler sichtbar.

Als Update über die vorhandene App installieren, nicht deinstallieren. Kein Firmware- oder Wall-Update für diese Korrektur erforderlich. Die Sommerfunktionen aus App 3.3.61 bleiben enthalten.

Release-Build, Lint, Android-Hosttests und Emulatorprüfungen bestanden. Geprüft wurden Adresswechsel, alte und neue Routen in beiden Reihenfolgen, Offline-Rückkehr, fremde Geräte an alten IPs, gleiche Lüfternummern, offene Updateprotokolle und die tatsächliche Updateansicht. Keine Installation auf Nutzergeräten.

Prüfgrenze: Ein zusätzlich ausgeführter historischer 2.0.0-Migrationstest ist wegen einer nicht passenden Signatur seiner lokalen Testdatei blockiert; das historische Release ist im aktuellen Kanal nicht vorhanden. Der Signaturschutz und die Migration bleiben unverändert. Die aktuellen Update-, DHCP- und Abschlussprüfungen bestehen.
