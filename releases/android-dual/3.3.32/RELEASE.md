# LeafLink Android 3.3.32 – Automatische VPN-Suche nach IP-Wechseln

Bekannte Lüfter werden bei geöffneter App auch dann im bisherigen Heimnetz
wiedergefunden, wenn sämtliche gespeicherten IP-Adressen gewechselt haben.
Eine neue IP muss dafür nicht manuell eingegeben werden. Die Suche läuft
abschnittsweise, mit höchstens 64 Zielen je 15 Sekunden. In einem üblichen
Heimnetz dauert ein Durchlauf etwa eine Minute; Verluste können ihn verlängern.

Es werden nur zuvor bekannte Geräteidentitäten übernommen und ausschließlich
private /24-Bereiche bereits gespeicherter Adressen geprüft, höchstens vier
Bereiche. Ein völlig unbekannter neuer Netzbereich kann nicht erraten werden.
Das VPN muss den Zugriff ins Heimnetz erlauben. Geräteübersichten werden
regelmäßig unabhängig von der geöffneten App-Seite erneut geladen.

Direkt bestätigte neue Adressen ersetzen alte Einträge desselben Lüfters automatisch.
Alte Einträge ohne Gerätezuordnung werden erst nach drei erfolglosen Prüfungen
entfernt, wenn alle bekannten Lüfter wieder erreichbar sind. Ein zeitweilig
ausgeschalteter Lüfter verliert dadurch weder Zuordnung noch Kopplung.
Manuell gelöschte Adressen bleiben ausgeschlossen. Räume, Hausplan und Kopplungen
bleiben erhalten; geschützte Steuerbefehle verwenden unverändert ihre Anmeldung.

Als App-Update installieren, nicht deinstallieren. Paket de.prinz.leaflink,
Versionscode 41, Android 6.0 oder neuer. Für diese Korrektur ist kein zusätzliches
Firmware- oder Wall-Update nötig. Die Anforderungen des Sicherheitsupdates
ab App 3.3.27 / Firmware 3.3.25 / Wall 0.6.8 gelten weiterhin.

Geprüft: sechs gleichzeitig geänderte Adressen ohne erreichbare alte Adresse
oder Geräteliste, automatische Bereinigung, Offline-Schutz, manuelle Ausschlüsse,
Netzwechsel und verspätete Antworten; Host- und isolierte Emulatorprüfungen,
Android-Build/Lint und Firmware-/Protokoll-Kompatibilität. Installation durch
den Nutzer; keine Testinstallation auf dem Nutzerhandy.
