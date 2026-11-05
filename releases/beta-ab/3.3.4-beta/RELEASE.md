# LeafLink 3.3.4 Beta

Die Suche nach einer zugeordneten Wall unterbricht eine bestehende WLAN-Verbindung nicht mehr. Die vorhandene Wall-Zuordnung, Funk- und WLAN-Zugangsdaten bleiben erhalten. Authentifizierte Wall-Befehle über das LAN bleiben möglich; die Funksuche wird nur bei tatsächlich getrenntem WLAN verwendet.

Die Weboberfläche lässt sich wieder geschützt bedienen. Mit App 3.3.3 öffnet **Einstellungen → verbundene Geräte → WEB** die Seite über die vorhandene Handykopplung ohne erneute Codeeingabe. Die einmalige Freigabe verfällt nach 30 Sekunden. Wer die Adresse direkt eingibt, kann weiterhin den Gerätecode nutzen und optional einen Sitzungsschlüssel bis zu sieben Tage auf dem eigenen Browser merken. Nach einem Geräteneustart erneut aus der App öffnen oder anmelden.

Keine Rückkehr zu ungeschützter Steuerung: Befehle sind authentifiziert und gegen Wiederholung geschützt. Signatur-, Versions-, Speicher- und Motorschutz der OTA-Updates bleiben erhalten. Die kompakte Web-Routenverwaltung spart Arbeitsspeicher. Vor OTA werden zudem nur bereits geschlossene TCP-Verbindungen freigegeben.

Voraussetzungen: ESP8266 ESP-12F, 4 MiB Flash, Hardwareprofil und A/B-Layout 2. Nur die signierte BIN verwenden. Das App-Update allein installiert keine Lüfterfirmware. Historische Safe-Versionen bleiben unverändert; diese Version bietet ausschließlich das Hardwareprofil.

Die Weboberfläche verwendet weiterhin lokales HTTP. Die Anmeldung ersetzt keine TLS-Verschlüsselung und schützt nicht vor einer aktiv manipulierten Webseite im Netzwerk. WLAN-Zugangsdaten werden deshalb weiterhin ausschließlich über die verschlüsselte App-Einrichtung geändert.
