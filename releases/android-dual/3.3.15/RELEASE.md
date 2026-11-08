# LeafLink Android 3.3.15 – Gruppen wechseln und freie Partnerplätze wählen

Lüfter lassen sich über **Gruppe ändern** direkt in der Raumübersicht und im
Gerätedialog einer anderen Lüftungsgruppe zuordnen. Die Raumzuordnung bleibt erhalten.

## Änderungen

- Bestehende Zielgruppen werden mit Gruppenname und vorhandenem Lüfter angezeigt.
  Angeboten werden kompatible Gruppen mit genau einem freien Partnerplatz.
- Während der WLAN-Einrichtung stehen diese Gruppen direkt als Vorschläge bereit.
  Alternativ lässt sich weiterhin ein neuer Gruppenname eingeben.
- Gespeicherte Offline-Partner zählen mit: Eine volle Gruppe wird nicht als frei
  vorgeschlagen. Vor dem Speichern wird die Belegung erneut geprüft.
- Auch gleich benannte Gruppen werden korrekt ausgewählt; ihr vorhandenes Symbol
  wird bei der Einrichtung übernommen.
- Bestätigte Zuordnungen werden sofort gespeichert. Bei weiteren Lüftern derselben
  Einrichtungsrunde werden die Vorschläge aktualisiert, ohne die Einrichtung neu
  starten oder die WLAN-Daten nochmals eingeben zu müssen.

## Installation und Prüfung

Über **App-Update** installieren. Paketkennung und Signatur bleiben gleich;
App-Daten, Kopplungen und Hausplan bleiben erhalten. Android 6.0 oder neuer erforderlich.

Direkt auf einem Samsung SM-S918B bestanden 22 neue Gruppenprüfungen sowie die
bestehenden Raum-, Einrichtungs- und Inventarprüfungen. Auch Build, Lint, Protokoll-
und Übersetzungstests bestanden. Die Auswahl wurde mit isolierten Testdaten geprüft;
kein echter Lüfter wurde dabei umgruppiert.
