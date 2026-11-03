# LeafLink 3.2.10 Beta – WLAN-Wechsel nach älterer Direktkopplung

Ältere gespeicherte Wall-Kopplungen konnten weiterhin per Direktfunk bedient
werden, beantworteten jedoch keine Anfragen zur Netzauswahl oder WLAN-Übertragung.
Ihnen fehlte der später eingeführte verschlüsselte Wall-Netzdatensatz.

3.2.10 übernimmt die bereits authentifiziert gespeicherten Funkzugangsdaten und
die bestehende Bindung einmalig in dieses Format. Nur ein vollständig gelöschtes
Erweiterungsfeld wird migriert. Beschädigte oder nicht authentifizierbare neue
Datensätze werden nicht durch einen Rückgriff auf alte Daten akzeptiert.

Danach läuft der normale verschlüsselte Abgleich mit Wall Control 0.5.10:
WLAN-Daten prüfen/übertragen, gewählte Netzart speichern und tatsächliche
Verbindung bestätigen. Kopplung, Gruppen und andere Einstellungen bleiben
erhalten; kein Zurücksetzen oder erneutes Koppeln erforderlich.

A/B-Startprüfung, Signaturprüfung, Rückfall und spätere OTA-Updates bleiben
erhalten. Signiertes A/B-Anwendungsupdate für 4-MB-ESP8266, Layout 2.
Hardware-/Safe-Profil passend auswählen; Safe deaktiviert die Motoransteuerung.

Profil: **hardware**.
