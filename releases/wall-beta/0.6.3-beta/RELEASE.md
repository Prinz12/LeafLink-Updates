# Wall Control 0.6.3 Beta – Router- und Repeaterrolle bleiben gespeichert

Behebt einen Fehler, durch den Wall Control nach einem Neustart die Rollen „Repeater“ und „Automatisch“ durch „Router“ ersetzen konnte. Die vollständige Zielrolle wird jetzt vor der Netzübergabe dauerhaft gespeichert und auch nach einer unterbrochenen Übergabe wieder aufgenommen. Vorhandene Einstellungen werden übernommen; ein Speicherfehler startet keinen Rollenwechsel.

Router, Repeater über einen Lüfter als Gateway, Automatik und der Erhalt der Rollen nach Neustarts wurden an einer realen Wall Control geprüft. Mit zwei Lüftern auf Firmware 3.3.11 wurde außerdem der bestätigte Wechsel in den Direktfunk und zurück ins WLAN geprüft. Inventar, Gruppen und Lüftereinstellungen bleiben erhalten.

Dieses Update betrifft Wall Control. Es ergänzt keine signalabhängige automatische Repeaterumschaltung in der Lüfterfirmware. Für diese Wall-Korrektur ist kein zusätzliches Android- oder Lüfter-Update erforderlich, wenn die Anlage bereits mit dem geschützten Funkprotokoll 2 betrieben wird.

Hardware: LILYGO T-Display ESP32 mit bestehendem 16-MiB-Layout. Die BIN ist für den regulären datenerhaltenden App-Slot-Updateweg, kein Vollflash. Nextion HMI 302 bleibt unverändert; ein TFT-Update ist nicht erforderlich. Die unveränderte TFT-Datei ist der Vollständigkeit halber beigefügt.

Beim Wechsel von Wall 0.5.x gelten weiterhin die Migrationsschritte für das geschützte Funkprotokoll 2: Wall-Funknetz in der App übernehmen und Lüfter mit physischer Freigabe koppeln. Bereits auf 0.6.x migrierte Anlagen benötigen keine erneute Kopplung.
