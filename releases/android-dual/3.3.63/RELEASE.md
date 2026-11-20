# LeafLink Android 3.3.63 – Updatefolge bei Gerätefehlern fortsetzen

Nach einer abgeschlossenen Updatefolge können gespeicherte Fehlversuche direkt geprüft oder abgeschlossen werden. Der vorherige Klick auf „GERÄTE PRÜFEN“ entfällt dafür. Die individuelle Prüfung liest weiterhin den betroffenen Lüfter frisch und prüft Identität, Zustand und Stabilität. Während einer laufenden Folge bleiben diese Aktionen gesperrt.

Ein Fehler bei einem einzelnen Lüfter wird dokumentiert; die übrigen ausgewählten Lüfter werden nacheinander weiter aktualisiert. Fehlgeschlagene Uploads werden nicht automatisch wiederholt. Offene Updateprotokolle bleiben erhalten. Der Gesamtstatus meldet ausdrücklich einen Abschluss mit Fehlern statt vollständigen Erfolg.

Gemeinsame Probleme wie WLAN-/VPN-Verlust oder -Wechsel, ungültige Updatepakete und nicht speicherbare Updateprotokolle stoppen weiterhin die Folge. Ein ausdrücklicher Stopp bleibt wirksam. Neue Uploads erfordern weiterhin Auswahl und Bestätigung.

Als Update über die vorhandene App installieren, nicht deinstallieren. Nur die App wird für diese Korrektur aktualisiert; Firmware und Wall bleiben unverändert. Keine Installation auf Nutzergeräten und keine tatsächlichen Geräteupdates durch die Tests.

Release-Build, Lint, Hosttests sowie Emulatorprüfungen der produktiven Updatefolge, der direkten Abschlussprüfung, des Journals und der Bedienung bestanden. Die Prüfung verwendet signierte Testpakete und simulierte Geräte. Der bereits dokumentierte historische 2.0.0-Migrationstest bleibt wegen seiner ungültigen alten Signaturfixture ausgeschlossen; die Signaturprüfung wurde nicht geändert.
