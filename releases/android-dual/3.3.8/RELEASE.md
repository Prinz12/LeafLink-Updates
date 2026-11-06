# LeafLink Android 3.3.8 – Statistik für jeden gespeicherten Lüfter

**Einstellungen → Gespeicherte Lüfter → Lebensdauer & Nutzung** öffnet unter
jedem Lüfter ein getrenntes Menü. Offline bleibt der letzte gespeicherte Abruf
mit einem Hinweis sichtbar; fehlende Daten werden nicht als Nullwerte dargestellt.

Die Erfassung beginnt mit der Installation der Firmware 3.3.8. Vorhandene
Kopplungen, WLAN-Daten, Hausplan und Einstellungen bleiben bei normalen Updates erhalten.
App und Lüfterfirmware werden getrennt aktualisiert.

Die Statistik unterscheidet Motoransteuerung, Stillstand und unbekannten Motorzustand
bei vorhandener Stromversorgung. Eine Ansteuerung beweist keine tatsächliche Rotation.
Zusätzlich werden lange Stillstände, Stillstand ab 70 % Luftfeuchte und Neustarts erfasst.
Stromlose Zeiten sind ausdrücklich als nachträgliche Netzzeit-Schätzung gekennzeichnet.
Auch Bootloader- und Updatezeiten können in diesen Beobachtungslücken enthalten sein.
Ohne gültige Zeit bleibt die Lücke ungeklärt. Frühere Laufzeiten werden nicht nachgetragen.

Die Zähler bleiben bei normalen Firmwareupdates, Filterreset und Werkseinstellungen
erhalten. Es gibt keine Rücksetzfunktion. Checkpoints erfolgen alle fünf Minuten und
vor regulären Neustarts/Updates. Ein plötzlicher Stromausfall kann den noch nicht
gespeicherten Abschnitt verlieren. Vollständiges Flashlöschen oder fremde Firmware
können die Daten weiterhin verändern; kein manipulationssicherer Beweiszähler.

Der aktive Safe-Profilpfad wurde entfernt. Aktuelle Updates sind ausschließlich
für echte Hardware. Signaturprüfung, Motorschutz und A/B-Rückfall bleiben aktiv.
