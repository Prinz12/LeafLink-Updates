# LeafLink 3.3.58 Beta

Bei der automatischen WLAN-Rückkehr aus dem Gruppenersatzbetrieb haben WLAN-Anmeldung und IP-Adressvergabe jetzt eigene Fristen.

- Bereits beim ersten Versuch darf der DHCP-Client bis zu 65 Sekunden auf ein Adressangebot warten. Trifft das Angebot spät ein, erhält die anschließende Anforderung einmalig weitere 65 Sekunden für die Bestätigung durch den Server. Die Netzwerkbibliothek steuert ihre Wiederholungen selbst.
- Erhält der Lüfter eine gültige IP-Adresse, nimmt er den LAN-Betrieb sofort wieder auf. Ein erkannter Funkabbruch während DHCP beendet den jeweiligen Versuch vorzeitig.
- Die Suche und die Anmeldung an einem unerreichbaren Zugangspunkt bleiben kurz. Nach zwei Fehlversuchen sucht der Lüfter bis zu vier Sekunden und wartet bis zu 15 Sekunden auf die Anmeldung.
- Während der Wartezeit laufen die lokalen Motorphasen weiter. Gruppenpakete können beim Wechsel auf den Routerkanal ausbleiben. Die Status-API zeigt, ob ein DHCP-Angebot oder dessen Bestätigung fehlt.

Das signierte Paket ist für ESP8266-Lüfter mit 4 MiB Flash und A/B-Layout 2 bestimmt. In der App unter Firmwareupdate „Beta-Versionen anzeigen“ aktivieren und „Version prüfen“ wählen.
