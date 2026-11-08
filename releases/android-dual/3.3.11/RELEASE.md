# LeafLink Android 3.3.11 – Mehrere Lüfter im WLAN einrichten

Nach erfolgreicher WLAN-Einrichtung lässt sich mit **Weiteren Lüfter hinzufügen**
direkt der nächste Lüfter einrichten. Das zuvor verwendete Ziel-WLAN und sein
Passwort werden während der geöffneten Einrichtungsrunde vorausgefüllt.

## Änderungen

- **Neue Einrichtung** verwirft den Gerätecode des vorherigen Lüfters. Für den
  nächsten LeafLink-Lüfter wird dessen eigener Code abgefragt.
- Ziel-WLAN und Passwort müssen nicht für jeden Lüfter erneut eingegeben werden.
  Die Übertragung wird weiterhin für jeden Lüfter bestätigt.
- Die Gruppenzuordnung erfolgt pro Lüfter. Während des Speicherns kann nicht
  vorzeitig zur Einrichtung des nächsten Lüfters gewechselt werden.
- Andere WLANs erhalten kein vorausgefülltes Passwort. Die WLAN-Zugangsdaten
  werden nur im Arbeitsspeicher gehalten und beim Schließen der Einrichtung
  gelöscht. Nach einem App-Neustart oder einer Neuerstellung des Bildschirms
  müssen sie erneut eingegeben werden.

## Installation und Prüfung

Über **App-Update** nach Updates suchen oder die APK über die vorhandene App
installieren. Paketkennung und Signatur bleiben gleich; vorhandene App-Daten,
Kopplungen und Hauspläne bleiben erhalten. Android 6.0 oder neuer erforderlich.

Build, Lint, Setup- und Protokolltests sowie 42 Prüfungen für aufeinanderfolgende
Einrichtungen und 20 Wiederaufnahme-Prüfungen im Android-Emulator bestanden.
Eine vollständige Einrichtungsrunde mit mehreren physischen Lüftern wurde für
diese Änderung noch nicht geprüft.
