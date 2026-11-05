# LeafLink Android 3.3.4

Behebt verfrühte Meldungen „Keine vollständige Rückmeldung“ bei der Gruppensteuerung.

Die App wartet jetzt auf die zum aktuellen Befehl gehörenden Bestätigungen aller angesprochenen Lüfter. Bei LeafLink zählen nur authentifizierte Antworten mit passender Befehlskennung und passendem Zustand. Ein alter gespeicherter Status reicht nicht mehr aus. Fehlende Antworten werden weiterhin als Fehler angezeigt.

Steuerbefehle werden in ihrer Reihenfolge gesendet. Geschützte Anmeldungen halten den Mindestabstand der Firmware ein; dadurch entfallen unnötige Wartezeiten durch deren Schutzbegrenzung.

Auf dem angeschlossenen Handy mit zwei echten Platinen geprüft: fünf Gruppen-Stufenwechsel, beide Geräte jeweils innerhalb einer Sekunde im angeforderten Zustand, fünf bestätigte App-Rückmeldungen. Die ursprüngliche Lüfterstufe wurde danach wiederhergestellt.

Vorhandene Kopplungen, Einstellungen und Hauspläne bleiben erhalten. Die automatische Web-Anmeldung aus App 3.3.3 bleibt enthalten. Für diese Korrektur ist kein neues Firmwareupdate erforderlich; der Hardwaretest erfolgte mit Firmware 3.3.4 Beta. Android-Paket und Signatur bleiben unverändert.
