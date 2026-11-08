# LeafLink 3.3.14 Beta – Gespeicherte Netzwerkrollen und automatische IN/OUT-Paare

**Automatisch**, **Router** und **Repeater** lassen sich über die Gerätewebseite und Android-App 3.3.16 wählen. Die Auswahl wird dauerhaft gespeichert und nach Neustarts wiederhergestellt. Einstellungen und bestehende WLAN-/Wall-Zugangsdaten bleiben beim normalen Update erhalten.

- **Automatisch:** wählt den Verbindungsweg abhängig von der Erreichbarkeit. Automatische Ausweichwege bleiben vorübergehend.
- **Router:** ausschließlich direkte WLAN-Verbindung, kein Repeater-Fallback.
- **Repeater:** Verbindung und Bedienung über ein anderes Leaf-Gateway. Bei Gateway-Ausfall sucht der Lüfter erneut, ohne die gewählte Rolle zu verlieren. Wechsel zurück zu Auto oder Router erfolgt über einen kontrollierten Neustart.

Das letzte erreichbare WLAN-Gateway kann nicht auf Repeater umgestellt werden. Ein Repeater ist kein allgemeiner WLAN- oder Internetverstärker. Bei reiner Wall-Funkkopplung muss für Routerbetrieb zuerst eine WLAN-Verbindung eingerichtet sein. Alte, bislang nur temporär gewählte Rollen müssen nach dem Update einmal neu ausgewählt werden.

**Installationsrichtung:** Ein bislang nicht manuell konfigurierter Lüfter startet mit **Auto / IN**. Genau zwei aktive Lüfter derselben Gruppe wählen automatisch einer IN und einer OUT. Eine feste Geräte-Reihenfolge verhindert Richtungswechsel durch eine neue Masterwahl. Eine manuelle IN-, OUT- oder physische Auswahl hat Vorrang; ein automatischer Partner passt sich an. Sind beide manuell eingestellt, bleiben beide Vorgaben erhalten. Bei mehr als zwei aktiven Gruppenmitgliedern erfolgt keine neue automatische Aufteilung. Mit **Auto** lässt sich eine manuelle Vorgabe wieder aufheben.

Die lokale und die über ein Gateway geöffnete Webseite enthalten angepasste Schaltflächen und Hinweise. Alte Firmware wird dort entsprechend gekennzeichnet.

202 Firmware-Hosttests, 54 native Regressionstestprogramme, beide Hardwarebuilds, Tasten-/LED-Profilprüfungen, Codec-/Kryptografie-Interoperabilität sowie Signatur-/Stackprüfungen bestanden. Die Tests prüfen gespeicherte Rollen beim Start, Speicherfehler, Gateway-Ausfall, manuelle Richtungen und automatische Paare. **Ein realer Neustart/Rollenwechsel und die automatische Paarzuordnung mit zwei physischen Lüftern wurden für diese Version noch nicht getestet.**

Voraussetzung: ESP8266 ESP-12F, 4 MiB Flash, Hardwareprofil, A/B-Layout 2. In der App unter **Firmware-Updates** die **Beta-Versionen einschließen**. Für die neuen App-Schaltflächen außerdem Android 3.3.16 installieren. Das Update führt keinen Werksreset aus.
