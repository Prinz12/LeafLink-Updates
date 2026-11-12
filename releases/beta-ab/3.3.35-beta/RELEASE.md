# LeafLink 3.3.35 Beta – Getaktete Gateway-Funkübertragung

Verlässliche Gateway-Telegramme werden aus den vorhandenen Puffern asynchron
gesendet: höchstens ein Fragment pro Serviceaufruf, weitere erst nach den
SDK-Sendecallbacks. Je Ziel wartet höchstens ein Telegramm auf seinen Mesh-ACK.
Dadurch können jüngere Telegramme wartende ältere nicht überholen. Der ACK-Timer
beginnt nach dem letzten Fragment. Wiederholungen bleiben begrenzt; es kommen
keine zusätzlichen Paketpuffer hinzu. Authentifizierung, Replay-Schutz,
Signaturprüfung und bestätigter A/B-Start bleiben erhalten.

An Repeater 1255 wurde dasselbe signierte Image über Gateway 6469 geprüft.
Die frühere Referenz mit App 3.3.40 / Gateway 3.3.34 benötigte 261,423 Sekunden
und 97 App-Wiederholungen. Zwei neue vollständige Läufe ergaben:
- 184.768 Sekunden, 6 App-Wiederholungen.
- 188.009 Sekunden, 19 App-Wiederholungen.

Beide Läufe bestätigten Imagehash, anderen A/B-Slot, gesunden Neustart,
Repeaterrolle, Einstellungen und Hausplan. Die Funkbedingungen können sich
zwischen den Messungen ändern; die Ergebnisse sind kein Langzeitnachweis.

9857 und 6469 wurden datenbewahrend aktualisiert. 1255 blieb für den identischen
Imagevergleich auf 3.3.33. Für den Gewinn die möglichen Gateways auf 3.3.35
aktualisieren; das adaptive App-Fenster benötigt Repeater-Firmware ab 3.3.33.
Hardware-Anwendungsupdate für ESP8266, 4 MiB, A/B-Layout 2; kein Zurücksetzen.
