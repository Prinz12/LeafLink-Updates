# LeafLink Android 3.3.39 – Adaptive Repeater-Übertragung

Repeater ab Firmware 3.3.33 können ein kleines Sendefenster verwenden. Die App
beginnt mit einem Block und lässt nach stabilen Bestätigungen zwei Blöcke zu.
Das Sendetempo und die Wartezeit folgen der gemessenen Antwortzeit. Paketverlust
oder eine Lücke reduzieren das Fenster; nur bestätigte Bytes zählen als Fortschritt.

Der Gerätetest mit demselben Image und Gateway auf Repeater 1255 ergab 12.1 % weniger
Übertragungszeit (315.8 auf 277.5 Sekunden einschließlich Abschlussantwort).
Beide Updates bestätigten das richtige Image, einen neuen A/B-Start und den
Erhalt von Einstellungen und Hausplan. Die Dauer hängt von der Funkstrecke ab.
Dabei waren 133 statt 33 Wiederholungen nötig;
alle wurden innerhalb der laufenden Übertragung behandelt.

Signatur- und Neustartprüfung bleiben vollständig erhalten. Bei älterer
Firmware verwendet die App weiterhin den bisherigen Ein-Block-Ablauf.
Als App-Update installieren; Kopplungen und Einstellungen bleiben erhalten.
