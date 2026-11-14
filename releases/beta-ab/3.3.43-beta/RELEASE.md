# LeafLink 3.3.43 Beta – Weitere Bediengeräte und bewusster Kopplungsstart

- Ein bereits autorisiertes Bediengerät kann einem weiteren Handy oder Tablet
  einen eigenen Zugang erteilen. Die Übertragung startet ausdrücklich per
  Freigabe-QR in App 3.3.45; vorhandene Zugänge und laufende Sitzungen bleiben erhalten.
- Erneute Freigaben desselben vorbereiteten Zugangs belegen keinen zusätzlichen
  Platz. Kennungskonflikte, volle Zugangsspeicher und Speicherfehler werden geprüft.
- Fabrikneue Lüfter ohne gespeichertes Netz öffnen beim Einschalten keinen
  Kopplungsmodus mehr. Für WLAN-Einrichtung die Taste etwa vier Sekunden drücken
  und loslassen. Die vorhandene kurze Tastengeste für die Wall-Anmeldung bleibt
  erhalten. Bereits gespeicherte Netzwerke starten weiterhin automatisch.
- Der absichtlich geschlossene Fabrikstart wird von der A/B-Startprüfung
  berücksichtigt; Speicher- und Motorprüfungen bleiben aktiv.

Zuerst **App 3.3.45** auf beiden Bediengeräten installieren, anschließend die
Lüfter aktualisieren. Dieses signierte Image ist für vorhandene
ESP8266/ESP12F-Hardware mit 4 MB und **A/B-Layout 2** bestimmt.
Kopplungen, WLAN-Einstellungen und Hausplan bleiben beim Update erhalten.

206 Firmware-Hosttests, 77 native Regressionsexecutables, Codec-Interoperabilität
und beide Hardware-Builds bestanden. Zehn eingeschaltete Lüfter wurden aktualisiert;
Firmware-Hash, bestätigter Neustart und erhaltene Einstellungen wurden geprüft.
Die Freigabe an ein Samsung-Tablet sowie ihre Wiederholung waren für alle zehn
Lüfter erfolgreich. Der geschlossene Fabrikstart wurde durch native Tests der
tatsächlichen Startfunktion geprüft; bestehende Geräte wurden dafür nicht gelöscht.
Einzelne Funkpakete können weiterhin verloren gehen. Beta-Version, keine
Zusage unbegrenzter Langzeitstabilität.

Im anschließenden parallelen Test beantworteten Handy und Tablet 400/400
authentifizierte Abfragen über rund zehn Minuten, ohne unerwarteten Lüfterneustart.
Die ursprünglichen Betriebszustände waren danach unverändert.
