# LeafLink Android 3.3.45 – Weiteres Bediengerät hinzufügen

Ein bereits gekoppeltes Handy kann einem weiteren Handy oder Tablet eigene
Lüfterzugänge freigeben. In den Einstellungen **Weiteres Bediengerät hinzufügen**
wählen, den Freigabe-QR anzeigen und auf dem zweiten Gerät **Freigabe übernehmen**
wählen. Beide Apps während der Übertragung im selben Heim-WLAN geöffnet lassen.

- Die vorhandenen Kopplungen bleiben erhalten. Das neue Gerät erhält eigene,
  separat widerrufbare Zugänge; bestehende Controller-Schlüssel werden nicht kopiert.
- Die Übertragung erfolgt lokal und verschlüsselt. Jeder freigegebene Lüfter
  wird vom Empfänger mit seinem neuen Zugang geprüft.
- Nach einem Abbruch kann die Freigabe wiederholt werden. Bereits bestätigte
  Zugänge bleiben erhalten. Ausgeschaltete Lüfter später einschalten, aktualisieren
  und durch eine erneute Freigabe ergänzen.
- Ohne gespeicherte Lüfter erklärt eine kurze Startanleitung die erste Einrichtung
  mit Tastendruck und QR-/Gerätecode. Die Anleitung ist in zehn Sprachen verfügbar.

**Voraussetzungen:** Android 9 oder neuer, App 3.3.45 auf beiden Bediengeräten
und Firmware 3.3.43 Beta auf den freizugebenden Lüftern. Die App verwendet
weiterhin Android 16 als Zielversion. Zuerst die App, danach die Lüfter aktualisieren;
für die Firmware den Beta-Kanal aktivieren. Pro Lüfter sind acht Zugänge möglich.

Die Freigabe unterstützt erreichbare LeafLink-Lüfter; HAPLA-Zugänge und
Wall-Einrichtungsfreigaben werden nicht übertragen. Die bestehende
Hausplan-Synchronisierung bleibt ein eigener Vorgang.

Die Übertragung und ihre Wiederholung wurden zwischen Samsung-Handy und
Samsung-Tablet mit zehn eingeschalteten Lüftern erfolgreich geprüft.
120 authentifizierte Bedienbefehle wurden bestätigt. Je Bediengerät wurden
ein Gateway und ein Repeater tatsächlich geschaltet, zurückgelesen und die
ursprünglichen Zustände aller betroffenen Lüfter wiederhergestellt, ohne Neustart.
Der Test decodierte den angezeigten QR und übergab das validierte Scannergebnis;
ein optischer Kamerascan war nicht Teil dieses automatisierten Gerätetests.
Hosttests, Firmware-Regressionen, Android-Build/Lint und Android-16-Emulatortests
bestanden. Dies ist keine Zusage unbegrenzter Langzeitstabilität.

Als Update ohne Deinstallation installieren, damit Kopplungen und Einstellungen
erhalten bleiben. Diese Veröffentlichung enthält ausschließlich die App.

Im anschließenden parallelen Test beantworteten Handy und Tablet 400/400
authentifizierte Abfragen über rund zehn Minuten, ohne unerwarteten Lüfterneustart.
Die ursprünglichen Betriebszustände waren danach unverändert.
