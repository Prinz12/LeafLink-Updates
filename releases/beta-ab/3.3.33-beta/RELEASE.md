# LeafLink 3.3.33 Beta – Kleines Sendefenster für Repeater-Updates

Zusammen mit App 3.3.39 kann die Firmware bis zu zwei ausstehende Datenblöcke
verarbeiten. Sie bestätigt ausschließlich den lückenlos empfangenen Bereich;
die App überträgt fehlende Blöcke erneut. Zwei kleine Wiederholungsdatensätze
verhindern doppelte Schreibvorgänge. Es wird kein zusätzlicher Datenpuffer im
Repeater angelegt; der Flash-Arbeitspuffer bleibt bei 1 KiB.

Die App startet mit einem Block und erhöht nach stabilen Antworten auf zwei.
Bei Verlusten oder falscher Reihenfolge reduziert sie das Fenster wieder.
Verschlüsselung, Signaturprüfung, A/B-Rückfall und die Kontrolle von Gerät,
Imagehash, Start, Einstellungen und Hausplan bleiben erhalten.

Am Repeater 1255 wurde dasselbe signierte Image mit beiden Verfahren über
dasselbe Gateway und mit derselben bereits installierten Firmware übertragen:
Ein Block 315.8 s, adaptives Fenster 277.5 s – 12.1 % kürzere
Übertragungszeit einschließlich Abschlussantwort. Beide bestätigten Slotwechsel
und den Erhalt von Einstellungen und Hausplan ohne Rollenwechsel. Das ist eine
Messung unter den dortigen Funkbedingungen, keine Zusage für jede Verbindung.
Die App zählte 33 Wiederholungen mit einem Block und
133 mit dem Fenster. Der Gewinn ist eine kürzere Gesamtzeit,
kein Nachweis einer niedrigeren Paketverlustrate oder einer Langzeitzuverlässigkeit.
Auch die vorherige Erstinstallation von 3.3.32 auf 3.3.33 war erfolgreich.

Für die Beschleunigung benötigt der Repeater bereits 3.3.33 und die App 3.3.39.
Die Erstinstallation auf älterer Firmware verwendet den bisherigen Ablauf.
Ältere Apps und Firmware bleiben mit dem Ein-Block-Verfahren kompatibel.
Enthält die Gegenrichtungs-Korrektur aus 3.3.32. Für diese weiterhin auch die
Partner und ihre möglichen Gateways aktualisieren.

Signiertes Hardware-Anwendungsupdate für ESP8266, 4 MiB, A/B-Layout 2.
Kopplungen, Gruppen, Einstellungen und Hausplan bleiben erhalten.
