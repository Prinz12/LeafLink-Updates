# LeafLink Android 3.3.6 – Korrekte Abfragen beim Gruppenmaster

Behebt die irreführende Meldung „Keine Geräteantwort bei: geschützter Befehl“
bei Gruppenmitgliedern, beispielsweise Lüfter 2710. Die App wartet bei
LeafLink-Geräten jetzt auf die aktuelle Gruppenrolle, bevor sie gemeinsame
Sensorwerte und Lüfterstufen abfragt. Diese Abfragen gehen nur an den
bestätigten Gruppenmaster. Veraltete Angaben aus der Geräteerkennung reichen
dafür nicht mehr aus.

Ein Wechsel von Gruppe, Geräteadresse oder Netzwerk verwirft die alte Rolle.
Rückmeldungen auf Bedienbefehle werden weiterhin für jedes Gerät geprüft.
Vorhandene Kopplungen, Hauspläne und Einstellungen bleiben beim Update erhalten.
Die Unterstützung für Originalgeräte mit HAPLA bleibt erhalten.

Auf einem echten Android-Handy mit zwei Lüftern geprüft: beide bestätigten
Stufe 2 und die Rückkehr zu Stufe 1. Wiederholte Statusabfragen und ein erneuter
App-Start liefen ohne den gemeldeten Timeout.

Dies ist ein App-Update. Die Lüfterfirmware bleibt bei 3.3.7 Beta.
