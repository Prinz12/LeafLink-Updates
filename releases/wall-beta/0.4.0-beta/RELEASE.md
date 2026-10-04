# Leaf Wall Control 0.4.0 Beta / HMI 302

Direktfunk-Zentrale für LILYGO T-Display V1.1 (ESP32, 16 MiB Flash) mit Nextion
NX4827K043_011 (480 × 272). Das interne LILYGO-Display bleibt ausgeschaltet.

Einstellungen → Leaf-Funknetz → Ohne WLAN-Router aktiviert die authentifizierte
ESP-NOW-Zentrale. Passend eingerichtete LeafLink-Lüfter ab 3.2.1 übernehmen ihre
vorhandenen Gruppen. Status, Leistung, Betriebsart und Gruppenwechsel funktionieren
ohne Heim-WLAN. Die Rolle bleibt nach Neustart erhalten.

Der Service-AP bleibt normalerweise aus. Software / Web → Zugangspunkt aktiviert
ihn ausdrücklich für zehn Minuten für Webbedienung und Datei-Updates. Rückkehr
zum Heim-WLAN: Funk-Einrichtung → Automatik / Heim-WLAN.

## Dateien installieren

Für bereits eingerichtete Geräte: In der authentifizierten Weboberfläche zunächst
`manifest.json`, dann `leaf-wall-control-0.4.0.bin` auswählen und installieren.
Die zu HMI 302 gehörende `leaf-wall-control-0.3.0.tft` ist unverändert und muss bei
bereits vorhandenem HMI 302 nicht erneut übertragen werden. Andernfalls nach dem
ESP32-Update das TFT mit demselben Manifest installieren.

Die BIN-Datei ist nur ein App-Update, kein Flash-Abbild für Erstinstallationen.
Nicht für andere Flashgrößen, Boards oder Displaymodelle verwenden. Manifest und
SHA-256 schützen die Dateiintegrität; dieses ESP32-Paket besitzt noch keine
Herausgebersignatur. Nextion hat keinen A/B-Rollback; unterbrochene TFT-Übertragungen
benötigen den USB-/microSD-Serviceweg.

## Prüfung und Grenzen

37 Controller-Prüfungen sowie 17 Prüfungen von Wurzelwahl, Routing und Transport
bestanden. 13 Live-Prüfungen mit fünf motorlosen Lüftern und drei Gruppen bestanden,
einschließlich Neustart, Kaltstart-Gruppenwechsel und explizitem Service-AP.
Firmware 3.2.1 Beta ist in getrennten Hardware-/Safe-Kanälen verfügbar.
Funkkennung und Schlüssel müssen übereinstimmen; fabrikneue Geräte werden nicht
unbeaufsichtigt gekoppelt. Kein NAT-/WLAN-Repeater. Lüfter-OTA erfordert weiterhin
Heim-WLAN. Die Uhrzeitsynchronisierung benötigt eine Zeitquelle; ohne gültige Uhr
bleibt ein eingestellter Darkmode-Zeitplan dunkel.
