# LeafLink Firmware 3.3.16 Beta

Firmwareupdates sind mit Android 3.3.17 direkt in der Repeaterrolle über ein Lüfter-Gateway möglich. Der Repeater braucht dafür keine direkte Routerverbindung; die Wall kann ausgeschaltet bleiben. Datenblöcke werden bestätigt und bei verlorenen Antworten wiederholt. Erst nach erfolgreicher Signatur- und Imageprüfung wird der neue A/B-Slot gestartet und geprüft.

Das Gateway wiederholt verlorene Funkpakete selbst. Eine funktionierende Repeaterverbindung wird nicht mehr für die Suche nach einer ausgeschalteten Wall unterbrochen. Während des Updates pausiert der zu aktualisierende Lüfter; anschließend startet er mit seinen gespeicherten Einstellungen.

Die neue Empfangsfunktion muss einmalig auf dem Lüfter vorhanden sein: Geräte mit älterer Firmware zunächst über USB oder eine direkte WLAN-Verbindung auf 3.3.16 aktualisieren. Danach ist der Funk-Updatepfad verfügbar. Router und Repeater verwenden dieselbe Firmwaredatei.

Die Weboberfläche zeigt Gruppennamen aus dem synchronisierten Hausplan. Fehlende oder ungültige Sensormessungen erscheinen als „Noch kein gültiger Messwert“ statt als 0 °C / 0 %. Die phasenabhängige Sensormessung bleibt erhalten.

WLAN-Repeater verwenden ein erreichbares Lüfter-Gateway auch bei ausgeschalteter Wall. Die gespeicherte Wall-Kopplung erzwingt nur im ausdrücklich gewählten reinen Wall-Funkbetrieb eine Bindung an diese Zentrale.

Die schnelle Geräteerkennung fragt auch Repeater über ihre eigene Geräteidentität und LAN-Aliasadresse ab.

Die Gateway-Weiterleitung bleibt jetzt auch dann aktiv, wenn mDNS-Geräteankündigungen wegen hoher App-Last pausieren oder fehlschlagen. LAN-Adressen und ARP-Antworten bleiben verfügbar; erneute mDNS-Anmeldungen erfolgen begrenzt und unabhängig davon.

Die A/B-Startprüfung berücksichtigt Repeater mit initialisiertem, verfügbarem Funkpfad. Gesunder Lauf, externe Startbestätigung und dauerhafte Speicherung bleiben erforderlich. Die LAN-Aliasadresse bleibt über Neustarts erhalten; Journal v15 übernimmt vorhandene Einstellungen. Ältere Repeater beziehen ihre Adresse einmalig über das gespeicherte WLAN.

Gespeicherte Netzwerkrolle, Gruppe, WLAN-Daten und manuelle Richtung bleiben erhalten. Automatische IN/OUT-Paare benötigen zwei gegenseitig erreichbare Gruppenmitglieder. Für aktuelle Anzeigen Android 3.3.17 verwenden.

Signiertes Hardwareprofil für ESP8266/ESP-12F mit 4 MiB und vorhandenem A/B-Layout 2.

Öffentliche Statusantworten eines Repeaters erreichen die App im richtigen Format. Interne Lüfterkommunikation und authentifizierte Steuerbefehle bleiben geschützt.

Realer Test mit zwei Lüftern und Android-Emulator bei ausgeschalteter Wall: vollständiges Update in 5:43 Minuten, Wiederholung mit 72 gezielt verlorenen Antworten in 7:19 Minuten. Signaturprüfung, Neustart, dauerhafte Slot-Bestätigung sowie Erhalt von Einstellungen und Hausplan bestanden. Dies sind Messwerte dieser Funkstrecke, keine allgemeine Zeitgarantie.
