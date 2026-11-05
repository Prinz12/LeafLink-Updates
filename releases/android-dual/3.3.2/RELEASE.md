# LeafLink Android 3.3.2 – OTA-Geräteerkennung über WLAN

Behebt „Nicht erreichbar / nicht kompatibel“ bei erreichbaren LeafLink-Lüftern, deren Mesh-Funknetz momentan nicht gestartet ist. Die App liest in diesem Fall die tatsächliche Gerätekennung direkt aus und gleicht Gerätenummer, Funkkennung und Gruppe ab. Auch die anschließende OTA-Gesundheitsprüfung unterstützt diesen WLAN-Betrieb.

Identitätsabgleich, Motorfehler- und Servicesperren, Gerätekopplung, signierte Firmwareprüfung, A/B-Startbestätigung und Kontrolle gespeicherter Einstellungen bleiben aktiv. Ein noch nicht gekoppeltes Handy muss den Lüfter vor dem Update mit seinem individuellen Gerätecode koppeln.

## Installation

In **App-Update** nach Updates suchen und 3.3.2 über die vorhandene App installieren. Anschließend **Firmware-Updates → Geräte prüfen**. Für Firmware 3.3.1 Beta muss **Beta-Versionen anzeigen** aktiviert sein. Ein bereits auf 3.3.1 aktualisierter Lüfter wird als **Bereits aktuell** angezeigt.

Paket `de.prinz.leaflink`, versionCode 11, Android ab API 23, unverändertes Release-Signaturzertifikat. Vorhandene App-Daten und Handyzugänge bleiben erhalten.

Build und Lint, Protokoll- und Kopplungs-Hosttests sowie API-23-Emulatorprüfungen bestanden. Die tatsächliche OTA-Erkennung wurde zusätzlich auf einem Samsung SM-S918B mit zwei echten Geräten geprüft. Neue Tests decken ruhendes Mesh, Neustart, fehlende und widersprüchliche Identitäten sowie weiterhin gesperrte Motorfehler ab.
