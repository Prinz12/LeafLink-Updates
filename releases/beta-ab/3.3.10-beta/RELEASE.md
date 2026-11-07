# LeafLink 3.3.10 Beta – Stabile Raumabfragen

Behebt einen zu hohen Stackbedarf bei der verschlüsselten Abfrage der
Raumzuordnung. Dieser Ablauf konnte einen Lüfter kurz unerreichbar machen und
einen Watchdog-Neustart auslösen. Die App zeigte dann „Keine Geräteantwort bei:
geschützter Befehl“.

Raumabfragen laufen jetzt über einen eigenen kleinen Antwortpfad und verwenden
einen vorhandenen Puffer. Das spart 1760 Byte Stack während der Antwort.
Authentifizierung, Geräteidentität, Signaturprüfung und A/B-Rückfall bleiben aktiv.
Die zusätzliche OTA-RAM-Reserve und die reduzierten Routineausgaben aus 3.3.9
bleiben erhalten; serielle Diagnose und Flasher-Protokolle sind weiter verfügbar.

Der Fehler wurde auf einem betroffenen Lüfter mit 3.3.9 seriell reproduziert.
Nach dem Update auf 3.3.10 gab es bei 1500 geschützten Raumabfragen keinen
Neustart und 1499 gültige Antworten. Eine einzelne UDP-Zeitüberschreitung blieb
ohne Neustart; die folgenden Abfragen funktionierten wieder. Ein zweiter Lüfter
beantwortete 500 von 500 Abfragen. 201 Hosttests, 49 native Regressionstests, Protokollvergleich,
Hardwarebuild und erweiterte Stack-Audits bestanden.
Ein mehrtägiger Dauertest ist damit nicht ersetzt.

Kopplungen, WLAN-Daten, Hausplan, Nutzungszähler und Einstellungen bleiben bei
normalen Firmwareupdates erhalten. Kein Werksreset und kein zusätzliches
App- oder Wall-Control-Update erforderlich. Bereits archivierte Fehlermeldungen
werden durch das Firmwareupdate nicht gelöscht.

Voraussetzung: ESP8266 ESP-12F mit 4 MiB Flash, Hardwareprofil und A/B-Layout 2.
In der App unter **Firmware-Updates** die **Beta-Versionen einschließen**, dann
**VERSION PRÜFEN** und **FIRMWARE HERUNTERLADEN** wählen.
