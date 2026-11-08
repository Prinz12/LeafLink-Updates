# LeafLink Updates

Öffentlicher Updatekanal für die LeafLink-Android-App und die LeafLink-Firmware.

APK, Firmware als BIN und die zugehörigen Beschreibungen stehen unter [Releases](https://github.com/Prinz12/LeafLink-Updates/releases).
Die App prüft diesen Kanal ohne Anmeldung oder GitHub-Token. Die Installation erhält
die vorhandenen App-Daten. Geräte lassen sich nur innerhalb desselben Protokolls koppeln.

Kanal: `android-dual` · Release-Tags: `app-dual-v…` · Android-Paket: `de.prinz.leaflink`.
Die App prüft Dateigröße, SHA-256, Paketkennung, Versionscode und Signatur vor der Installation.

## Firmware 3.3.13 Beta: Werksreset über die Gerätetaste

[Firmware 3.3.13 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.13-beta)
ergänzt einen bestätigten Werksreset: 15 Sekunden halten und loslassen, dann
innerhalb von 10 Sekunden erneut 4 Sekunden halten und loslassen. Gerätecode,
Betriebsstunden und Filterlaufzeit bleiben erhalten. Das normale Update erhält
alle Einstellungen. Der reale Tastentest steht noch aus; die automatisierten
Tasten-, Speicher- und Regressionstests bestanden.

## App 3.3.12: Robustere Lüfteranmeldung

[Android-App 3.3.12](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.12)
fängt vorübergehende Antwortausfälle bei der Einrichtung und Wall-Zuordnung ab.
WLAN-Daten werden bei fehlender Bestätigung nicht erneut gesendet; neue Lüfter
werden zusätzlich direkt im lokalen WLAN gesucht. Update über **App-Update**.

## App 3.3.11: Weitere Lüfter mit denselben WLAN-Daten

[Android-App 3.3.11](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.11)
ergänzt **Weiteren Lüfter hinzufügen** nach erfolgreicher WLAN-Einrichtung.
Ziel-WLAN und Passwort bleiben für die laufende Einrichtungsrunde verfügbar;
der Gerätecode wird für jeden LeafLink-Lüfter neu abgefragt. Der Fehler beim
Wechsel über **Neue Einrichtung** ist behoben. Update über **App-Update**.

## Wall Control 0.6.4 Beta: Rollen je Lüfter

[Wall Control 0.6.4 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.4-beta)
zeigt unter **Lüfter / Gruppen** sowie in der Web-Geräteverwaltung Router/Repeater,
Auto/Manuell und den Repeater-Nachbarn. Alte Werte sind als „zuletzt“ gekennzeichnet.
Inventar und Einstellungen bleiben erhalten; kein TFT-Update erforderlich.

## App 3.3.10 und Firmware 3.3.12 Beta: Netzwerkrollen und Repeater

[Android-App 3.3.10](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.10)
zeigt unter **Gespeicherte Lüfter** Router, Repeater, deren Gateway sowie
Automatik/Handrolle. Alte Werte sind ausdrücklich als „zuletzt“ gekennzeichnet.

[Lüfter-Firmware 3.3.12 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.12-beta)
korrigiert den manuellen Repeater-Test bei Wall-Kopplung und ergänzt einen
begrenzten automatischen Funkversuch bei anhaltend schwachem WLAN und einem
Gateway mit besserem WLAN-Empfang. Reale Weiterleitung und Steuerung wurden geprüft;
die Signalauslösung wurde simuliert, ein Reichweiten-Dauertest steht aus.

App-Update über **App-Update**, Lüfterupdate über **Firmware-Updates** mit
eingeschlossenen Beta-Versionen. Einstellungen und Kopplungen bleiben erhalten.

## Wall Control 0.6.3 Beta: Rollen bleiben nach Neustarts erhalten

[Wall Control 0.6.3 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.3-beta)
behält Repeater und Automatik nach einem Neustart und speichert die vollständige
Zielrolle vor der Netzübergabe. Inventar, Gruppen und Einstellungen bleiben erhalten.
Nextion HMI 302 ist unverändert; ein Display-Update ist nicht erforderlich.

## Firmware 3.3.11 Beta: Neustartkorrektur bei App-Abfragen

[Lüfter-Firmware 3.3.11 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.11-beta)
behebt einen Stacküberlauf bei geschützten App-Abfragen und spart dabei
656 Byte Stack. Die bisherigen OTA-RAM-Verbesserungen, serielle Diagnose und
Flasher-Protokolle bleiben erhalten. Zwei Lüfter absolvierten jeweils einen
30-Minuten-Lasttest und die anschließende Ruhephase ohne Neustart.

In **Firmware-Updates** die **Beta-Versionen einschließen**, dann die Version
prüfen und die Firmware herunterladen. Einstellungen und Kopplungen bleiben
erhalten; ein zusätzliches App- oder Wall-Control-Update ist nicht erforderlich.

## Firmware 3.3.10 Beta: Stabile Raumabfragen

[Lüfter-Firmware 3.3.10 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.10-beta)
behebt den zu hohen Stackbedarf bei geschützten Raumabfragen, der Watchdog-
Neustarts und vorübergehende Nichterreichbarkeit verursachen konnte. Die
OTA-RAM-Verbesserungen aus 3.3.9 bleiben enthalten. Für betroffene Lüfter
empfehlen wir das Update über **Firmware-Updates** mit eingeschlossenen
Beta-Versionen. Einstellungen und Kopplungen bleiben erhalten.

## Firmware 3.3.9 Beta: Mehr RAM für OTA-Updates

[Lüfter-Firmware 3.3.9 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.9-beta)
schafft während OTA rund 10 KiB zusätzliche RAM-Reserve und reduziert häufige
Debug-Ausgaben. Serielle Diagnose, Flasher-Protokolle und die vorhandenen
Schutzprüfungen bleiben erhalten. Einstellungen und Nutzungszähler bleiben bei
normalen Updates erhalten.

In **Firmware-Updates** die **Beta-Versionen einschließen**, dann die Version
prüfen und die Firmware herunterladen. Dafür ist kein zusätzliches App- oder
Wall-Control-Update erforderlich.

## Lebensdauer und Nutzung: App und Firmware 3.3.8

[Android-App 3.3.8](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.8)
und [Lüfter-Firmware 3.3.8 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.8-beta)
ergänzen unter **Einstellungen → Gespeicherte Lüfter → Lebensdauer & Nutzung**
ein separates Menü für jeden Lüfter. Laufzeit, Stillstand, lange Unterbrechungen
und Feuchtestillstand werden ab Firmwareinstallation erfasst. Stromlose Zeiten
sind als Netzzeit-Schätzung gekennzeichnet; die Anzeige ist kein Beweiszähler.

Die Zähler überstehen normale Firmwareupdates und Werkseinstellungen. Es gibt
keine Rücksetzfunktion. Bei plötzlichem Stromausfall kann der Abschnitt seit dem
letzten Fünf-Minuten-Checkpoint fehlen. Vollständiges Flashlöschen oder fremde
Firmware können die Daten weiterhin verändern. Details stehen in den Releases.

Neue Builds und Updatepfade unterstützen ausschließlich echte Hardware.
Der aktive Safe-Kanal wurde entfernt; historische Releases bleiben erhalten.
Wall Control 0.6.2 benötigt für diese Statistik kein Update.

## WLAN-Rückkehr: App 3.3.5 und Firmware 3.3.7 Beta

[Android-App 3.3.5](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.5)
und [Lüfter-Firmware 3.3.7 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.7-beta)
beheben die ausbleibende Wiedererkennung nach „Gespeichertes WLAN beibehalten“.
Die Firmware initialisiert das Funkmodul beim Verlassen des Einrichtungs-WLANs
vollständig neu. Die App prüft zusätzlich bekannte Geräteadressen direkt und
bevorzugt Bedienbefehle vor wartenden Hintergrundabfragen.

Für die vollständige Korrektur beide Updates installieren. In **Firmware-Updates**
die Beta-Versionen einschließen. Kopplungen, WLAN-Daten, Hauspläne und Einstellungen
bleiben erhalten. App- und Firmwareupdate erfolgen getrennt; ein Werksreset ist
nicht erforderlich. Wall Control 0.6.2 bleibt aktuell.

## Wall 0.6.2 und Lüfter-Firmware ab 3.3.6 Beta

[Wall Control 0.6.2](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.2-beta)
und [Lüfter-Firmware 3.3.6](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.6-beta)
verkürzen den Wechsel zwischen WLAN und Direktfunk und verbessern die
Bestätigung der Wall-Bedienung. Für die vollständige Korrektur beide Seiten
aktualisieren. Gemessen wurden rund 18,5 Sekunden in den Direktfunk und
25–33 Sekunden zurück ins WLAN, statt zuvor über 100 Sekunden.

Für die Lüfter in **Firmware-Updates**
Beta-Versionen einschließen und die Version erneut prüfen. Vorhandene
Zuordnungen und Einstellungen bleiben erhalten. Beim Umstieg von Wall 0.5.x
auf das geschützte Funkprotokoll 2 die Migrationshinweise im Wall-Release
beachten; bereits migrierte 0.6.x-Anlagen benötigen keine erneute Kopplung.

## Enthaltene Verbesserungen aus Android-App 3.3.4

[App 3.3.4 herunterladen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.4).
Behebt verfrühte Meldungen „Keine vollständige Rückmeldung“ bei der
Gruppensteuerung. Die App bestätigt erst die passenden Antworten aller
angesprochenen Geräte, sendet Befehle in Reihenfolge und berücksichtigt den
Mindestabstand geschützter Anmeldungen. Für diese Korrektur ist kein neues
Firmwareupdate erforderlich.

Die automatische Web-Anmeldung über **Einstellungen → verbundene Geräte → WEB**
bleibt enthalten und benötigt Firmware 3.3.4 Beta. Kopplungen, Hausplan und
Einstellungen bleiben erhalten. Das App-Update installiert keine Lüfterfirmware.

### Sicherheitsumstellung ab App 3.3.0

[App 3.3.0 herunterladen und Updatebeschreibung lesen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.0).
Die Version ergänzt Gerätecode-/QR-Kopplung, verschlüsselte LeafLink-Steuerung,
Handyzugänge und die Übernahme eines Wall-Funknetzes. Die vorhandene App erkennt
sie über **App-Update**. Android-Paket und Release-Signatur bleiben gleich.

Die LeafLink-Steuerung benötigt Firmware 3.3.0 und eine einmalige Kopplung mit
dem Gerätecode. Bei älterer LeafLink-Firmware zuerst die Sicherheitsumstellung
vorbereiten; das App-Update allein aktualisiert keine Lüfter. HAPLA wird weiterhin
separat unterstützt. Hinweise zur Wall-Migration stehen in der Updatebeschreibung.

App 3.2.2 korrigiert einen Fehlalarm nach erfolgreichen Firmware-Updates auf 3.2.0.
Bei einer bereits bestätigten Installation schließt **Firmware-Updates → Geräte
prüfen** den gespeicherten Vorgang durch Auslesen ab, ohne die Firmware erneut
zu übertragen. Änderungen an vorhandenen Einstellungen werden weiterhin erkannt.

## Firmware 3.3.4 Beta

[Signierte Hardware-Firmware 3.3.4 Beta herunterladen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.4-beta).
Die Suche nach der zugeordneten Wall trennt ein funktionierendes WLAN nicht mehr.
Die vorhandene Wall-Zuordnung und gespeicherte Daten bleiben erhalten. Die
Weboberfläche unterstützt die automatische Freigabe durch App 3.3.3 sowie
alternativ den Gerätecode und eine optional gespeicherte Browsersitzung.

Die OTA-Speicherkorrekturen aus 3.3.3 bleiben enthalten. Eine sparsamere
Web-Routenverwaltung erhält den nötigen Arbeitsspeicher. Bei älteren Versionen,
die schon vor dem Upload an Speichermangel scheitern, ist einmalig eine
datenerhaltende USB-Serviceinstallation erforderlich.

In der App **Firmware-Updates → Beta-Versionen anzeigen → nach Updates suchen**.
Voraussetzung: Hardwareprofil, ESP8266 ESP-12F mit 4 MiB Flash und bestehendes
A/B-Layout 2. Die App prüft Profil, Layout, Größe, Hash und Signatur.
Für 3.3.4 wird kein Safe-Profil mehr angeboten; historische Releases bleiben erhalten.

Beim Wechsel von 3.2.x zuerst App 3.3.1 installieren und den individuellen
Gerätecode für die anschließende physisch freigegebene Kopplung bereithalten.
Bestehende Wall-Anlagen benötigen eine abgestimmte Sicherheitsumstellung;
die Voraussetzungen und der begrenzte Hardwareprüfstand stehen in der
[Updatebeschreibung](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.4-beta).
Das App-Update allein installiert keine Lüfterfirmware.

Dieses Repository enthält ausschließlich Release-Beschreibungen und
Updateinformationen; APKs und signierte BIN-Dateien liegen als Release-Downloads
bereit. Quellcode, Schlüssel und Gerätesicherungen werden nicht veröffentlicht.

## Wandbediengerät 0.5.1 Beta

[Update und Anleitung](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.5.1-beta)
für LILYGO T-Display (16 MiB) und Nextion NX4827K043_011.
Kanal `wall-beta`, Tag-Präfix `wall-v`, Manifest `manifest.json`.
Installation über die authentifizierte Weboberfläche; die Android-App filtert
diesen separaten Kanal aus. HMI 302 bleibt unverändert.

Wall Control 0.5.1 korrigiert den schnellen Rückwechsel ins Heim-WLAN unmittelbar nach einer Neugerätesuche. 0.5.0 wird dadurch ersetzt; bitte 0.5.1 verwenden.
