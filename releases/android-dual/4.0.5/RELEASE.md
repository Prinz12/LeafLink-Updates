# LeafLink für Android 4.0.5

Beim Koppeln per Geräte-QR-Code richtet LeafLink den lokalen Webzugriff automatisch ein, sobald der Lüfter im Heim-WLAN erreichbar ist. Ein vorhandenes gültiges Gerätezertifikat wird weiterverwendet.

Mit **WEB** öffnet sich die geschützte Lüfteroberfläche direkt in der App. Dafür ist kein Zertifikatsimport in Android nötig.

Für Firefox oder Chrome führt **Einstellungen → Gerätezugänge → Browser für dieses Zuhause einrichten** durch die einmalige Einrichtung pro Bediengerät. Die Haus-CA gilt für alle von ihr ausgestellten Lüfterzertifikate. Über **Im normalen Browser öffnen** gelangst du aus den Gerätedetails zur freigegebenen Oberfläche.

Die App läuft ab Android 9. Der automatische HTTPS-Webzugriff setzt einen gekoppelten LeafLink-Lüfter mit Firmware ab 4.0.0 voraus.
