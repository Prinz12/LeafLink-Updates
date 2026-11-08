# LeafLink Android 3.3.14 – Stromlose Lüfter schneller erkennen

Die App erkennt fehlende Antworten jetzt unabhängig vom normalen Übersichtsrefresh.
Bei geöffneter App verschwindet ein dauerhaft nicht erreichbarer Lüfter normalerweise
nach ungefähr 10–15 Sekunden aus der aktiven Übersicht.

## Änderungen

- Öffentliche Status-Pings alle fünf Sekunden und eine Offline-Prüfung jede Sekunde.
- Nach zehn Sekunden ohne gültige Antwort folgen zwei Kontrollanfragen und ein
  viersekündiges Bestätigungsfenster. Einzelne verlorene Antworten werden toleriert.
- Gespeicherte Lüfter, Kopplungen und Raumzuordnungen bleiben erhalten. Nach Rückkehr
  der Antworten erscheint der Lüfter automatisch wieder.
- Häufigere Status-Pings erhöhen nicht den Takt der zugehörigen Detailabfragen.
- App-Pausen und Netzwerkwechsel brechen offene Offline-Prüfungen ab.

## Installation und Prüfung

Über **App-Update** installieren. Paketkennung und Signatur bleiben gleich;
App-Daten und Einstellungen bleiben erhalten. Android 6.0 oder neuer erforderlich.

Build, Lint und automatisierte Erreichbarkeits-, Warteschlangen- und Suchprüfungen
bestanden. Auf einem Samsung SM-S918B wurde ein Antwortausfall mit dem echten
App-Repository und einem lokalen UDP-Testendpunkt geprüft: Offline nach 14,1 Sekunden
seit letzter Antwort, einzelne verlorene Antwort toleriert und automatische
Wiedererkennung erfolgreich. Die reale Stromtrennung eines Lüfters wurde dabei
nicht durchgeführt. Die Zeitangabe gilt für eine laufende App und ist keine harte
Echtzeitgarantie.
