# LeafLink 3.3.52 Beta – Funkverarbeitung während Webseitenabrufen

Behebt eine nachgewiesene Ursache voller Funk-Empfangswarteschlangen:
Während längerer HTTP-Antworten wurde die eigene Funkverarbeitung bisher
nicht bedient. Sie läuft jetzt begrenzt und kooperativ weiter.

- Direkter Vergleich auf Lüfter 3111: 15 vollständige Webseitenabrufe
  verursachten vorher 257 Empfangsüberläufe, mit dieser Version keinen.
- Daten fremder Funkrouten belegen nicht mehr die eigene Empfangswarteschlange.
  Authentifizierung und Replay-Schutz bleiben erhalten.
- WLAN-Gateways ohne frischen Repeater senden Suchanfragen nicht zusätzlich
  über Funk. Bereits angekündigte und indirekte Repeater bleiben erreichbar.
- SDK-Sendungen werden einzeln abgearbeitet und Rückrufe dem Ziel zugeordnet.
  Peer-Löschung und Kanalwechsel erfolgen nicht während einer laufenden Sendung.
- Neue Diagnosezähler für fremde Routen, Empfangspausen und unerwartete Rückrufe.
  Die Empfangsqueue und das Funkformat bleiben unverändert.

Einstellungen, Hausplan, Kopplungen und Signatur-/A/B-Prüfungen bleiben erhalten.
Die aktuelle App 3.3.54 kann dieses Firmwareupdate installieren.

Die Änderungen beseitigen die reproduzierte Empfangsblockade und schützen
Funkressourcen vor überlappenden Zugriffen. **Eine endgültige Behebung des
seltenen SDK-Watchdogs ist damit noch nicht nachgewiesen.** Die SDK-Assertion
wird nicht umgangen. Einzelne Funkverluste oder kontrollierte Speicherabweisungen
können weiterhin auftreten; entsprechende Zähler bleiben sichtbar.
