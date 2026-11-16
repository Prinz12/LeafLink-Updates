# LeafLink 3.3.53 Beta – Korrektur gleichzeitiger Funk-Sendeereignisse

Behebt einen konkreten Fehler in der Ereignisreihenfolge des WLAN-Treibers:
Treffen RTS und Sendeabschluss unterschiedlicher Warteschlangen gleichzeitig
ein, konnte der Treiber die falsche Warteschlange prüfen, in einer Assertion
hängen bleiben und dadurch einen Watchdog-Neustart auslösen.

- Gezielte Übernahme der Ereigniskorrektur bei unverändertem bisherigen SDK.
  Assertions, Signaturprüfung und A/B-Rückfallschutz bleiben aktiv.
- Nachstellung am originalen Maschinencode erreicht die bekannte Absturzstelle
  `0x40104d26`. Die Korrektur besteht 64 Queue-Kombinationen und 320 Prüfungen
  der Abschluss-/Fehlerreihenfolge, außerdem Sonder- und ungültige Queue-Fälle.
- Neue Statusfelder `sdkVersion` und `sdkTxOrderDeferrals` für die Diagnose.
- Kein zusätzlicher dynamischer Speicherbedarf des Fixes; statischer RAM +16 Byte.

Über das physische Tablet auf zwei Geräten installiert und bestätigt;
Einstellungen, Hausplan und Kopplungen bleiben erhalten. Drei echte
App-Netzprüfungen ergaben 360/360 Antworten. Während 31 Minuten Gerätebeobachtung
gab es keine ungeplanten Neustarts oder neuen Empfangsüberläufe. Unter HTTP-Last
trat eine kontrollierte Speicherabwehr auf; der Heap erholte sich anschließend.

Der geplante Sechsstundentest wurde auf Nutzerwunsch vorzeitig beendet.
Ein mehrstündiger Stabilitätsnachweis liegt für diese Version noch nicht vor.
Der seltene Ereigniskonflikt wurde im kurzen Hardwaretest nicht gezählt;
die historische genaue Interruptkombination lässt sich aus den alten Crashdaten
nicht rückwirkend beweisen. Die reproduzierte Fehlerursache und ihre Korrektur
sind am Binärcode geprüft; weitere Watchdog-Ursachen bleiben möglich.

Für Hardwaregeräte mit bestehendem A/B-Layout 2. Installation mit der aktuellen
App 3.3.54 und aktivierten Beta-Firmwareupdates.
