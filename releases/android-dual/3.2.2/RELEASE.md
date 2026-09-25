# LeafLink Android 3.2.2 – Firmware-Abschlussprüfung korrigiert

Beim Update von Firmware 3.0.0 auf 3.2.0 konnte die App trotz erfolgreich
installierter und bestätigter Firmware „Settings or house plan changed“ melden.
Ursache waren die zusätzlich eingeführten Raumfelder. Dieser Vergleich ist korrigiert.

- Bekannte neue Raumfelder werden beim Versionswechsel berücksichtigt. Vorhandene Einstellungen und Hausplandaten werden weiterhin geprüft.
- **Firmware-Updates → Geräte prüfen** schließt einen bereits übertragenen und bestätigten Vorgang durch erneutes Auslesen ab. Es erfolgt dabei kein neuer Firmware-Upload.
- Die Geräteanzeige zeigt nach bestätigtem Start die tatsächliche Firmwareversion, auch wenn anschließend eine Einstellungsprüfung nötig ist.
- Gespeicherte Fehler- und Uploaddaten bleiben erhalten. Unklare oder unvollständige Uploads werden nicht automatisch fortgesetzt.
- Öffentliche App- und Firmware-Downloads bleiben ohne GitHub-Zugang verfügbar.

Die APK als Update über die bestehende LeafLink-App installieren. Paketkennung
und Signaturschlüssel bleiben gleich; die App-Daten werden nicht gelöscht.

Geprüft im virtuellen Android: 70 neue Abschlussprüfungen mit simuliertem
Versionswechsel und signierter Firmware, 176 vorhandene Firmware-Prüfungen,
26 Raumgruppen-Prüfungen sowie die Android-Hosttests. Build und Lint ohne Fehler.
