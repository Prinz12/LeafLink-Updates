# LeafLink Android 3.3.17

Gruppennamen erscheinen auch in Firmware-Updates, Fortschrittsanzeigen, Berichten und Meldungen. Die internen Gerätezuordnungen bleiben unverändert.

- AUTO, IN, OUT und PHYSISCH bleiben in einer Reihe und haben dieselbe Höhe.
- „Raum zuordnen“ steht direkt unter dem Raum, „Gruppe ändern“ direkt unter der Lüftungsgruppe.
- Die wirksame Richtung im offenen Gerätedialog wird regelmäßig neu gelesen.
- Nach dem Netzwerkrollenwechsel liest die App automatisch weiter, auch über ein neues Gateway. Bleibt die Bestätigung aus, erscheint ein konkreter Hinweis statt einer endlosen Fortschrittsmeldung.

Für den Betrieb eines WLAN-Repeaters ohne eingeschaltete Wall zusätzlich Lüfterfirmware 3.3.16 Beta installieren. Wall 0.6.5 Beta übernimmt Gruppennamen aus dem synchronisierten Hausplan.

Firmwareupdates erreichen Repeater jetzt über das Lüfter-Gateway. Die App prüft das konkrete Zielgerät, überträgt die signierte Firmware in bestätigten Blöcken und kontrolliert anschließend Neustart, A/B-Slot, Einstellungen und Hausplan. Am Repeater ist keine direkte Routerverbindung erforderlich. Dafür muss die neue Empfangsfunktion ab Firmware 3.3.16 einmalig über USB oder direktes WLAN installiert sein.

Datenerhaltendes Update für Android ab 6.0, Paket de.prinz.leaflink, Versionscode 26, unveränderte Signatur. Bedienoberfläche auf einem Samsung SM-S918B geprüft; Funkupdates anschließend vom Android-Emulator über zwei echte Lüfter getestet. Kein App-Downloadtest.

Repeater-Erkennung: Bei mDNS-Ankündigungen über ein Gateway wird die eigene Adresse des Repeaters gezielt auf seine tatsächliche Geräteidentität geprüft. Für vollständige Repeater-Statusantworten Firmware 3.3.16 verwenden.

Zwei vollständige Updates im Repeaterbetrieb bei ausgeschalteter Wall bestanden: 5:43 Minuten im normalen Versuch und 7:19 Minuten mit 72 absichtlich verworfenen Antworten. Beide einschließlich Neustart und bestätigtem Firmware-Slot, mit erhaltenen Einstellungen und Hausplan. Die Dauer hängt von der Funkstrecke ab.
