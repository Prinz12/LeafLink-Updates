# LeafLink Android 3.3.35 – Korrigierte Verbindungsprüfung

Enthält die flackerfreie Netzwerkübersicht, die Drehungskorrektur, sichtbar
bleibende Handy-/Routerelemente und konkrete Diagnosehinweise aus 3.3.34.

Der Verbindungstest berücksichtigt jetzt zwei zusätzliche Grenzen:

- Bis zu drei Sekunden Wartezeit je Antwort. Langsamere Antworten über Funkwege
  werden nicht mehr bereits nach einer Sekunde als fehlend gewertet.
- Mindestens 300 ms Pause zwischen Prüfanfragen. Damit löst die App bei einem
  einzelnen Prüflüfter nicht selbst die 250-ms-Antwortbegrenzung der Firmware aus.

Der Test bleibt rein lesend. Fehlende Antworten innerhalb des Zeitfensters werden
weiterhin angezeigt, ohne einen bestimmten Funkabschnitt als Ursache zu behaupten.
Das Gesamtzeitlimit beträgt weiterhin 90 Sekunden; Teilprüfungen sind gekennzeichnet.

Als App-Update installieren, nicht deinstallieren. Paket `de.prinz.leaflink`,
Versionscode 44, Android 6.0 oder neuer. Kopplungen, Räume und Einstellungen bleiben
erhalten. Gegenüber 3.3.33 ist kein zusätzliches Firmware- oder Wall-Update nötig.

Regressionsprüfung mit verzögerten Antworten nach 1,25 und 2,6 Sekunden, einer
nachgebildeten 250-ms-Firmwarebegrenzung, Paketverlust, Identitätsprüfung und
Netzwechsel; Android-Releasebuild und Lint. Die Darstellungskorrekturen wurden
im Emulator und auf einem Galaxy S23 Ultra geprüft.
