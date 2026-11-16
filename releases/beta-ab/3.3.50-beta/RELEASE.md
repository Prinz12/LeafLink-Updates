# LeafLink 3.3.50 Beta – Netzprüfung und Speicherreserven

- Begrenzte ausstehende Funkaufträge entlasten den WLAN-Sendepfad. Überlast
  wird gezählt; eine fehlende Sendebestätigung gibt keinen falschen freien Platz.
- Kleine Netzwerkantwort für App 3.3.53 statt vollständiger Gerätediagnose.
- Seltenere Heap-Komplettscans und neue abgetastete Speicher-Minima.
- Fehlende Speicherreserve bei der Mesh-Schlüsselableitung wird abgefangen.

Zuerst **App 3.3.53** installieren, anschließend die Lüfter aktualisieren.
Dieses signierte Image gilt für ESP8266/ESP12F mit 4 MB, Hardwareprofil und
vorhandenem **A/B-Layout 2**. Kopplungen, Einstellungen und Hausplan bleiben erhalten.

Die Änderungen adressieren Last- und Speicherpfade nach zwei beobachteten
WLAN-SDK-Watchdogs. Ein kurzer erfolgreicher Belastungstest garantiert keine
dauerhafte Fehlerfreiheit; die Firmware bleibt im Beta-Kanal.

Geprüft auf dem angeschlossenen Tablet: sechs Netzprüfungen, danach eine weitere
nach Aktualisierung eines zusätzlich betroffenen Geräts. Insgesamt 838/840
Antworten; die aktualisierten Geräte beantworteten ihre jeweiligen Prüfpakete
vollständig und zeigten keinen zusätzlichen Neustart. Zwei Antworten fehlten
bei Repeatern mit älterer Firmware. Speicher- und Queuegrenzen bleiben sichtbar.
Automatisierte Firmware-, Protokoll-, Android- und Emulatorprüfungen bestanden.
