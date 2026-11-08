# LeafLink 3.3.12 Beta – Repeaterkorrektur und automatische Funkweiterleitung

Behebt einen Fehler beim manuellen Repeater-Test über die Weboberfläche: Bei Wall-gekoppelten Lüftern konnte der Test versehentlich dauerhaften Direktfunk speichern, nur die Wall als Zentrale suchen und dadurch andere erreichbare Gateways übergehen. Der temporäre Test behält jetzt die gespeicherte WLAN-Auswahl und die Kopplung. Eine fehlende Route oder ausbleibende Gateway-Bestätigungen führen kontrolliert zurück zur gespeicherten Verbindung.

Der Automatikbetrieb kann nun auch bei einer noch bestehenden, aber anhaltend schwachen WLAN-Verbindung über andere Platinen weiterleiten. Der Versuch beginnt nach 30 Sekunden schwachem Signal, wenn ein frisch gemeldetes Gateway deutlich besseren WLAN-Empfang hat. Hysterese und eine Wartezeit nach fehlgeschlagenen Versuchen vermeiden ständige Wechsel. Feste Rollen, Einrichtung und Updates werden berücksichtigt. Eine bestätigte Funkroute bleibt aktiv; die Rückkehr zum eigenen WLAN erfolgt bei Routenverlust, manuell oder nach Neustart.

Die Geräteübersicht meldet eingestellte Betriebsart und tatsächliche Netzwerkrolle getrennt. App 3.3.10 zeigt diese Informationen unter **Gespeicherte Lüfter** an. Das Funkformat bleibt kompatibel; ein zusätzliches Wall-Update ist für diese Lüfterkorrektur nicht erforderlich.

Geprüft: 202 Firmware-Hosttests, 52 native Testprogramme, Protokollvergleich, Hardwarebuild, Signatur-/Stackprüfungen und datenbehaltende Installation auf zwei realen Platinen. Ein realer Repeater-Test übertrug Zustände und Steuerbefehle über eine zweite Platine und bestätigte die Rückkehr ins WLAN. Die Signalauslösung wurde mit simulierten Empfangswerten im Produktionscode geprüft. Ein echter Reichweiten-Dauertest oder erzwungener Mehrhoptest ist damit nicht belegt; einzelne HTTP-Abfragen konnten auslaufen.

Voraussetzung: ESP8266 ESP-12F, 4 MiB Flash, Hardwareprofil und A/B-Layout 2. Einstellungen, Kopplungen und Nutzungszähler bleiben beim normalen Update erhalten. Kein Werksreset.

In **Firmware-Updates** die **Beta-Versionen einschließen**, dann **VERSION PRÜFEN** und **FIRMWARE HERUNTERLADEN** wählen. Anschließend die gewünschten Lüfter über den bestehenden Updateablauf aktualisieren.
