# LeafLink Android 3.3.29 – Fließende Seitenwechsel und neues Blatt-Icon

In der Lüfter-Bedienansicht folgen die Raumseiten jetzt dem Finger: Der nächste Raum kommt seitlich ins Bild. Kurze oder abgebrochene Gesten gleiten zurück; längere oder schnelle Wischbewegungen wechseln den Raum.

Auch auf den Hauptseiten ist Wischen möglich, in derselben Reihenfolge wie die untere Leiste: **Home → Hausplan → Meldungen → Einstellungen**. Nach der Geste gleiten die Seiten seitlich ineinander. Nach rechts geht es zurück. Die untere Navigationsleiste bleibt stehen. Regler, vertikales Scrollen und das Verschieben oder Zoomen im Hausplan behalten ihre eigenen Gesten; im Hausplan funktioniert der Seitenwechsel über Kopfbereich oder Navigationsleiste.

Beim Start erscheint ein größeres grünes Blatt mit **LeafLink** darunter. Anschließend gleitet das Blatt zur Home-Navigation. Das Homescreen-Icon verwendet jetzt dieselbe Blattform auf weißem Hintergrund.

## Installation und Kompatibilität

- Paket `de.prinz.leaflink`, Versionscode 38, Android 6.0 oder neuer; bestehendes Release-Zertifikat.
- Als Update installieren: vorhandene App-Daten und Kopplungen bleiben erhalten.
- Gleicher Protokollstand wie Android 3.3.28: LeafLink-Firmware 3.3.25 Beta und bei App-Zugriff über die Wall deren Gateway 0.6.8 Beta. HAPLA-Unterstützung bleibt enthalten.
- Beim Wechsel von App-Versionen vor 3.3.27 die [Reihenfolge des Sicherheitsupdates](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.27) beachten.

## Prüfung

50 UI-Prüfungen für Raumwechsel, Gestenabbruch, Richtung, Hauptseiten-Reihenfolge, Regler- und Hausplanbedienung sowie Startdesign bestanden. Startbildschirm, Icon und Seitenübergänge wurden im Android-15-Emulator visuell geprüft.

Android-Hosttests, signierter Release-Build und Release-Lint sowie die vorgeschriebenen Codec-, Firmware-Host-/Native-Prüfungen und der Hardwareprofil-Build bestanden. Diese Veröffentlichung installiert keine App oder Firmware automatisch.
