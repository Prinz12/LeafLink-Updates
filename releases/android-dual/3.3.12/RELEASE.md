# LeafLink Android 3.3.12 – Robustere Lüfteranmeldung

Die Einrichtung kann kurze Antwortausfälle beim Handynamen, Funknetzschlüssel
und der Wall-Zuordnung automatisch abfangen. Bereits übertragene WLAN-Daten
müssen dafür nicht erneut eingegeben werden.

## Änderungen

- Begrenzte Wiederholungen bei ausbleibenden Antworten auf sichere, wiederholbare
  Einrichtungsschritte. Gerätecode und Authentifizierung bleiben erforderlich.
- Verspätete und doppelte bestätigte Antworten stören nachfolgende Schritte nicht.
- Bei fehlender WLAN-Bestätigung sucht die App den Lüfter im Zielnetz weiter.
  WLAN-Daten werden dabei nicht automatisch erneut gesendet.
- Bei fehlender Gruppenbestätigung prüft die App die tatsächlich gespeicherte
  Zuordnung, ohne die Änderung automatisch erneut zu senden.
- Neue Lüfter werden bei ausbleibendem Broadcast zusätzlich direkt im privaten
  lokalen /24- oder kleineren WLAN-Subnetz gesucht.
- Weiteren Lüfter hinzufügen verwendet weiterhin die WLAN-Daten der geöffneten
  Einrichtungsrunde. Beim Schließen werden diese aus dem Arbeitsspeicher gelöscht.

## Installation und Prüfung

Über **App-Update** nach Updates suchen oder über die vorhandene App installieren.
Paketkennung und Signatur bleiben gleich; App-Daten, Kopplungen und Hauspläne
bleiben erhalten. Android 6.0 oder neuer erforderlich.

Mit einem physischen Lüfter und Samsung-Handy wurden Kopplung, Wall-Zuordnung
und WLAN-Übertragung erfolgreich durchgeführt. Die zusätzliche direkte Suche
wurde anschließend auf demselben Handy gegen den Lüfter ohne gespeicherte
Zieladresse oder Broadcast erfolgreich geprüft. Verlorene und doppelte Antworten
wurden zusätzlich mit 169 verschlüsselten Regressionen geprüft. Setup- und
Protokolltests, Build und Lint bestanden. Die vollständige Neuanmeldung wurde
nach der abschließenden Suchergänzung nicht nochmals wiederholt.
