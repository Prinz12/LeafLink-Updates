# LeafLink Android 3.3.24 – Lüfter erkennen und Empfang bewerten

- Unter **Einstellungen → Lüfter → Gerätedetails** lässt sich die LED des ausgewählten LeafLink-Lüfters mit **Lüfter blinken lassen** zur Identifizierung aktivieren. Der Befehl adressiert dieses Gerät und funktioniert auch über ein erreichbares Leaf-Gateway.
- Die Gerätedetails zeigen die **WLAN-Empfangsstärke in dBm** mit farblicher Bewertung: **Gut** ab −67 dBm, **Mittel** ab −75 dBm, darunter **Schwach**. Bei geöffneten Details wird der Wert alle 15 Sekunden neu abgefragt.
- Fehlende oder ungültige Empfangswerte werden als nicht verfügbar angezeigt. Repeater ohne nutzbare Empfangsmessung sind ausdrücklich gekennzeichnet; der Empfangswert eines anderen Gateways wird nicht als Wert des Lüfters dargestellt.
- Gruppenkarten zeigen die beteiligten Geräte einmalig als **Wirkt auf: Lüfternummer · Raum · Geschoss**. Die zusätzliche Geräte-/Protokollzeile entfällt.
- Der erklärende Satz zur Zuordnung eines einzelnen Geräts zu einer anderen Lüftergruppe wurde entfernt.

Android ab 6.0; Paketkennung und Signaturschlüssel bleiben unverändert. Einstellungen, Kopplungen und Hausplan bleiben beim normalen App-Update erhalten. Diese Veröffentlichung aktualisiert die Android-App; Lüfter-Firmware wird dadurch nicht automatisch installiert.

Signierter Releasebuild, Lint und gezielte Emulatorprüfungen bestanden. Das tatsächliche LED-Blinken an einem physischen Lüfter wurde für diese App-Version noch nicht beobachtet.
