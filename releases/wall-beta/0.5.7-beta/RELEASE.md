# WLAN-Daten mit Wall Control übertragen

Wall Control 0.5.7 und LeafLink 3.2.5 Beta ergänzen die auswählbare Funktion
„WLAN-Daten auch an Lüfter übertragen“. In der Weboberfläche ist die Option
zunächst ausgeschaltet; am Display stehen „Nur Wall Control“, „Auch an Lüfter“
und „Abbrechen“ zur Wahl.

Voraussetzung: unterstützende Firmware auf beiden Seiten und eine bereits mit
individuellem Einrichtungscode authentifiziert eingerichtete private Wall-
Funkbindung. Eine bloße LAN-Erkennung ist keine solche Kopplung. Entfernte Lüfter
werden ausgeschlossen. Ältere oder nicht erreichbare Lüfter werden nicht als
Erfolg gezählt. Die Daten werden verschlüsselt übertragen.

Jeder Lüfter prüft das WLAN bis zu 30 Sekunden und speichert nur nach erfolgreicher
Verbindung. Gruppen und Funkbindung bleiben erhalten. Er bestätigt Verbindung
und Speicherung und startet anschließend nach 15 Sekunden geordnet neu.
Fehler behalten die alten Daten; fehlende Bestätigung wird als unbestätigt
angezeigt, auch wenn der Lüfter bereits gespeichert haben könnte.

Nach allen Versuchen wechselt Wall Control selbst ins eingegebene WLAN, auch
bei Teilerfolg. Fehlgeschlagene Lüfter bleiben bei ihrem bisherigen Netz.
Einzelheiten stehen pro Lüfter in der Weboberfläche; am Display erscheinen
Fortschritt, Summe und die ersten drei Ergebnisse. Die Funktion verteilt keine
Firmware. Der Direktfunk und die private Funkidentität bleiben erhalten.

Diese Beta wurde durch Host-, Produktionsfunktions-, Kryptografie- und
Browsertests sowie Builds geprüft. Die neue WLAN-Übertragung wurde noch nicht
auf physischen Geräten ausgeführt. Die Veröffentlichung installiert nichts
automatisch. Bestehende Daten bleiben beim regulären Update erhalten.

Nach erstmaliger erfolgreicher WLAN-Übertragung nutzt die Lüfterkonfiguration
einen erweiterten authentifizierten Betriebsmodus. Ältere Firmware vor 3.2.5
versteht diesen Modus nicht; ein Rückgang erfordert eine gesonderte Prüfung der
Erreichbarkeit und Funkbindung.

Enthält außerdem die Korrektur aus 0.5.6: Nach erfolgreicher Aufnahme zeigt
die Gruppenansicht nicht mehr „Aufnahme abgebrochen“. Entfernen, Wiederaufnehmen,
endgültiges Löschen entfernter Lüfter und Auflösen von Gruppen sind enthalten.

ESP32 LILYGO T-Display, bestehendes 16-MiB-Layout. App-BIN für den regulären
Firmware-Updateweg, kein Vollflash. Das vorhandene Nextion HMI 302 bleibt
kompatibel; das unveränderte TFT liegt zur Vollständigkeit bei.
