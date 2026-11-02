# Wall Control 0.5.10 Beta – alle Lüfter im gewählten Netz

Am Display unter Einstellungen → Leaf-Funknetz und im Web unter WLAN und
Leaf-Funknetz gilt eine gemeinsame Auswahl: „Alle direkt mit Wall Control“
oder „Alle im gespeicherten WLAN“. Die Auswahl wird dauerhaft gespeichert.
Jeder eingerichtete Lüfter wird regelmäßig abgeglichen; ausgeschaltete Geräte
holen den Wechsel nach ihrer Rückkehr nach. Entfernte Lüfter bleiben ausgeschlossen.

Für WLAN werden bei Bedarf die in Wall Control gespeicherten Zugangsdaten
verschlüsselt übertragen und am Lüfter geprüft. Erneute Kennworteingabe ist
nicht erforderlich. Gruppen und Kopplung bleiben erhalten. Die Anzeige nennt
die Zahl der tatsächlich bestätigten Geräte und je Lüfter einen ausstehenden
Wechsel oder fehlende Erreichbarkeit. Bloßes Senden zählt nicht als Erfolg.

Das Einrichten neuer WLAN-Daten ändert die gewählte Direktbetriebsart nicht
mehr nebenbei. Die ausdrückliche WLAN-Weitergabe bleibt zusätzlich verfügbar.
Voraussetzung für den automatischen Abgleich: LeafLink 3.2.8 auf den Lüftern.

ESP32 LILYGO T-Display, bestehendes 16-MiB-Layout. App-BIN für den regulären
Updateweg, kein Vollflash. Nextion HMI 302 bleibt kompatibel, kein TFT-Update.
Die Korrektur gegen blockierende Upload-Abbrüche aus 0.5.9 ist enthalten.

Nach einem Netzwechsel prueft Wall Control die bisherige LAN-Adresse gezielt neu. Eine aktuelle WLAN-Identitaet ersetzt einen veralteten Funkweg; dadurch bleibt ein bereits zurueckgekehrter Luefter nicht wegen des alten Transportwegs als offline markiert.

Beim Wechsel ins WLAN wird die gespeicherte Auswahl erreichbarer Luefter zuerst ueber den noch aktiven Direktfunk bestaetigt. Erst danach wechselt Wall Control seinen eigenen Kanal und prueft die tatsaechliche WLAN-Verbindung.
