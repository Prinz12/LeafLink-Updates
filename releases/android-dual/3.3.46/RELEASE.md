# LeafLink Android 3.3.46 – Vollständigen Hausplan übernehmen

„Weiteres Bediengerät hinzufügen“ überträgt jetzt auch den vollständigen
gespeicherten Hausplan. Zuvor wurden nur die Lüfterzugänge freigegeben; auf dem
neuen Gerät konnten dadurch einfache, gleichmäßig angeordnete Rechtecke entstehen.

Enthalten sind alle gespeicherten Planobjekte und Planeinstellungen: Etagen,
Raumformen, Teilflächen, Anordnung und Maße, Materialien, Fenster, Türen und
Durchgänge samt Positionen, Breiten, Anschlägen und Öffnungsrichtungen,
Etagenverbindungen, Lüfterpositionen, Wandzuordnungen sowie Raum- und Gruppennamen.
Der vollständige Plan wird unabhängig von der Erreichbarkeit einzelner Lüfter
übernommen. Bestehende Lüfterzugänge bleiben erhalten.

**Beide Bediengeräte auf App 3.3.46 aktualisieren**, anschließend die Freigabe vom
Gerät mit dem gewünschten vollständigen Plan wiederholen. Der Quellplan ersetzt
den bisherigen Plan auf dem Empfänger. Dabei wird keine zusätzliche Sicherung
des alten Empfängerplans angelegt. Die manuelle Hausplansicherung bleibt verfügbar.
Für die Zugangsfreigabe ist weiterhin Firmware 3.3.43 Beta erforderlich; für
diese Plankorrektur ist kein weiteres Firmware-Update nötig.

Der Transfer erfolgt lokal und verschlüsselt. Der Empfänger bestätigt erst nach
Validierung, Speicherung und vollständigem Inhaltsvergleich. Wiederholung,
gemeinsame Planrevision und Neuladen der Ansicht verhindern, dass wieder ein
unabhängiger Ersatzplan angezeigt wird. Ältere Gegenstellen zeigen einen Hinweis
auf das notwendige App-Update für die Planübernahme.

Auf Samsung-Handy und Samsung-Tablet geprüft: identische Planinhalte mit
3 Etagen, 17 Raumflächen, 10 Fenstern, 11 Türen, 1 Durchgang,
1 Etagenverbindung und 10 Lüfterpositionen – auch nach Neustart und Anzeige.
10/10 vorhandene Zugänge erneut bestätigt. Objekt-, Speicherfehler-,
Editor-, Import- und Verschlüsselungstests sowie Release-Build und Lint bestanden.
Der QR wurde im automatisierten Test aus dem gerenderten Bild decodiert;
der optische Kamerascan war nicht Bestandteil dieses Tests.

Android 9 oder neuer erforderlich (minSdk 28); targetSdk bleibt Android 16 (36).
Als Update ohne Deinstallation installieren. Diese Veröffentlichung enthält
ausschließlich die App; Firmware und physische Lüftereinstellungen bleiben unverändert.
