# LeafLink 3.3.24 Beta – App-Anmeldung auf der Serviceseite

Die über die gekoppelte App freigegebene Webanmeldung bleibt beim Wechsel zu
**Service & Diagnose** erhalten. Wiederhergestellte Browserseiten verwenden den
aktuellen Anmeldezähler. Eine durch frühen Seitenwechsel oder Neuladen unterbrochene
Anmeldung wird innerhalb ihrer kurzen Gültigkeit im selben Tab fortgesetzt.
Während der App-Anmeldung erscheint keine zusätzliche Gerätecodeabfrage.

Direkte Webaufrufe ohne Anmeldung bleiben geschützt. Signaturprüfung, Replay-Schutz,
IP-Bindung, Ablaufzeiten und Abmeldung bleiben erhalten. Ein Geräte-Neustart beendet
die Browsersitzung weiterhin. Danach die Webseite erneut aus der App öffnen.

In der App Beta-Versionen anzeigen und Firmware 3.3.24 Beta auswählen. Anschließend
die Webseite aus der gekoppelten App neu öffnen. Android 3.3.26 und Wall 0.6.7 bleiben
kompatibel; dafür ist kein zusätzlicher App- oder Wall-Download nötig.

Die adaptive Sommermessung und der geschützte Fernneustart aus den vorherigen
Versionen bleiben enthalten. Ein Neustart garantiert weiterhin keine neue IP-Adresse.

Geprüft mit Produktions-Webseiten im Desktop- und Mobilformat: Service starten und
beenden, wiederhergestellter Zählerstand, verzögerte Anmeldung mit Seitenwechsel,
Neuladen, abgelaufene Freigabe, falscher Code, Replay und Abmeldung. Zusätzlich
Firmware-Host-/Native-Tests, Hardware-Build/Stackprüfung, Protokoll- und
Kryptografieprüfungen sowie Android-Hosttests, Build, Lint und Emulatorprüfungen.

Signiertes Hardware-A/B-Image, Layout 2. Installation durch den Nutzer; kein
Flashen durch den Assistenten und kein Test auf dem betroffenen Nutzerhandy.
