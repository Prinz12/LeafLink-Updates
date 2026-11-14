# LeafLink Updates

## App 3.3.50: Geräteneutrale Netzwerkübersicht

[App 3.3.50](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.50)
bezeichnet das Bediengerät in der Netzwerkübersicht und den Verbindungsdetails
als „Dieses Gerät“ statt „Dein Handy“.

## App 3.3.49: Einheitliche Netzwerkübersicht

[App 3.3.49](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.49)
vereinheitlicht das Farbschema der Netzwerkübersicht, ergänzt einen deutlich
beschrifteten Zurück-Button und zeigt schmalere Lüfterkarten.

## App 3.3.48: Gerätezugänge und Bedienung

[App 3.3.48](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.48)
ermöglicht das Entfernen eines Gerätezugangs an einzelnen oder allen gekoppelten
Lüftern. Hinzu kommen eine scrollbare Geschossauswahl, bessere Schaltflächenabstände
und weniger Neuaufbauten der Einstellungen bei laufenden Statusmeldungen.

## App 3.3.47: Ausgeschaltete Lüfter nachträglich freigeben und App zurücksetzen

[App 3.3.47](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.47)
merkt ausdrücklich freigegebene, ausgeschaltete Lüfter verschlüsselt vor und
holt deren Zugänge bei geöffneter App automatisch nach. Beim Ergänzen von
Lüftern kann der vorhandene Hausplan erhalten bleiben. Die neue Aktion
„App vollständig zurücksetzen“ löscht nach Bestätigung nur lokale App-Daten;
Lüfter und ihre gespeicherten Pläne bleiben unverändert.

## App 3.3.46: Hausplan vollständig auf ein weiteres Gerät übernehmen

[App 3.3.46](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.46)
ergänzt die Bediengeräte-Freigabe um den vollständigen gespeicherten Hausplan:
Etagen, Raumformen und Maße, Materialien, Fenster, Türen, Durchgänge,
Etagenverbindungen, Lüfterpositionen und sämtliche zugehörigen Planeinstellungen.
Beide Apps aktualisieren und die Freigabe vom Gerät mit dem vollständigen Plan
wiederholen. Der Quellplan ersetzt den bisherigen Empfängerplan ohne zusätzliche
Sicherung. Bestehende Lüfterzugänge bleiben erhalten. Die Übernahme wurde zwischen
Samsung-Handy und Samsung-Tablet einschließlich Inhaltsvergleich nach Neustart
und Anzeige geprüft. Firmware 3.3.43 Beta bleibt unverändert.

## App 3.3.45 und Firmware 3.3.43: Weiteres Bediengerät hinzufügen

[App 3.3.45](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.45)
und [Firmware 3.3.43 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.43-beta)
ermöglichen die lokale Freigabe bereits gekoppelter Lüfter an ein weiteres Handy
oder Tablet. Auf dem vorhandenen Handy in den Einstellungen **Weiteres
Bediengerät hinzufügen**, auf dem neuen Gerät **Freigabe übernehmen** wählen.
Beide Apps im selben Heim-WLAN geöffnet lassen. Das neue Gerät erhält eigene
Zugänge; vorhandene Kopplungen bleiben erhalten. Zehn eingeschaltete Lüfter wurden
zwischen Samsung-Handy und Samsung-Tablet erfolgreich freigegeben und erneut geprüft.

Zuerst beide Apps aktualisieren, anschließend die Lüfter im Beta-Kanal.
Ausgeschaltete Lüfter lassen sich später durch eine erneute Freigabe ergänzen.
Die leere Startansicht erklärt die erste Einrichtung. Fabrikneue Lüfter starten
die Kopplung erst nach dem vorgesehenen Tastendruck. Android 9 oder neuer erforderlich.

## App 3.3.44: Android 16 und zuverlässige Kommunikation

[App 3.3.44 herunterladen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.44).
Voraussetzung ist jetzt **Android 9 oder neuer**. Die App verwendet `targetSdk 36`
und unterstützt die neue System-Zurück-Navigation sowie angepasste Abstände zu
Systemleisten und Kameraausschnitten. Tests auf Android 9, 16 und 17 sowie im
Tabletfenster bestanden. Im Flottentest mit Firmware 3.3.42 Beta antworteten
alle zwölf Lüfter auf 240/240 authentifizierte Abfragen, ohne Neustart.
Als Update ohne Deinstallation installieren; Einstellungen und Kopplungen bleiben erhalten.

