# LeafLink 3.3.13 Beta – Werksreset über die Gerätetaste

Der Lüfter kann ohne App oder WLAN mit einer zweistufigen Tastenfolge zur
Ersteinrichtung zurückgesetzt werden.

## Bedienung

1. Am eingeschalteten Lüfter die Taste etwa **15 Sekunden halten**, bis die LED
   wiederholt dreimal blinkt. Dann loslassen.
2. Innerhalb von **10 Sekunden erneut drücken** und etwa **4 Sekunden halten**,
   bis die LED dauerhaft leuchtet. Dann loslassen.
3. Erst dieses zweite Loslassen bestätigt das Löschen. Nach erfolgreichem Reset
   startet der Lüfter neu und ist wieder zur Einrichtung bereit.

Keine Bestätigung oder ein zu kurzer zweiter Druck brechen die Resetabsicht ab.
Dauerhaftes Halten allein löst keinen Reset aus. Firmwareupdates, noch nicht
bestätigter Firmwarestart und laufende Netzwerkübernahmen sperren den Reset.

## Daten und Update

Der ausdrücklich bestätigte Reset löscht WLAN-Zugangsdaten, Handy-/Wall-Kopplungen,
Direktgruppen, Raumzuordnung, persönliche Einstellungen und die lokale Hausplankopie.
Gerätenummer, gedruckter Gerätecode, installierte Firmware, Betriebsstunden und
Filterlaufzeit bleiben erhalten. Die Filterdaten bleiben jetzt auch beim
Werksreset über den Servicebereich erhalten. Andere Geräte und dort gespeicherte
Hauspläne oder Einträge werden nicht gelöscht.

**Das normale Firmwareupdate löst keinen Werksreset aus und erhält Einstellungen
und Kopplungen.** Voraussetzung: ESP8266 ESP-12F, 4 MiB Flash, Hardwareprofil und
A/B-Layout 2. Kein zusätzliches App- oder Wall-Update erforderlich.

In **Firmware-Updates** die **Beta-Versionen einschließen**, anschließend
**VERSION PRÜFEN** und **FIRMWARE HERUNTERLADEN** wählen.

## Prüfung

202 Firmware-Hosttests, 53 native Regressionstestprogramme, beide Hardwarebuilds,
Tasten-/LED-Tests mit zwei Herstellerprofilen, sieben ungültige Profilprüfungen,
Codec-/Kryptografie-Interoperabilität und Signatur-/Stackprüfungen bestanden.
Die Tests decken Abbruch, Zeitablauf, gehaltene Tasten, Zeitüberlauf, Datenbeibehaltung
und Speicherfehler ab. Bei Löschfehlern wird kein erfolgreicher Reset gemeldet;
wegen getrennter Speicherbereiche können bereits Teilbereiche gelöscht sein.

**Der reale Tastendruck, die LED-Anzeige und der Löschvorgang auf einem physischen
Lüfter wurden noch nicht geprüft.** Es wurde für diese Veröffentlichung kein
vorhandener Lüfter zurückgesetzt.
