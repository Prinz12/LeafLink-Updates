# LeafLink 3.3.11 Beta – Neustartkorrektur bei App-Abfragen

Behebt einen Stacküberlauf bei normalen geschützten App-Abfragen. Ein nur
für die Einrichtung benötigter WLAN-Scan-Puffer belegte bisher auch während
anderer Befehle Speicher auf dem Stack. Bei verschlüsselten Antworten und
WLAN-Übertragung konnte dies einen ungeplanten Neustart auslösen.

Der WLAN-Scan läuft jetzt in einer getrennten Funktion. Das reduziert den
Stackbedarf des allgemeinen Befehlshandlers um 656 Byte, ohne zusätzlichen
Heap zu benötigen. Die Korrektur für Raumabfragen aus 3.3.10 und die
OTA-RAM-Verbesserungen aus 3.3.9 bleiben enthalten. Normale Debugausgaben
bleiben reduziert; serielle Diagnose und Flasher-Protokolle sind verfügbar.
Authentifizierung, Signaturprüfung und A/B-Rückfall bleiben aktiv.

Geprüft wurden zwei Lüfter mit jeweils 30 Minuten gemischter Netzwerklast und
anschließender Ruhephase. Dabei trat kein Neustart auf; Einstellungen blieben
erhalten. Einzelne UDP-Antwortausfälle ohne Neustart wurden beobachtet.
202 Firmware-Hosttests, 50 native Regressionstestprogramme, Protokollvergleich,
Hardwarebuild, verschärfte Stack-Prüfungen und serielle Installerprüfungen
bestanden. Ein mehrtägiger Dauertest ist dadurch nicht ersetzt.

Kopplungen, WLAN-Daten, Hausplan, Nutzungszähler und Einstellungen bleiben bei
normalen Firmwareupdates erhalten. Kein Werksreset und kein zusätzliches
App- oder Wall-Control-Update erforderlich. Bereits archivierte Fehlermeldungen
werden durch das Firmwareupdate nicht gelöscht.

Voraussetzung: ESP8266 ESP-12F mit 4 MiB Flash, Hardwareprofil und A/B-Layout 2.
In der App unter **Firmware-Updates** die **Beta-Versionen einschließen**, dann
**VERSION PRÜFEN** und **FIRMWARE HERUNTERLADEN** wählen. Anschließend die
gewünschten Lüfter über den bestehenden Updateablauf aktualisieren.
