# LeafLink Android 3.2.4 – Firmware-Updates erneut starten

- „Fehlversuch prüfen“ erkennt Abbrüche vor dem ersten Firmwareupload und
  schließt den alten Versuch nach erneuter Geräteprüfung ab.
- Mit „Alten Versuch abschließen“ lässt sich ein neuer Updateversuch vorbereiten,
  auch nach einer USB-Reparatur oder inzwischen geänderten Einstellungen.
- Der alte Versuch bleibt archiviert. Ein neuer Upload erfordert erneut
  Geräteauswahl und Bestätigung. Es erfolgt keine automatische Wiederholung.
- Laufende Updates, unbestätigte Starts, falsche Gerätekennung und instabile
  Zustände bleiben geschützt. Die Prüfung selbst benötigt keinen Download.
- Das Prüfergebnis wird sichtbar angezeigt und bleibt nach App-Neustart erhalten.

Unterstützt weiterhin HAPLA und LeafLink. Paket `de.prinz.leaflink`, versionCode 8,
Android ab API 23, bisheriges LeafLink-Signaturzertifikat. Als Update über die
bestehende App installieren; App-Daten, Gruppen und Hausplan bleiben erhalten.

Firmware 3.2.4 Beta wird separat für Hardware und Safe angeboten. Eine alte
Firmware, die bereits die OTA-Vorbereitung dauerhaft wegen Speichermangel
ablehnt, benötigt zunächst ein datenbehaltendes USB-Firmwareupdate. Das
Abschließen eines App-Versuchs behebt keinen RAM-Mangel auf dem Gerät.

Geprüft: acht Android-Hosttestsuiten, Build und Release-Lint, 105 isolierte
Update-/Journal-/UI-Prüfungen, öffentliche Firmwarekanalprüfung sowie
datenbehaltendes App-Update und Fehlversuchsprüfung auf einem Samsung SM-S918B.
