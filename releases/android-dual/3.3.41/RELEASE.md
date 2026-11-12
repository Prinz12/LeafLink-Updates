# LeafLink Android 3.3.41 – Repeater schneller erreichen

Frisch erkannte, gekoppelte Repeater werden beim ersten Lesen bevorzugt über
Mesh angesprochen. Der kurzlebige Transporthinweis ersetzt keine authentifizierte
Identitätsprüfung und ändert keine Zieladresse. Veraltete Hinweise dürfen nur
beim Lesen auf HTTP zurückfallen; Prepare und Upload werden nicht wiederholt.
Im lesenden Vergleich an 1255: 5433 ms bisher, 453 ms mit Mesh-Hinweis.

Die zusätzliche Beschleunigung der Datenübertragung kommt aus Gateway-Firmware
3.3.35. Das adaptive Fenster mit höchstens zwei Blöcken bleibt unverändert.

An Repeater 1255 wurde dasselbe signierte Image über Gateway 6469 geprüft.
Die frühere Referenz mit App 3.3.40 / Gateway 3.3.34 benötigte 261,423 Sekunden
und 97 App-Wiederholungen. Zwei neue vollständige Läufe ergaben:
- 184.768 Sekunden, 6 App-Wiederholungen.
- 188.009 Sekunden, 19 App-Wiederholungen.

Beide Läufe bestätigten Imagehash, anderen A/B-Slot, gesunden Neustart,
Repeaterrolle, Einstellungen und Hausplan. Die Funkbedingungen können sich
zwischen den Messungen ändern; die Ergebnisse sind kein Langzeitnachweis.

Ohne Deinstallation aktualisieren; Kopplungen und Einstellungen bleiben erhalten.
