# LeafLink RTOS 4.2.58

Das signierte A/B-Flottenupdate ist für kompatible LeafLink-Lüfter mit ESP8266, 4 MB Flash und Layout 2 bestimmt.

- Der HTTPS-Empfang verwendet einen wiederverwendbaren TLS-Puffer. Während des Uploads beschreibt der authentifizierte HTTPS-Task den inaktiven Slot exklusiv. Die Firmware prüft Image und Signatur vor dem Slotwechsel.
- Aktualisiere zuerst die LeafLink-App auf 4.2.12. Sie verwendet bei älteren RTOS-Ständen verschlüsseltes UDP und bevorzugt danach HTTPS bei direkter WLAN-Verbindung. Für Updates über andere Lüfter bleibt verschlüsseltes UDP verfügbar.
- Mit demselben korrigierten Schreibpfad hat ein kompatibler Lüfter zehn HTTPS-Updates in Folge abgeschlossen. Der private Teststand 4.2.57 kann regulär auf 4.2.58 wechseln.

In der App unter **Firmware-Updates → Version prüfen → Geräte prüfen** nach dem Update suchen.