## App 3.3.42 und Firmware 3.3.36: Lebensdauer bei Repeatern

[App 3.3.42](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.42)
und [Firmware 3.3.36 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.36-beta)
beheben gemeinsam den fehlenden Abruf unter **Lebensdauer & Nutzung** bei
Repeatern. Die App liest die Zähler über die verschlüsselte Geräteverbindung.
Zuerst die App, anschließend die betroffenen Repeater aktualisieren;
ein reines Gateway-Update reicht nicht. Vorhandene Zähler bleiben erhalten.
Builds, Hosttests und Emulatorprüfung bestanden; physischer Repeatertest noch offen.

## App 3.3.41 und Firmware 3.3.35: Getaktete Repeater-Updates

[App 3.3.41](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.41)
und [Firmware 3.3.35 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.35-beta)
verkürzen den Repeater-Erstzugriff und takten Gateway-Funkfragmente anhand
der Sendebestätigungen. Zwei vollständige Vergleichsläufe an 1255 bestätigten
kürzere Übertragungen mit weniger Wiederholungen und erhaltenen Einstellungen.

## App 3.3.40 und Firmware 3.3.34: Weniger OTA-Wiederholungen

[App 3.3.40](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.40)
und [Firmware 3.3.34 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.34-beta)
verbinden kleinere Funkblöcke mit einer strikt geordneten Gateway-Queue.
Im Vergleich an 1255: 137 auf 97 Wiederholungen und 292,031 auf 261,423 Sekunden
über denselben direkten Gateway. Start und Datenerhalt wurden bestätigt.
Für diesen Vorteil App und verwendete Gateways aktualisieren; der Repeater
benötigt mindestens 3.3.33 für das Sendefenster.

## App 3.3.39 und Firmware 3.3.33: Adaptives Repeater-Update

[Android 3.3.39](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.39)
und [Firmware 3.3.33 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.33-beta)
ergänzen ein auf zwei Blöcke begrenztes, an die Verbindung angepasstes Sendefenster.
Im Vergleich auf Repeater 1255 sank die Übertragungszeit um 12.1 %;
bestätigter Start, Einstellungen und Hausplan wurden nach beiden Transfers geprüft.
Für das Fenster benötigt der Repeater bereits 3.3.33. Die Erstinstallation auf
älterer Firmware verwendet den bisherigen Ablauf. Kein Rollenwechsel erforderlich,
wenn der Repeater bereits den speichersparenden Updater ab 3.3.31 besitzt.

## Firmware 3.3.32: Automatische Gegenrichtung bei Repeatern

[Firmware 3.3.32 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.32-beta)
behebt fehlende Partnerdaten für die automatische Richtungszuordnung im
Repeaterbetrieb. Gateways leiten diese Daten gezielt in die jeweilige Gruppe
weiter, auch bei Partnern an unterschiedlichen Gateways.
Beide Partner und ihre möglichen Gateways aktualisieren; bei wechselnden
Rollen alle Lüfter auf denselben Stand bringen. Auto-Einstellung, Gruppen und
Kopplungen beibehalten. App 3.3.38 bleibt passend. Die reale Gegenrichtung nach
Installation ist noch zu bestätigen.

## App 3.3.38 und Firmware 3.3.31: Speicher beim Repeater-Update

[Android 3.3.38](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.38)
und [Firmware 3.3.31 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.31-beta)
trennen die Firmwareübertragung von der Signaturprüfung. Der Repeater gibt
vor der abschließenden Prüfung seine Funk- und Empfangspuffer frei. Die App
meldet Erfolg erst nach dem bestätigten Start des richtigen Images.
Zuerst die App aktualisieren. Die Korrektur muss auf dem Repeater selbst
installiert sein; bei bisherigem Speichermangel kann dafür einmalig Routerbetrieb
nötig sein. Der vollständige Folgetest auf einem realen Repeater bestand:
747652 Byte übertragen, bestätigter Slotwechsel, Einstellungen und Hausplan
erhalten. Gesamtdauer 6 Minuten 7 Sekunden, ohne weiteren Rollenwechsel.

## App 3.3.37 und Firmware 3.3.30: Auto-Anzeige und Gatewaywechsel

