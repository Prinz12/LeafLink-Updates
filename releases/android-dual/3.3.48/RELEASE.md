# LeafLink Android 3.3.48 – Gerätezugänge und Bedienung

Unter **Einstellungen → Gerätezugänge verwalten** werden Bediengeräte mit ihrer
eindeutigen Kennung zusammengefasst. Ein Zugang lässt sich nach Bestätigung
an einem einzelnen Lüfter oder an allen gekoppelten Lüftern entfernen.
Ausgeschaltete Lüfter bleiben als ausstehend vorgemerkt; bei geöffneter App
wird die Entfernung nachgeholt und durch erneutes authentisiertes Lesen bestätigt.
Der eigene Zugang ist vor versehentlicher Selbstentfernung geschützt.
Andere Gerätezugänge und gespeicherte Hauspläne bleiben erhalten.

Nach einem vollständigen App-Reset entsteht bei erneuter Freigabe ein neuer
Zugang. Ein alter Eintrag kann nun gezielt vollständig entfernt werden.
Gleiche Modellnamen werden aus Sicherheitsgründen nicht automatisch zusammengelegt.
Die Bezeichnung „Handyzugänge“ wurde durch „Gerätezugänge“ ersetzt.

Die Einstellungen behalten bei unveränderter Struktur ihre Ansicht und
Scrollposition. Laufende Statusmeldungen lösen keinen vollständigen Neuaufbau
mehr aus. Untereinanderliegende Aktionsschaltflächen erhalten mehr Abstand.
Die Geschossauswahl öffnet eine scrollbare Liste, sodass auch das dritte und
weitere Geschosse auf schmalen Handybildschirmen erreichbar bleiben.
Unter Lebensdauer & Nutzung heißt der Zähler jetzt **„Zeit mit Stromversorgung“**.

Geprüft: Zugangsverwaltung einschließlich Offline-Fällen, Neustart und verlorener
Bestätigung; Entfernung eines alten Zugangs an zwölf realen Lüftern mit bestätigter
Erhaltung der übrigen Zugänge; unveränderter Tablet-Hausplan; stabile
Einstellungsansicht über 100 Aktualisierungen; Auswahl aus zwölf Geschossen
im Handy-Emulator; bestehende Editor-, Freigabe-, Kanal- und Lokalisierungsprüfungen;
Release-Build und Lint. Scrollmessungen zeigen kleinere lange Ausreißer,
belegen aber keine pauschal bessere Jank-Rate oder dauerhaft flüssige 60 fps.

Android 9 oder neuer (minSdk 28), targetSdk Android 16 (36), Versioncode 58.
Als Update ohne Deinstallation installieren. Bestehende Zugänge und Pläne bleiben
beim normalen Update erhalten. Für Gerätezugänge ist LeafLink-Firmware 3.3.43 Beta
oder neuer erforderlich. Diese Veröffentlichung enthält keine Firmwareänderung.
