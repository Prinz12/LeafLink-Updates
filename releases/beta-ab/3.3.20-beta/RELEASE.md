# LeafLink 3.3.20 Beta – IP-Konflikterkennung und Routername

- Erkennt über ARP, wenn ein anderes Gerät dieselbe IPv4-Adresse beansprucht. Nach Bezug einer Adresse erfolgen drei kurze Prüfungen; anschließend überwacht die Firmware empfangene ARP-Pakete.
- Meldet den Konflikt per DHCPDECLINE an den Router, gibt die Konfliktadresse auf und startet nach einer Wartezeit eine neue DHCP-Anfrage. Die Konfliktbehebung benötigt keinen Geräteneustart und keinen Wechsel des WLAN-Modus.
- Fehlgeschlagene Übertragungen, Speichermangel und ein vorübergehend nicht antwortender DHCP-Server werden mit begrenzten Wiederholungen behandelt. Diagnosezähler zeigen Konflikte und DHCP-Wiederanläufe an.
- Die Lüfter melden sich beim Router mit `Leaf-` plus Lüfternummer, beispielsweise **Leaf-6469**. Der **Einrichtungs-AP samt Name und Kopplungen bleibt unverändert**.
- Motorüberwachung und Sicherheitsfristen bleiben aktiv. Bei fehlender Gruppenbestätigung pausiert die Sommerautomatik sicher und kann nach Wiederherstellung wieder koordinieren.

**Android 3.3.21 und Wall 0.6.6 Beta bleiben kompatibel.** Dieselbe Firmware für Router und Repeater. Signiertes A/B-Update für Hardwaregeräte mit Layout 2; Einstellungen bleiben erhalten. Der normale geplante Neustart zur Installation des Updates bleibt erforderlich.

204 Firmware-Hosttests, 63 native Regressionstestprogramme, zusätzliche DHCP- und Wall-WLAN-Laufzeittests, 957 Kryptografieprüfungen, Protokoll-Kompatibilität, Android-Build/Lint und 24 Emulator-Oberflächenprüfungen bestanden. Hardwarebuild und Stackaudit bestanden; zusätzlicher fester RAM-Bedarf nur 128 Bytes.

Ein realer Lüfter wurde über das gekoppelte Handy datenbewahrend aktualisiert: genauer Imagehash, Slotwechsel, bestätigter Start, erhaltene Einstellungen und Hausplan sowie verschlüsselte Temperaturabfragen wurden geprüft. Die FRITZ!Box löst den neuen Gerätenamen erfolgreich auf. Ein zweiminütiger Paralleltest mit 76 authentifizierten Handy-Abfragerunden und 99 HTTP-Zustandsrunden blieb ohne Abfragefehler, zusätzlichen Neustart oder Motorfehler; auch die Bedienbestätigung mit unveränderten Sollwerten gelang. Dies ist kein Dauerlauf.

Ein echter Konflikt mit anschließendem DHCP-Adresswechsel auf einem aktualisierten Lüfter wurde noch nicht praktisch nachgewiesen. Die Veröffentlichung installiert keine Geräte automatisch. Der Router muss eine freie Adresse vergeben können; eine dauerhaft fehlerhafte feste Zuordnung muss im Router korrigiert werden. Über ARP nicht sichtbare Geräte können nicht erkannt werden.
