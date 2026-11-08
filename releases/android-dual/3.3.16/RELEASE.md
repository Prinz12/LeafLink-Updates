# LeafLink Android 3.3.16 – Rollenanzeige und Netzwerkeinstellungen

Nach dem Erkennen oder Umgruppieren eines Lüfters fragt die App dessen Master-/Slave-Rolle für 45 Sekunden im Abstand von zwei Sekunden ab. Anschließend gilt wieder das normale Intervall. Auch ein bereits geöffneter Gerätedialog aktualisiert die Rollenanzeige.

Unter **Gerätedetails → Netzwerkrolle ändern** stehen **Automatisch**, **Router** und **Repeater** zur Verfügung. Bei gespeicherten, nur über ein Gateway erreichbaren Lüftern ist die Auswahl auch im Gerätemenü erreichbar. Die App prüft den aktuellen Verbindungsweg und bestätigt einen übermittelten Befehl erst nach Rückmeldung des Zielgeräts. Ein noch laufender Rollenwechsel wird entsprechend angezeigt; über **Aktualisieren** kann der Stand erneut gelesen werden.

**Für dauerhafte Rollenwahl und automatische IN/OUT-Paare ist Firmware 3.3.14 Beta oder neuer erforderlich.** Ältere Firmware erhält einen Updatehinweis. Repeater arbeiten über ein anderes Leaf-Gateway; Router verwenden ausschließlich die direkte WLAN-Verbindung. Die Firmware schützt das letzte erreichbare Gateway vor dem Wechsel zum Repeater.

Die Installationsrichtung bietet **AUTO**, **IN**, **OUT** und **PHYSISCH**. Mit neuer Firmware startet ein bislang nicht manuell konfigurierter Lüfter in Auto mit IN. Ein automatisches Paar wählt einmal IN und einmal OUT; manuelle Einstellungen bleiben erhalten. AUTO aktiviert die Paarzuordnung wieder.

Bei einzelnen verlorenen Antworten auf Hintergrundabfragen erfolgt nun eine begrenzte Wiederholung mit frischer verschlüsselter Anfrage. Schreibbefehle werden nicht automatisch wiederholt. Bleibt eine Leseabfrage erfolglos, benennt die Meldung den betroffenen Bereich; spätere erfolgreiche Abfragen kennzeichnen den entsprechenden Fehler als behoben, ohne das Archiv mit Routineeinträgen zu füllen.

Geprüft auf Samsung SM-S918B: Rollenänderung im simulierten lokalen Gerät nach 1,468 Sekunden angezeigt; 24 Einstellungs-/Dialogprüfungen, 63 Meldungsprüfungen und 108 Firmware-Abschlussprüfungen bestanden. Zusätzlich 28 verschlüsselte Lese-/Wiederholungsprüfungen und 169 Setup-Wiederholungsprüfungen bestanden. Hosttests, Release-/Debug-Build, Lint und Signaturprüfung bestanden. Kein Emulator und kein App-Downloadtest. Es wurden keine realen Lüfter umgruppiert oder umgeschaltet.

Paket `de.prinz.leaflink`, Versionscode 25, unveränderte Signatur. Installation als Update erhält vorhandene App-Daten.
