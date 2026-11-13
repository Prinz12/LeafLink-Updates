# LeafLink Android 3.3.42 – Lebensdauer und Nutzung bei Repeatern

„Lebensdauer & Nutzung“ liest die Statistik jetzt auch über die verschlüsselte
Repeater-Verbindung. Dazu benötigt der betreffende Lüfter Firmware 3.3.36.
Die App prüft Gerätekennung und Datenformat und wiederholt eine verlorene
Leseantwort einmal. Bei Verbindungswechseln oder fehlenden Antworten bleiben
die letzten gespeicherten Werte als alter Abruf erkennbar.

Zuerst diese App aktualisieren, danach die betroffenen Repeater auf
Firmware 3.3.36 Beta. Ältere direkt erreichbare WLAN-Lüfter behalten ihren
bisherigen Statistikabruf. Als Update ohne Deinstallation installieren;
Kopplungen und Einstellungen bleiben erhalten.

App-Build, Lint und sämtliche Android-Hosttests bestanden. Der Emulator prüft
den vom Firmwarecode erzeugten Datensatz, falsche Gerätekennungen, beschädigte
Daten, Navigation und Offlinecache. Physische Repeaterprüfung noch ausstehend.