[Android 3.3.37](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.37)
behält die zuletzt bestätigte Installationsrichtung bei fehlenden Antworten
markiert und kennzeichnet den fehlenden aktuellen Status separat.
[Firmware 3.3.30 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.30-beta)
gibt alte Repeater-Adressen nach einem bestätigten Gatewaywechsel frei.
Für diese Firmwarekorrektur die Gateways aktualisieren; Repeater können
auf 3.3.29 bleiben. Kopplungen und Einstellungen bleiben erhalten.

## App 3.3.36 und Firmware 3.3.29: Netzwerkanfragen und Gatewaywahl

[Android 3.3.36](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.36)
vermeidet konkurrierende Identitätsabfragen für gerade bestätigte Geräte.
[Firmware 3.3.29 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.29-beta)
berücksichtigt WLAN-Signal, beobachtete Beacon-Verluste und geschätzte Last bei
der Gatewaywahl. Gestaffelte Haltezeiten stabilisieren die Auswahl; bei Ausfall
wird ohne diese Wartezeit neu gewählt. Enthält außerdem die Speicher- und
Zustellungskorrekturen für den Funktransport. Für die vollständige adaptive
Auswahl alle beteiligten Gateways und Repeater aktualisieren.
Als Updates installieren; Kopplungen und Einstellungen bleiben erhalten.

## App 3.3.35: Korrigierte Verbindungsprüfung

[Android 3.3.35](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.35)
enthält alle Darstellungskorrekturen aus 3.3.34. Zusätzlich berücksichtigt der
Verbindungstest verzögerte Antworten bis drei Sekunden und die 250-ms-Antwortbegrenzung
der Firmware. So erzeugen zu schnelle Prüfanfragen keine zusätzlichen Warnungen.
Als Update installieren; Kopplungen und Einstellungen bleiben erhalten.

## App 3.3.34: Stabile Netzwerkübersicht

[Android 3.3.34](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.34)
korrigiert das Flackern bei Aktualisierungen und erhält die geöffnete Netzwerkseite
beim Drehen. Handy und Router bleiben über der seitlich verschiebbaren Gerätekarte
sichtbar. Aktuelle Wege sind durchgezogen; Diagnosehinweise nennen Lüfter und Grund.
Als App-Update installieren; Kopplungen und Einstellungen bleiben erhalten.
Gegenüber 3.3.33 ist kein Firmware- oder Wall-Update erforderlich.

## App 3.3.33: Netzwerkübersicht und Verbindungsprüfung

[Android 3.3.33](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.33)
ergänzt eine grafische Netzwerkübersicht mit direkten Gateways und gemeldeten
Repeaterketten bis sechs Funkhops. Die Geräteprüfung zeigt Antwortanzahl und
mittlere Antwortzeit. Veraltete und unvollständige Routen bleiben erkennbar;
die Endgeräteprüfung wird nicht als Messung einzelner Funkstrecken ausgegeben.
Kompakte Karten und dauerhaft erreichbare Prüfschaltflächen unterstützen auch
kleine Displays und Querformat. Als App-Update installieren; gegenüber 3.3.32
ist kein zusätzliches Firmware- oder Wall-Update nötig. Die Anforderungen des
Sicherheitsupdates unten gelten weiterhin.

## App 3.3.32: VPN-Suche nach Adresswechseln

[Android 3.3.32](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.32) findet bekannte Lüfter bei geöffneter App auch dann im bisherigen Heimnetz wieder, wenn alle gespeicherten Adressen gewechselt haben. Neue direkt bestätigte Adressen ersetzen alte automatisch. Kopplungen, Räume und manuelle Ausschlüsse bleiben erhalten. Installation als App-Update durch den Nutzer; für diese Korrektur kein zusätzliches Firmware- oder Wall-Update nötig. Die Versionsanforderungen des Sicherheitsupdates unten gelten weiterhin.

## App 3.3.28: QR-Scanner mit Scanrahmen

[Android 3.3.28](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.28) ergänzt einen animierten Scanrahmen, einen grünen Erfolgsrahmen mit Häkchen, kurze Vibration und eine Taschenlampentaste. Nur vollständig im Rahmen liegende Gerätecodes werden übernommen. Die Verarbeitung bleibt lokal auf dem Handy.

Als App-Update installieren; vorhandene Daten und Kopplungen bleiben erhalten. Der Protokollstand entspricht 3.3.27. Bei älteren App-/Firmwareständen zunächst die nachfolgende Reihenfolge des Sicherheitsupdates beachten.


## Sicherheitsupdate: Nonce-Korrektur

## Reihenfolge für dieses Sicherheitsupdate

