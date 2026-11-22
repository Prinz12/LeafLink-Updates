# LeafLink Lüfter-Firmware 4.0.6

Diese Version verbessert den lokalen Webzugriff aus LeafLink und im normalen Browser. Der Lüfter überträgt die Startseite samt Anmeldeskripten in einer HTTPS-Antwort und schließt die Übertragung vollständig ab. Eine unterbrochene Statusabfrage darf der Browser einmal wiederholen. Bedienbefehle werden einmal gesendet.

Bei knappem Arbeitsspeicher behandelt der WLAN-Empfang fehlenden Platz für die Paketverwaltung. Statusantworten der App werden bevorzugt. Vorhandene Kopplungen und gültige Gerätezertifikate können weiterverwendet werden.

In LeafLink **Firmware-Updates** öffnen, **Version prüfen**, die Lüfter suchen und das Update für die gewünschten Geräte starten. Nach dem Neustart zeigt die App die bestätigte Firmware an.

Das signierte Paket ist für LeafLink-Lüfter mit ESP8266, 4 MiB Flash, Hardwareprofil und A/B-Bootlayout 2 bestimmt.
