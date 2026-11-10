# LeafLink Android 3.3.30 – Hauptseiten folgen dem Finger

Korrigiert die Wischgesten zwischen **Home → Hausplan → Meldungen → Einstellungen**. In 3.3.29 begann der seitliche Übergang erst nach dem Loslassen. Jetzt folgt die aktuelle Seite direkt dem Finger und die benachbarte Seite wird bereits während des Ziehens sichtbar – wie in der Lüfter-Bedienansicht.

- Kurze oder abgebrochene Gesten gleiten zur Ausgangsseite zurück.
- Zurückziehen und Richtungswechsel funktionieren während derselben Geste.
- Wischstrecke, Geschwindigkeit und Rückgleitdauer verwenden dieselben Regeln wie der Raumwechsel.
- Die untere Leiste bleibt stehen. Regler, vertikales Scrollen und Hausplan-Zoom/Verschieben behalten Vorrang.
- Eine Meldungsvorschau markiert noch nichts als gelesen. Erst ein abgeschlossener Wechsel öffnet die Zielseite.
- Wird die App verlassen oder die Ansicht während der Bewegung geschlossen, wird die Geste sauber abgebrochen.

## Installation und Kompatibilität

Paket `de.prinz.leaflink`, Versionscode 39, Android 6.0 oder neuer, bestehendes Release-Zertifikat. Als Update installieren; App-Daten und Kopplungen bleiben erhalten.

Unveränderter Protokollstand gegenüber 3.3.29: LeafLink-Firmware 3.3.25 Beta und bei App-Zugriff über die Wall deren Gateway 0.6.8 Beta. HAPLA-Unterstützung bleibt enthalten. Beim Wechsel von Versionen vor 3.3.27 die [Reihenfolge des Sicherheitsupdates](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.27) beachten.

Die Fingerbewegung wurde ausdrücklich vor dem Loslassen im Android-Emulator geprüft. Diese Veröffentlichung installiert keine App oder Firmware automatisch.
