# LeafLink 3.3.18 Beta – Sommerautomatik

- Neuer eigener Modus **Sommerautomatik**, vollständig in der Lüfter-Firmware. App und Wall müssen für den laufenden Betrieb nicht eingeschaltet bleiben.
- Phase A fördert Innenluft nach draußen und misst innen; Phase B fördert Außenluft nach innen und misst außen. Zwei Messhälften von jeweils 30 Sekunden werden beim Start und anschließend alle fünf Minuten durchgeführt.
- Innerhalb der bestehenden Gruppe wird die kühlere geeignete Zuluftseite gewählt, der Partner führt Luft ab. Dauerhafte Kühlung startet oberhalb 23 °C innen bei mindestens 2 °C kühlerer Außenluft und endet beim Erreichen des Innenziels oder unter 0,5 °C Vorteil. Die kurzen Messläufe können auch wärmere Außenluft ansaugen.
- Temperaturhysterese, frische Messwerte und begrenzte Steuerfreigaben vermeiden häufiges Umschalten und stoppen bei fehlenden Daten oder Verbindung. Ausschalten, Nacht- und Servicebetrieb haben Vorrang.

Alle beteiligten Lüfter auf **3.3.18 Beta** aktualisieren. Auswahl über **Android 3.3.20**, die integrierte Weboberfläche oder **Wall Control 0.6.6 Beta**. Mindestens zwei kompatible Lüfter in derselben Gruppe erforderlich; keine automatische Auswahl über getrennte Gruppen hinweg.

Signiertes A/B-Update für bestehende Layout-2-Geräte; Einstellungen bleiben erhalten. Dieselbe Firmware unterstützt Router und Repeater. Für Updates über Repeater muss dessen Empfänger ab 3.3.16 bereits installiert sein.

Firmware-Host-/Native-Tests, Protokoll-Interoperabilität, Hardwarebuild mit Stackprüfung sowie App-/Wall- und Browserprüfungen bestanden. Thermische Messgüte und Kühlverhalten im realen Haus sind noch nicht praktisch erprobt. Mit dieser Veröffentlichung wird kein Gerät automatisch aktualisiert.
