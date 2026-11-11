# LeafLink Android 3.3.38 – Repeater-Updates mit getrennter Prüfung

Die App erkennt über den authentifizierten Gerätestatus, ob der Repeater die
Speicherfreigabe vor der Signaturprüfung unterstützt (Firmware ab 3.3.31).
Sie verwendet dann den neuen Abschlussablauf. Ältere Firmware behält ihren
bisherigen Ablauf. Eine Annahme der Prüfung gilt noch nicht als Update-Erfolg:
Gerätekennung, Zielversion, Imagehash, Startslot, bestätigter Start sowie
Einstellungen und Hausplan werden weiterhin geprüft.

Als App-Update installieren; Kopplungen und Einstellungen bleiben erhalten.
Für den neuen Ablauf benötigt der Repeater selbst Firmware 3.3.31. Bei einem
Speichermangel der alten Firmware kann deren erste Aktualisierung noch einmal
den vorübergehenden Routerbetrieb erfordern.
