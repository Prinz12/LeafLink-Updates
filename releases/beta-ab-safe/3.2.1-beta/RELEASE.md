# LeafLink Firmware 3.2.1 Beta – Direktfunk mit Wandbediengerät

Das Wandbediengerät kann die Lüfter ohne Heim-WLAN-Router über authentifizierten
ESP-NOW-Direktfunk steuern. Voraussetzung ist Wall Control 0.4.0 mit passender
Funkkennung und passendem Schlüssel. Bestehende Lüftungsgruppen, Raumzuordnungen
und Einstellungen bleiben erhalten.

- Die Bindung an das Bediengerät und den Funkkanal bleibt nach Stromausfall erhalten.
- Status, Gruppenbedienung und Gruppenwechsel funktionieren auch nach Kaltstart
  ohne DHCP-Adresse; Befehle werden durch Quittung und passenden Zustand bestätigt.
- Die Rückkehr zu Automatik/Heim-WLAN löst die Bindung. Bei längerem Verlust der
  Zentrale greift die begrenzte Wiederherstellung über das gespeicherte WLAN.
- Funknachrichten werden in der Hauptschleife verarbeitet; reduzierte Stacklast
  und vor OTA freigegebene Empfangspuffer verbessern die Zuverlässigkeit.

## Zielgeräte und Installation

Nur für bestehende LeafLink-Geräte mit ESP8266 ESP-12F, 4 MiB Flash, A/B-Layout 2
und dem unten genannten Profil. Kein vollständiges Flash-Abbild; nicht ab Adresse 0
schreiben. Originalfirmware und HAPLA sind nicht kompatibel. Lüfterupdates erfolgen
im Heim-WLAN; ein Update der Lüfter über die reine Direktfunkstrecke ist nicht enthalten.
Fabrikneue Geräte und unabhängig eingerichtete Funkpaare werden nicht automatisch gekoppelt.

Journal v11 übernimmt bestehende Konfigurationen. Die Direktfunkbindung ist ein
neuer Datensatz; ältere Firmware kennt sie nicht. Kein Firmware-Downgrade im
gebundenen Direktfunkbetrieb: zuerst zu Automatik/Heim-WLAN zurückkehren.

## Prüfung

196 Firmware-Hosttests, 33 native Testprogramme, Codec-Interoperabilität und
Hardware-/Safe-Builds bestanden. Fünf motorlose Prüfgeräte wurden mit exakt diesen
signierten Images geprüft: alle drei Gruppen bedienen, Panel-Neustart, Lüfter-
Kaltstart, Gruppenwechsel und Service-AP. 13 Live-Prüfungen bestanden; ursprüngliche
Gruppen und Betriebswerte wurden wiederhergestellt. Dies ist kein Motor-/Luftmengentest.

`version.json` enthält Größe, SHA-256, Profil, Layout und Downloadlink.
Die RSA-Signatur wurde gegen den bestehenden LeafLink-Vertrauensschlüssel geprüft.

Profil: **Safe – deaktivierte Hardware-Ausgänge.**
