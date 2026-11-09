# LeafLink Android 3.3.22 – Firmware-Updates nach IP-Wechsel

Wechselt ein gekoppelter Lüfter beim Firmware-Update seine DHCP-Adresse, sucht die App ihn im lokalen Netz erneut und bestätigt die neue Adresse mit dem bestehenden Geräteschlüssel. Die Abschlussprüfung folgt anschließend dem richtigen Lüfter. Eine fremde Antwort an der alten Adresse gilt nicht als Updatebestätigung.

Gespeicherte, unbestätigte Updateversuche bleiben erhalten. Nach Installation der App unter **Firmware-Updates → Geräte prüfen** erneut prüfen. Wenn das Gerät auf seine vorige Firmware zurückgefallen ist: Firmware herunterladen, **Fehlversuch prüfen** wählen und den angebotenen erneuten Upload ausdrücklich bestätigen. Die App startet keinen automatischen Doppel-Upload.

Firmware **3.3.20 Beta** und Wall **0.6.6 Beta** bleiben aktuell. Die Veröffentlichung installiert weder App noch Lüfter automatisch. Vorhandene App-Daten und Kopplungen bleiben erhalten.

Releasebuild, Lint, Protokoll-/Interoperabilitätsprüfungen sowie Emulatorprüfungen für aktuelle Firmware-Updates, IP-Wechsel, Identität und Updateabschluss bestanden. Der erneute Updateversuch am betroffenen realen Lüfter steht noch aus. Die Wiederentdeckung benötigt Erreichbarkeit im lokalen Netz; getrennte VLANs oder ein geroutetes VPN können sie einschränken.

Signiertes Update für `de.prinz.leaflink`, Versionscode **31**.
