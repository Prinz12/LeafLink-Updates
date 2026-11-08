# Wall Control 0.6.4 Beta – Rollen unter Lüfter / Gruppen

Unter **Einstellungen → Lüfter / Gruppen** zeigt Wall Control jetzt die tatsächliche Netzwerkrolle jedes Lüfters. Beim Antippen erscheinen außerdem **Auto/Manuell** und bei Repeatern der unmittelbare Nachbar, zum Beispiel **Manuell / Repeater via 4811**. Die Web-Geräteverwaltung zeigt dieselben Angaben.

Die Anzeige verwendet authentifizierte Funkmeldungen und bei Bedarf die aktuelle Statusabfrage beim bekannten Gateway, keine Vermutung aus WLAN-Adresse oder Master/Slave. Meldungen älter als 30 Sekunden werden als „zuletzt“ gekennzeichnet; fehlende Daten bleiben unbekannt. Eine aktuelle Rollenmeldung über ein Gateway ist auch sichtbar, wenn die direkte Wall-Steuerverbindung noch unbestätigt ist. Routing und Lüftereinstellungen werden durch die Anzeige nicht verändert.

Fehlende Nextion-Bestätigungen für reine Text-/Farbzuweisungen werden begrenzt erneut angefordert. Bedienbefehle werden nicht wiederholt.

Datenerhaltendes Update für LILYGO T-Display ESP32 mit bestehendem 16-MiB-Layout. Inventar, Gruppen und Einstellungen bleiben erhalten. **Nextion HMI 302 ist unverändert; ein TFT-Update ist nicht erforderlich.** Die unveränderte TFT-Datei ist der Vollständigkeit halber beigefügt.

Für Anlagen mit geschütztem Funkprotokoll 2. Beim Wechsel von Wall 0.5.x gelten weiterhin die Migrationsschritte für 0.6.x. Aktuelle Rollenmeldungen wurden mit Lüfterfirmware 3.3.12 geprüft; bei sehr alter Firmware kann die Auto/Manuell-Angabe fehlen.
