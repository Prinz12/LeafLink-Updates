# LeafLink 3.3.21 Beta – Service und einstellbare Sommerautomatik

- Alle erfolgreich angesteuerten Motorbewegungen zählen zur Wartung, auch kurze Messimpulse, Richtungswechsel und Service-Testläufe. Stillstandszeiten zählen nicht; Teilsekunden bleiben zwischen Bewegungen erhalten.
- Service 1 nach standardmäßig 4320 Motorstunden. Service 2 für die große Reinigung nach drei Intervallen, standardmäßig 12960 Motorstunden (ca. 18 Monate Dauerbetrieb). Frühes Quittieren von Service 1 verschiebt Service 2 nicht.
- Fälligen Service mit mindestens 1,5 Sekunden Tastendruck und anschließendem Loslassen quittieren. Bei Service 2 werden beide Wartungszähler zurückgesetzt. Die Service-LED leuchtet dauerhaft statt zu pulsieren. Setup, Kopplung und Werksreset behalten ihre bisherigen Gesten.
- Vorwarnung standardmäßig 168 Motorstunden vor dem nächsten Service. App und Weboberfläche unterscheiden Service 1 und Service 2; die bisherige Fernquittierung bleibt verfügbar.
- Sommer Auto lässt sich mit Android 3.3.23 unter Gruppeneinstellungen → Sommerautomatik anpassen: Wunschtemperatur, Messdauer je Richtung, Messintervall, nötiger Kühlvorteil der Außenluft und maximale Messleistung. Die Einstellungen werden auf jedem erreichbaren Gruppenmitglied gespeichert und bestätigt.

**Installation:** Zuerst Android 3.3.23 installieren, dann Beta-Versionen in der Firmwareauswahl anzeigen und alle an Sommer Auto beteiligten Lüfter aktualisieren. Mindestens zwei kompatible Lüfter mit gleichen Einstellungen sind nötig. Alte oder unterschiedlich konfigurierte Gruppenmitglieder verhindern die automatische Kühlung. Die Gruppenleistung begrenzt weiterhin Mess- und Kühlleistung. Wall 0.6.6 Beta bleibt für die Modusauswahl kompatibel.

Signiertes Hardware-A/B-Update für ESP8266 mit vorhandenem Layout 2. Einstellungen bleiben erhalten. Vorhandene Filterstunden werden als Ausgangspunkt für Service 2 übernommen; bereits vor dem Update quittierte Wartungszyklen sind nicht rekonstruierbar. Die Zählung erfasst Motorbefehle, keine mechanisch bestätigte Drehung. Bei Stromausfall oder Neustart kann die seit dem letzten Speicherpunkt aufgelaufene Zeit fehlen (standardmäßig bis etwa sechs Motorstunden).

204 Firmware-Hosttests, 64 native Regressionstestprogramme, Herstellerprofil- und Protokolltests, Hardwarebuild und Stackprüfung bestanden. Android-Hosttests, Build, Lint und Emulatorprüfungen bestanden. Die Veröffentlichung aktualisiert keine Geräte automatisch. Bedienung am realen Lüfter und thermisches Verhalten im Haus sind für diesen Stand noch nicht praktisch erprobt.
