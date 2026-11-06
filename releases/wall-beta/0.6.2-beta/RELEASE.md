# Wall Control 0.6.2 Beta – schnellere Netzwechsel und bestätigte Bedienung

Die Wall wartet beim Netzwechsel nur auf kürzlich erreichbare Lüfter. Ausgeschaltete Inventareinträge bleiben gespeichert und unbestätigt. Sobald WLAN verbunden ist, startet die geschützte Kommunikation ohne zusätzliche feste Wartezeit. Die zuletzt bekannte WLAN-Adresse bleibt als Suchhinweis erhalten; eine frische Geräteidentität wird weiterhin geprüft.

Der Empfangsschutz berücksichtigt unterschiedliche Reihenfolgen von LAN- und Funkpaketen. Eine fehlende WLAN-Befehlsbestätigung führt zu höchstens zwei begrenzten Wiederholungen desselben Sollzustands. Erfolg wird erst mit passender Bestätigung und Istzustand gemeldet. Die erste Stufenwahl bleibt erhalten, während die Stufenwerte des Gruppenmasters gelesen werden.

Zusammen mit Lüfter-Firmware 3.3.6 wurden zwei vollständige Wechsel mit realen Geräten geprüft: 18,5 Sekunden in den Direktfunk sowie 25,1 und 33,4 Sekunden zurück ins WLAN statt zuvor über 100 Sekunden. Anschließend blieben beide Lüfter bei frischen Statusabfragen stabil erreichbar. Diese Zeiten sind Messwerte und keine Garantie für jede Netzwerkumgebung.

Vorhandenes Inventar, Gruppen, Einstellungen und Wall-Zuordnungen bleiben erhalten. Für die vollständige Korrektur beide Seiten aktualisieren: Wall 0.6.2 und Lüfter-Firmware 3.3.6. Die Android-App bleibt bei 3.3.4.

Wichtig beim Wechsel von Wall 0.5.x: Version 0.6.x verwendet das geschützte Funkprotokoll 2 mit eigenständigem Wall-Funkzugang. Den Wall-Funknetzcode über „Wall-Funknetz übernehmen“ in die App importieren und die Lüfter mit physischer Freigabe koppeln. Die bisherige ungeschützte Funkverbindung wird nicht weiterverwendet. Bereits auf 0.6.x migrierte Anlagen behalten ihre Zuordnung ohne erneute Kopplung.

Hardware: LILYGO T-Display ESP32 mit bestehendem 16-MiB-Layout. Die BIN ist für den regulären datenerhaltenden App-Slot-Updateweg, kein Vollflash. Nextion HMI 302 bleibt unverändert; ein TFT-Update ist nicht erforderlich. Die unveränderte TFT-Datei ist nur der Vollständigkeit halber beigefügt.
