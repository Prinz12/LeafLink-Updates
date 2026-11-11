# LeafLink Android 3.3.34 – Stabile Netzwerkübersicht

- Die Netzwerkübersicht aktualisiert vorhandene Karten und Werte, ohne bei jeder
  Messung die gesamte sichtbare Ansicht neu aufzubauen.
- Beim Drehen und nach einem Appwechsel bleibt die Netzwerkseite einschließlich
  gewähltem Lüfter erhalten. Unterbrochene Verbindungstests können erneut gestartet werden.
- Handy und Router bleiben auch bei vielen direkten Gateways über der seitlich
  verschiebbaren Gerätekarte sichtbar.
- Aktuell gemeldete Verbindungen werden durchgezogen dargestellt. Veraltete und
  unbestätigte Abschnitte bleiben gestrichelt.
- Statt „auffällig“ nennt die Übersicht den betroffenen Lüfter und die Beobachtung:
  fehlende Antworten oder schwaches WLAN mit Empfangswert.

Die Geräteprüfung misst weiterhin den gesamten Weg vom Handy zum jeweiligen
Lüfter. Sie weist keinen einzelnen Funkabschnitt als Ursache fehlender Antworten nach.

## Installation

Als Update installieren, nicht deinstallieren. Kopplungen, Räume und Einstellungen
bleiben erhalten. Paket `de.prinz.leaflink`, Versionscode 43, Android 6.0 oder neuer.
Gegenüber 3.3.33 ist kein zusätzliches Firmware- oder Wall-Update erforderlich.
Die Anforderungen des Sicherheitsupdates ab App 3.3.27 bleiben gültig.

## Prüfung

Android-Build, Lint, Netzwerk-, Protokoll-, Übersetzungs- und Updateprüfungen sowie
Firmware-Kompatibilitätstests. Isolierte Emulatorprüfungen für Hochformat, Querformat
und 130 % Schriftgröße, einschließlich stabiler Aktualisierung und Wiederherstellung
der gewählten Lüfterseite. Zusätzlich wurde der Wechsel zwischen Hoch- und Querformat
auf einem Galaxy S23 Ultra geprüft. Ein Dauertest mehrstufiger Funkketten ist nicht enthalten.
