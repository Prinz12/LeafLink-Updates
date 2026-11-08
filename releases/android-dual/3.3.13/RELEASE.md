# LeafLink Android 3.3.13 – Lüfter schneller wiederfinden

Die App sucht fehlende bekannte Lüfter bei geöffneter App alle fünf Sekunden
an ihren gespeicherten privaten Adressen. Ausgeschaltete oder langsam antwortende
Geräte halten die Erkennung anderer Lüfter nicht mehr auf.

## Änderungen

- Gemeinsame schnelle Suche für beide unterstützten Protokolle, mit einer
  Wiederholung fehlender Antworten und begrenzter Laufzeit.
- Status-Pings laufen unabhängig von langsamen geschützten Abfragen.
  Steuerbefehle behalten ihre Reihenfolge und Authentifizierung.
- Geräteübersichten anderer Lüfter werden unabhängig von langsamen Einzelabfragen
  gelesen. Kürzlich antwortende Geräte erhalten keine zusätzlichen Suchanfragen.
- Netzwerkwechsel und gelöschte Geräte verwerfen veraltete Suchergebnisse.

Die schnelle Wiedererkennung setzt eine bekannte, weiterhin gültige IP-Adresse
und eine erreichbare Firmware voraus. Weitere Suchverfahren bleiben aktiv.
Die Zeit, die der Lüfter selbst zum WLAN-Verbindungsaufbau braucht, bleibt davon
unabhängig; eine feste Erkennungszeit ab Einschalten wird nicht zugesichert.

## Installation und Prüfung

Über **App-Update** nach Updates suchen oder über die vorhandene App installieren.
Paketkennung und Signatur bleiben gleich; App-Daten, Kopplungen und Hauspläne
bleiben erhalten. Android 6.0 oder neuer erforderlich.

Build, Lint, UDP-, Warteschlangen-, Protokoll- und Einrichtungsprüfungen bestanden.
Alle 52 Suchlogik-Prüfungen bestanden zusätzlich auf einem Samsung SM-S918B.
Die neue Suche fand einen erreichbaren echten Lüfter über das Handy-WLAN nach
66 ms. Das ist eine einzelne Suchmessung, kein Vergleich der Einschaltzeit.
Das Update wurde auf dem Handy mit erhaltenen Daten installiert.
