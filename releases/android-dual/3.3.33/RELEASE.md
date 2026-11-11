# LeafLink Android 3.3.33 – Netzwerkübersicht und Verbindungsprüfung

Die neue Netzwerkübersicht zeigt, welche LeafLink-Lüfter direkt als Gateway
arbeiten und welche über andere Lüfter erreichbar sind. Gemeldete Repeaterketten
mit bis zu sechs Funkhops werden dargestellt. Unvollständige und veraltete
Routen bleiben ausdrücklich gekennzeichnet.

## Neu

- **Einstellungen → Netzwerkübersicht → Verbindungen prüfen** öffnet die Karte.
- Antippen eines Lüfters öffnet seinen Verbindungsweg und die Prüfergebnisse.
  Der Einstieg ist auch direkt aus den Gerätedetails möglich.
- Kompakte Karten mit Gerätenummer, Raum, gemeldetem Funknachbarn und verfügbarem
  WLAN-Empfang. Die Prüfschaltfläche bleibt sichtbar, im Querformat seitlich.
- Zehn lesende Identitätsanfragen je Ziel liefern die Anzahl erfolgreicher
  Antworten und die mittlere Antwortzeit. Abbruch, Zeitlimits und Netzwechsel
  werden berücksichtigt.

Die Prüfung misst den gesamten Weg vom Handy zum jeweiligen Lüfter. Sie weist
keine einzelne Funkstrecke eindeutig als Fehlerursache nach. Nicht gemeldete
Empfangswerte werden nicht erfunden. Die Karte betrifft LeafLink-Geräte;
HAPLA-Geräte bleiben in den bisherigen App-Funktionen unterstützt.

## Installation und Kompatibilität

Als App-Update installieren, nicht deinstallieren. Vorhandene App-Daten und
Kopplungen bleiben erhalten. Paket `de.prinz.leaflink`, Versionscode 42,
Android 6.0 oder neuer.

Für diese Erweiterung ist gegenüber App 3.3.32 kein zusätzliches Firmware-
oder Wall-Update erforderlich. Die Anforderungen des Sicherheitsupdates ab
App 3.3.27 / Firmware 3.3.25 / Wall 0.6.8 gelten weiterhin.

## Prüfung

Android-Build und Lint, Diagnose- und Protokolltests sowie isolierte
Emulatorprüfungen bestanden, einschließlich kleinem Display, 130 % Schriftgröße
und Querformat. Verlorene Antworten, veraltete Daten, fehlende Nachbarn und
widersprüchliche Routen wurden geprüft. Firmware-Kompatibilitätstests bestanden.
Ein realer Dauertest einer mehrstufigen Funkkette steht noch aus.

Die Veröffentlichung installiert die App nicht automatisch auf dem Handy.
