# LeafLink 3.3.57 Beta

Diese Version verbessert die Rückkehr von Lüftergruppen ins WLAN und enthält die WLAN-Verwaltung und den Verbindungsverlauf aus den Versionen 3.3.55 und 3.3.56.

- Bei den ersten beiden Versuchen sucht der Lüfter bis zu 1,5 Sekunden und wartet bis zu 4 Sekunden auf Anmeldung und IP-Adresse. Ab dem dritten Versuch sucht er bis zu 4 Sekunden und gibt der Verbindung bis zu 15 Sekunden. Nach erfolgreicher Rückkehr gelten wieder die kurzen Fristen.
- Während der Suche führt der Lüfter den zuletzt synchronisierten Gruppentakt lokal fort. Bei Kanalwechseln können Gruppenpakete kurz ausbleiben. Die Status-API zeigt die verwendeten Fristen und den letzten Fehler.
- Im Gerätedialog der LeafLink-App ab 3.3.58 lassen sich WLAN-Zugänge ersetzen und zusätzliche Netze hinterlegen. Der Lüfter kann anhand der Signalstärke zwischen den gespeicherten Netzen wählen.
- Bei ausbleibenden Antworten des lokalen Routers versucht der Lüfter eine erneute WLAN-Anmeldung. Die Gerätewebseite zeigt die letzten drei gespeicherten Verbindungsstörungen.

Das signierte Paket ist für ESP8266-Lüfter mit 4 MiB Flash und A/B-Layout 2 bestimmt. Im Firmwareupdate der App „Beta-Versionen anzeigen“ aktivieren und „Version prüfen“ wählen.

Auf einem Testlüfter wurden der bestätigte Start, die Routerantwort und die Gruppenverbindung sowie der Erhalt von Einstellungen und Hausplan geprüft. Die verzögerte IP-Vergabe und die Richtungswechsel während der Suche wurden im Simulationstest geprüft.
