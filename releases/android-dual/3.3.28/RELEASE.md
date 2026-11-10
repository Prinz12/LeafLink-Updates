# LeafLink Android 3.3.28 – QR-Scanner mit Scanrahmen

Der QR-Scanner zeigt jetzt einen mittigen Rahmen mit abgerundeten Eckmarkierungen, einer langsam wandernden Scanlinie und einem abgedunkelten Außenbereich. Ein Gerätecode wird erst übernommen, wenn der vollständige QR-Code innerhalb des Rahmens liegt.

Bei erfolgreicher Erkennung erscheinen kurz ein grüner Rahmen und ein Häkchen. Eine kurze Vibration bestätigt den Scan; anschließend geht die Einrichtung automatisch weiter. Die Taschenlampentaste schaltet das Kameralicht bei Bedarf ein und aus. Auf Geräten ohne unterstütztes Kameralicht ist die Taste deaktiviert. Beim Verlassen des Scanners und nach erfolgreichem Scan werden Kamera und Licht freigegeben.

Die Verarbeitung bleibt lokal auf dem Handy. Kameraaufnahmen und Gerätecodes werden nicht hochgeladen.

## Installation und Kompatibilität

- Paket `de.prinz.leaflink`, Versionscode 37, Android 6.0 oder neuer; bestehendes Release-Zertifikat.
- Als Update installieren: vorhandene App-Daten und Kopplungen bleiben erhalten.
- Gleicher Protokollstand wie Android 3.3.27: für LeafLink-Lüfter Firmware 3.3.25 Beta und bei App-Zugriff über die Wall deren Gateway 0.6.8 Beta verwenden. HAPLA-Unterstützung bleibt enthalten.
- Beim Wechsel von App-Versionen vor 3.3.27 die [Reihenfolge des Sicherheitsupdates](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.27) beachten.

## Prüfung

114 Scannerprüfungen für Bildausschnitt, Kameradrehungen, Bildschirmformate und vollständig bzw. teilweise außerhalb liegende QR-Codes bestanden. Auf einem Samsung SM-S918B wurden Kamerastart, Taschenlampenschaltung, Pause/Fortsetzen, Erfolgsanzeige und Rückkehr mit erzeugten Kamerabildern geprüft. Die Haptik wurde softwareseitig ausgelöst; eine Prüfung mit einem gedruckten Geräteetikett war nicht Teil dieses Tests.

Android-Hosttests, signierter Release-Build, Release-Lint und Android-Emulatorprüfungen sowie die vorgeschriebenen Codec-, Firmware-Host-/Native-Prüfungen und der Hardwareprofil-Build bestanden. Diese Veröffentlichung installiert keine App und keine Firmware automatisch.
