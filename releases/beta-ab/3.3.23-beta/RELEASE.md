# LeafLink 3.3.23 Beta – Geschützter Fernneustart

Nach Anmeldung die Lüfter-Weboberfläche öffnen: **Service & Diagnose →
Servicemodus starten → Neutral neu starten**. Ab dieser Firmware ist für den
Neustart kein Tastendruck direkt am Lüfter erforderlich.

Die aktive Servicesitzung und geschützte Anmeldung bleiben erforderlich.
Ein laufendes Firmwareupdate, eine bereits geplante Wartungsaktion oder eine
fehlgeschlagene Neutralbestätigung des Motorausgangs verhindern den Neustart.
Eine wiederholte Anforderung verschiebt den bereits geplanten Neustart nicht.
Einstellungen und Kopplungen bleiben erhalten. Werkseinstellungen, WLAN-Löschen,
WLAN-Wechsel und nicht-neutrale Motortests verlangen weiterhin die Bestätigung
am Gerät.

**Ein Neustart garantiert keine neue DHCP-Adresse.** Eine doppelte IP-Zuordnung
zwischen VPN-Handy und Lüfter muss weiterhin im Router behoben werden. Die neue
Funktion steht erst nach Installation dieser Firmware zur Verfügung; sie kann
keine ältere Firmware aus der Ferne neu starten.

Die optionale adaptive Sommermessung aus 3.3.22 bleibt enthalten. Für eine Gruppe
mit adaptiver Messung müssen alle Gruppenlüfter mindestens 3.3.22 verwenden.
Wall 0.6.7 bleibt kompatibel und benötigt für diesen Release kein Update.

Signiertes Hardware-A/B-Image, Layout 2. In der App Beta-Versionen anzeigen,
Firmware 3.3.23 Beta auswählen. Installation durch den Nutzer; kein Flashen
durch den Assistenten und kein physischer Neustarttest dieses Builds.

Prüfung: Firmware-Host-/Native-Tests, Neustart- und Autorisierungsregression,
Hardware-Build/Stackprüfung, Protokoll-Interoperabilität, Signatur und Vergleich
der öffentlich heruntergeladenen Release-Dateien.
