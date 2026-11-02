# LeafLink 3.2.8 Beta – gemeinsame Netzauswahl durch Wall Control

Mit Wall Control 0.5.10 folgen eingerichtete Lüfter der dort gespeicherten
Auswahl: alle direkt oder alle im gespeicherten WLAN. Jeder Abgleich ist
verschlüsselt und an die bestehende Kopplung sowie eine frische Sitzung gebunden.
Eine angenommene Umschaltung ist noch keine Bestätigung des aktiven Netzes.

Ein beim Wechsel ausgeschalteter Lüfter holt die Auswahl nach seiner Rückkehr
nach. Ein Lüfter im WLAN sucht bei ausbleibendem Controllerkontakt zeitweise
im privaten Funknetz nach der Zentrale. Ohne Antwort kehrt er zum gespeicherten
WLAN zurück und verlängert das Suchintervall. WLAN-Daten, Gruppen und Kopplung
werden dabei nicht gelöscht. Dauerhafte Einstellungen werden nur bei Änderungen
geschrieben. Während eines Updates oder unbestätigten A/B-Starts ist die
automatische Umschaltung gesperrt.

Enthält die WLAN-Speicherkorrektur aus 3.2.7. Bestehendes 4-MiB-A/B-Layout 2,
Signaturprüfung, Startbestätigung, Rückfall und regulärer OTA-Weg bleiben erhalten.
Signiertes Anwendungsupdate, kein Vollflash. Hardware- und Safe-Profil beachten.
Für die neue automatische Netzauswahl müssen Wall Control und alle betroffenen
Lüfter aktualisiert sein. Ältere oder unerreichbare Geräte bleiben unbestätigt.

Profil: **hardware**.

Bei WLAN-Ausfall bleibt die private Wall-Verbindung fuer den Netzabgleich erhalten. Gespeicherte Gruppenpartner leiten gekoppelte Luefter nicht mehr in ein separates Gruppen-Funknetz um.

Ein direkt gestarteter Luefter kann einen verpassten WLAN-Wechsel nachholen: Die Kanalsuche passt auch den internen Funkzugangspunkt an. Zum bereits im WLAN befindlichen, direkt erreichbaren gekoppelten Controller gibt es einen authentifizierten Broadcast-Rueckweg ohne Weiterleitung. Die verschluesselte Netzsitzung und die tatsaechliche WLAN-Bestaetigung bleiben erforderlich.
