# LeafLink 3.3.51 Beta – Aktuelle Verbindungsdiagnose

Die Geräte-Webübersicht bewertet neue Verwerfungen und Wiederholungen über
einen gleitenden Messzeitraum von mindestens 60 Sekunden. Hohe Gesamtzähler
aus vergangenen Betriebsstunden erzeugen allein keine Verbindungswarnung mehr.

- Aktuelle Ereignisse pro Minute und ausklappbare Gesamtzähler je Gerät.
- Warnung ab 25 neuen Verwerfungen/min oder 50 Wiederholungen/min.
- Fehlende, veraltete oder gesättigte Messwerte werden ausdrücklich benannt.
- Detailursachen am geöffneten Gateway, etwa volle Empfangswarteschlange,
  fehlgeschlagene Funksendung oder Speicherschutz. Für entfernte Geräte werden
  nicht übertragene Ursachen nicht geraten.
- Kein zusätzlicher Messverlauf im Lüfterspeicher und keine zusätzlichen
  Funkabfragen. Bestehende Gerätemeldungen, Einstellungen und Hausplan bleiben erhalten.

Nach dem Update die Webseite des aktualisierten Gateways neu laden und etwa
eine Minute geöffnet lassen. Darüber werden auch ältere Lüfter und Repeater
bewertet. Andere Gateways erhalten die neue Oberfläche durch ihr eigenes Update.

Diese Version verbessert die Diagnoseanzeige. Sie behebt keine zugrunde
liegenden Funkfehler oder Watchdog-Ursachen.
