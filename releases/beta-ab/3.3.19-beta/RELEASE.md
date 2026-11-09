# LeafLink 3.3.19 Beta – Anmeldung bei fragmentiertem Speicher und Sommermesswerte

- Die laufende verschlüsselte Kommunikation verwendet einen fest reservierten Kryptografie-Arbeitsbereich. Eine Anmeldung scheitert dadurch nicht mehr an der bisherigen Anforderung eines freien zusammenhängenden 6-KB-Blocks. Auch die Web-Anmeldung nutzt diesen Bereich.
- Stackgrenzen werden beim Build geprüft; Höchstverbrauch und abgewiesene Kryptografieaufrufe erscheinen in der Gerätediagnose. Bestehende Last-, Zeit- und Sicherheitsgrenzen bleiben wirksam.
- Jeder Lüfter liefert seine eigenen Innen-/Außentemperaturen der Sommerautomatik an die Gruppenseite von Android 3.3.21. Fehlende und veraltete Werte werden getrennt gekennzeichnet.

Alle beteiligten Lüfter aktualisieren. **Android 3.3.21** ergänzt die Anzeige; **Wall 0.6.6 Beta** bleibt kompatibel. Die Sommerautomatik läuft weiterhin in der Firmware.

204 Hosttests, 62 native Regressionstestprogramme, unabhängige Kryptografieprüfungen und Hardwarebuild mit Stackaudit bestanden. Ein realer Lüfter bestand einen zehnminütigen gemischten Netzwerklasttest ohne beobachteten Neustart oder Motorfehler. Parallel gelangen 188 vollständige authentifizierte Abfragerunden vom Handy ohne Fehler. Das ist ein begrenzter Belastungsnachweis, keine Garantie für jede Betriebsbedingung oder einen mehrtägigen Dauerbetrieb. Geplante Update-/Wartungsneustarts bleiben erhalten.

Signiertes A/B-Update für Hardwaregeräte mit Layout 2; Einstellungen bleiben erhalten. Dieselbe Firmware für Router und Repeater. Die neuen Laufzeittests erfolgten im Routerbetrieb; ein erneuter realer Repeater-Dauerlauf steht aus. Die Veröffentlichung installiert keine weiteren Geräte automatisch.