1. Bei App-Zugriff über die Wall zuerst **Wall Control 0.6.8 Beta** aktualisieren.
2. Alle betroffenen Lüfter auf **Firmware 3.3.25 Beta** bringen: signiertes Hardware-A/B-Image über die vorhandene Web-Serviceoberfläche oder den verifizierten A/B-Installer installieren und den bestätigten Start prüfen. Kein Vollflash, kein Zurücksetzen.
3. Danach **Android 3.3.27** über den App-Updatekanal installieren. Die App als Update installieren, nicht deinstallieren.

**Alte und neue App-/Lüfterstände sind für die geschützte Steuerung nicht kompatibel.** Die alte App kann nach dem Firmwarewechsel auch die abschließende OTA-Statusprüfung nicht mehr ausführen. Deshalb diesen Übergang über die Web-Serviceoberfläche bzw. den verifizierten A/B-Installer durchführen. Eine bereits aktualisierte App kann alte Lüfter nicht per App-OTA aktualisieren; in diesem Fall ebenfalls den Web-/A/B-Weg verwenden.

Kopplungen, Gerätecodes, Gruppen, WLAN-Einstellungen und vorhandene Wall-Zuordnungen bleiben erhalten. Kein erneutes Anlernen erforderlich. HAPLA-Geräte bleiben unterstützt. Das Nextion-Display bleibt bei HMI 302; kein TFT-Update erforderlich.

Zusammengehörige Versionen: [Firmware 3.3.25 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.25-beta), [Android 3.3.27](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.27), [Wall 0.6.8 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.8-beta).

## Prüfung

Neue App-Sitzungen erhalten einen frischen authentifizierten Schlüsselkontext. 290 Verschlüsselungen mit Paketverlust, über 40 separaten App-Prozessneustarts und simulierten Firmware-Neustarts ergaben kein doppeltes Schlüssel/Nonce-Paar. Replay-, Manipulations-, Zählergrenzen-, Kopplungs-, Wall-, Build- und Android-Emulatorprüfungen bestanden. Kein Live-Hardwaretest dieses Builds. Die Veröffentlichung installiert nichts automatisch.

Öffentlicher Updatekanal für die LeafLink-Android-App und die LeafLink-Firmware.

