# LeafLink Android 3.3.5 – WLAN-Rückkehr und zuverlässige Bedienung

Nach „Gespeichertes WLAN beibehalten“ wartet die App auf die bestätigte Rückkehr
des gekoppelten Lüfters ins Heim-WLAN. Sie prüft neben WLAN-Rundrufen auch bereits
bekannte Geräteadressen im aktuellen Netz. Dadurch funktioniert die Wiedererkennung
auch dann, wenn der Router Rundrufe nicht weiterleitet. Die Gerätekennung muss
weiterhin genau passen; die vorhandene Lüftungsgruppe bleibt erhalten.

Eine verlorene erste Antwort im Einrichtungs-WLAN wird durch begrenzte Wiederholung
der lesenden Geräteabfrage abgefangen. Eine unterbrochene Einrichtung kann die
Suche fortsetzen, ohne Kopplung oder WLAN-Daten erneut zu senden.

Bedienbefehle werden vor wartenden Hintergrundabfragen ausgeführt. Überholte
Abfragen werden zusammengefasst, veraltete Befehle nach einem Netzwechsel
verworfen. Die App fragt gruppenweite Messwerte nur bei Geräten ab, die diese
beantworten. Geschützte Gerätebestätigungen bleiben erforderlich.

Für die vollständige Korrektur nach der Kopplung auch die Lüfter auf **3.3.7 Beta**
aktualisieren. Das App-Update allein installiert keine Lüfterfirmware.
Vorhandene Kopplungen, Hauspläne und Einstellungen bleiben erhalten. Android-Paket
und Release-Signatur bleiben gleich; HAPLA wird weiterhin unterstützt.

Geprüft mit Android-Hosttests, Emulator und zwei realen Lüftern: Stufe 2 und die
Rückkehr zu Stufe 1 wurden auf beiden Geräten bestätigt. Die Messwerte gelten für
den Testaufbau und sind keine garantierte Reaktionszeit.
