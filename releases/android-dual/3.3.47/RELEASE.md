# LeafLink Android 3.3.47 – Ausstehende Freigaben und App zurücksetzen

„Weiteres Bediengerät hinzufügen“ berücksichtigt jetzt auch gespeicherte,
gerade ausgeschaltete Lüfter. Die ausdrücklich freigegebenen Zugänge werden
verschlüsselt vorgemerkt und bei geöffneter App automatisch nachgeholt, sobald
das freigebende Gerät die Lüfter erreicht. Anschließend bestätigt der Empfänger
seinen eigenen Zugang. Beide Apps müssen dafür nicht gleichzeitig geöffnet sein.

Es werden ausschließlich die beim QR-Vorgang freigegebenen Lüfter berücksichtigt.
Der bisherige Geräteschlüssel wird nicht weitergegeben. Ausstehende Freigaben
laufen nach sieben Tagen ab und lassen sich unter Einstellungen abbrechen.
Bereits erteilte Zugänge werden weiterhin über „Handyzugänge verwalten“ widerrufen.
Beide Apps müssen aktualisiert sein; die Lüfter benötigen Firmware 3.3.43 Beta
oder neuer. Diese App-Veröffentlichung ändert keine Firmware.

Beim Ergänzen von Lüftern kann der Empfänger seinen vorhandenen Hausplan behalten.
Bei einer leeren App ist die vollständige Planübernahme vorausgewählt; bei einem
vorhandenen Plan wird dessen Ersetzung ausdrücklich ausgewählt.

Neu unter **Einstellungen → Gerätezugänge → App vollständig zurücksetzen**:
Nach einer ausdrücklichen Bestätigung werden alle lokalen App-Daten einschließlich
Zugängen, Hausplan, lokalen Sicherungen, Einstellungen und Cache gelöscht.
Die App beendet sich und startet anschließend wie frisch installiert.
**Lüfter, deren Einstellungen und die auf ihnen gespeicherten Pläne bleiben erhalten.**
Während eines Firmware-Updates ist der Reset gesperrt.

Geprüft: 31 Prüfungen zu Verschlüsselung, Offline-/Wiederverbindungsfällen,
Wiederholungen, Ablauf und Abbruch auf Tablet und Emulator; 575 Kanal-/QR-Prüfungen;
vollständiger App-Reset einschließlich Keystore über die echte UI einer isolierten
Testinstallation; Release-Build, Lint und Lokalisierung. Die QR-Übertragung wurde
mit gerendertem QR und Scanner-Rückgabepfad geprüft, nicht mit optischer Kamera.

Android 9 oder neuer (minSdk 28), targetSdk Android 16 (36), Versioncode 57.
Als Update ohne Deinstallation installieren. Bestehende Zugänge und Pläne bleiben
beim normalen Update erhalten; die neue Reset-Aktion ist ausdrücklich optional.