APK, Firmware als BIN und die zugehörigen Beschreibungen stehen unter [Releases](https://github.com/Prinz12/LeafLink-Updates/releases).
Die App prüft diesen Kanal ohne Anmeldung oder GitHub-Token. Die Installation erhält
die vorhandenen App-Daten. Geräte lassen sich nur innerhalb desselben Protokolls koppeln.

Kanal: `android-dual` · Release-Tags: `app-dual-v…` · Android-Paket: `de.prinz.leaflink`.
Die App prüft Dateigröße, SHA-256, Paketkennung, Versionscode und Signatur vor der Installation.

## Webanmeldung beim Service: Firmware 3.3.24 Beta

[Firmware 3.3.24 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.24-beta) erhält die App-Webanmeldung beim Wechsel zur Serviceseite, Neuladen während der Anmeldung und wiederhergestellten Browserseiten. Die geschützte Anmeldung bleibt erforderlich; eine erfolgreiche App-Freigabe muss nicht erneut mit dem Gerätecode bestätigt werden. Nach dem Firmwareupdate die Webseite erneut aus der App öffnen. Android 3.3.26 und Wall 0.6.7 bleiben kompatibel. Installation durch den Nutzer.

## Fernneustart und VPN-Gerätesuche: Firmware 3.3.23 Beta, App 3.3.26

[Firmware 3.3.23 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.23-beta) ermöglicht den geschützten Neustart über **Service & Diagnose → Servicemodus starten → Neutral neu starten** ohne Tastendruck am Lüfter. [Android 3.3.26](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.26) verbessert das Nachfinden über mehrere Geräteübersichten im VPN. Die Firmware bleibt gegen Neustarts während Updates oder ohne bestätigten neutralen Motorausgang gesperrt. Eine doppelte VPN-/DHCP-Adresse muss weiterhin im Router behoben werden; ein Neustart garantiert keine neue Adresse. Installation durch den Nutzer, praktischer Neustart-/VPN-Test dieses Releases noch ausstehend. Wall 0.6.7 bleibt kompatibel.

## Adaptive Sommermessung: App 3.3.25, Firmware 3.3.22 Beta, Wall 0.6.7 Beta

[Android 3.3.25](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.25), [Lüfterfirmware 3.3.22 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.22-beta) und [Wall Control 0.6.7 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.7-beta) ergänzen die wählbare Messung bis zur Temperaturstabilisierung. Beide Lüfter müssen ihre Messung bestätigen; bei Zeitablauf gibt es keine neue Kühlfreigabe. Auswahl über App, Wall und Web. Alle Gruppenlüfter aktualisieren. Installation durch den Nutzer; thermischer Praxistest noch ausstehend. Details in den Releasebeschreibungen.

## Firmware 3.3.21 Beta und App 3.3.23: Service und Sommer-Gruppenwerte

[Android 3.3.23](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.23) ergänzt die Sommerautomatik-Einstellungen pro Gruppe und zeigt Service 2 an. [Firmware 3.3.21 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.21-beta) zählt alle Motorbewegungen, quittiert fälligen Service nach 1,5 Sekunden Tastendruck und zeigt ihn mit Dauerlicht an. Service 2 wird standardmäßig nach 12960 Motorstunden fällig, etwa 18 Monaten Dauerbetrieb. Zuerst die App, danach alle beteiligten Lüfter aktualisieren; Beta-Versionen in der Firmwareauswahl aktivieren. Wall 0.6.6 Beta bleibt kompatibel. Automatisierte Prüfungen bestanden, praktischer Gerätetest noch ausstehend. Details zu Wartungsdaten und Kompatibilität in den Releasebeschreibungen.

## App 3.3.22: Firmware-Abschluss nach IP-Wechsel

[Android 3.3.22](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.22) findet gekoppelte Lüfter nach einem DHCP-Adresswechsel erneut und prüft die neue Adresse mit dem Geräteschlüssel. Gespeicherte Fehlversuche lassen sich über **Geräte prüfen → Fehlversuch prüfen** wieder aufnehmen; ein erneuter Upload benötigt eine ausdrückliche Bestätigung. Firmware 3.3.20 Beta und Wall 0.6.6 Beta bleiben aktuell.

## Firmware 3.3.20 Beta: IP-Konflikte und Routername

[Firmware 3.3.20 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.20-beta) ergänzt ARP-Konflikterkennung und automatische neue DHCP-Anfragen ohne Geräteneustart. Der Routername lautet `Leaf-` plus Lüfternummer. Einrichtungs-AP und Kopplungen bleiben erhalten. Android 3.3.21 und Wall 0.6.6 Beta bleiben kompatibel. Automatisierte Prüfungen bestanden; ein realer Konflikt-/DHCP-Wechseltest steht noch aus. Details und Grenzen in der Releasebeschreibung.

## Firmware 3.3.19 Beta und App 3.3.21: Speicher und Temperaturanzeige

[Firmware 3.3.19 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.19-beta) reserviert den Arbeitsbereich für die laufende verschlüsselte Bedienung und behebt die beobachtete Anmeldeblockade bei fragmentiertem Speicher. [Android 3.3.21](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.21) zeigt im Modus Sommerautomatik pro Lüfter Innen- und Außentemperatur auf der Gruppenseite. Beide Updates zusammen installieren; Wall 0.6.6 Beta bleibt kompatibel.

Automatisierte Prüfungen und ein begrenzter realer Belastungstest bestanden. Ein uneingeschränkt neustartfreier Dauerbetrieb unter jeder Bedingung ist damit nicht nachgewiesen; geplante Update- und Wartungsneustarts bleiben erhalten. Details in den Releasebeschreibungen.

## Sommerautomatik: Firmware 3.3.18 Beta, App 3.3.20 und Wall 0.6.6 Beta

[Firmware 3.3.18 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.18-beta) regelt die Sommerautomatik direkt auf den Lüftern: kurze Messläufe erfassen Innen- und Außenluft, anschließend wird innerhalb der Gruppe die kühlere geeignete Zuluftseite gewählt. Dauerhafte Kühlung startet oberhalb 23 °C innen bei mindestens 2 °C kühlerer Außenluft. Die Messläufe finden beim Start und alle fünf Minuten statt und können kurzzeitig wärmere Außenluft ansaugen.

Der eigene Modus ist über [Android 3.3.20](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.20), die Lüfter-Weboberfläche sowie [Wall Control 0.6.6 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.6-beta) auswählbar. Alle beteiligten Lüfter aktualisieren; mindestens zwei kompatible Geräte in derselben Gruppe sind erforderlich. App und Wall müssen für den laufenden Betrieb nicht eingeschaltet bleiben. Das Nextion-Display benötigt kein TFT-Update.

Software-, Build-, Protokoll-, Browser- und Emulatorprüfungen bestanden. Das thermische Verhalten im realen Haus ist noch nicht praktisch erprobt. Die Veröffentlichung installiert keine Geräte automatisch.

## App 3.3.19: Mehrere Lüfter gezielt einrichten

[Android 3.3.19](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.19) wählt bei gleichnamigen Einrichtungsnetzen gezielt den passenden Lüfter. QR-Code oder manuelle Eingabe von Gerätenummer und Gerätecode werden unterstützt. Ziel-WLAN und Passwort bleiben für weitere Lüfter derselben Einrichtungsrunde verfügbar. Fünf zusätzliche Lüfter wurden nacheinander am echten Handy erfolgreich eingerichtet; die App zeigte danach alle drei Paare vollständig an.

## App 3.3.18 und Firmware 3.3.17 Beta

[Android 3.3.18](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.18) filtert vorübergehende Fehler aus den Meldungen, zeigt einen dauerhaften Updatehinweis und unterstützt Webzugang sowie Hausplansicherung über Repeater.

[Firmware 3.3.17 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.17-beta) ergänzt die verschlüsselte Repeater-Hausplansicherung und korrigiert die Webanmeldung bei knappem Gerätespeicher. Beide Updates zusammen installieren; Wall 0.6.5 Beta bleibt aktuell. Während Firmware-Updates die App nicht vollständig schließen oder wegwischen und das Handy im WLAN lassen.

## App 3.3.17, Firmware 3.3.16 Beta und Wall 0.6.5 Beta

[Android 3.3.17](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.17) korrigiert Gruppennamen und die Anordnung der Geräteeinstellungen; Richtung und Netzwerkrollenwechsel werden im offenen Dialog nachgelesen.
[Firmware 3.3.16 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.16-beta) ermöglicht Updates direkt in der Repeaterrolle, korrigiert Gruppennamen und fehlende Sensorwerte in der Weboberfläche und arbeitet ohne eingeschaltete Wall. Die neue Update-Empfangsfunktion muss einmalig über USB oder direktes WLAN installiert werden; danach braucht der Repeater für Updates keine Routerverbindung.
[Wall 0.6.5 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.6.5-beta) übernimmt Gruppennamen aus dem App-Hausplan.

## App 3.3.16 und Firmware 3.3.14 Beta: Rollen und Richtung

[Android 3.3.16](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.16) aktualisiert Master/Slave nach der Gruppenzuordnung schneller und ergänzt die Auswahl **Automatisch / Router / Repeater**.
[Firmware 3.3.14 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.14-beta) erhält die gewählte Netzwerkrolle nach Neustarts und ergänzt automatische IN/OUT-Paare mit IN als Einzelgeräte-Standard. Manuelle Richtungen bleiben erhalten. Beide Updates sind für den vollständigen Funktionsumfang erforderlich.

## App 3.3.15: Gruppen wechseln und freie Partnerplätze wählen

[Android-App 3.3.15](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.15)
ergänzt **Gruppe ändern** direkt an erreichbaren Lüftern in der Raumübersicht.
Bei der Neueinrichtung werden passende bestehende Gruppen ohne Partner angeboten.
Offline-Mitglieder und die bereits eingerichteten Lüfter derselben Runde werden
bei der Belegung berücksichtigt. Update über **App-Update**.

## App 3.3.14: Stromlose Lüfter schneller erkennen

[Android-App 3.3.14](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.14)
erkennt dauerhaft fehlende Antworten bei geöffneter App normalerweise nach etwa
10–15 Sekunden. Einzelne verlorene Antworten werden toleriert; gespeicherte
Zuordnungen bleiben erhalten. Auf einem Samsung-Handy mit simuliertem Antwortausfall
geprüft. Update über **App-Update**.

## App 3.3.13: Lüfter schneller wiederfinden

[Android-App 3.3.13](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.13)
sucht fehlende bekannte Lüfter bei geöffneter App alle fünf Sekunden erneut.
Langsame oder ausgeschaltete Geräte blockieren die schnelle Suche und Status-Pings
anderer Geräte nicht mehr. Direkt auf einem Samsung-Handy geprüft; Update über
**App-Update** mit erhaltenen Einstellungen.

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
