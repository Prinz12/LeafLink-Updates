# Wall Control 0.6.7 Beta – Adaptive Sommermessung

Die neue Gruppenoption **Bis Temperatur stabil** verlängert Innen- und Außenmessungen bedarfsgerecht. Die Regelung läuft vollständig in der Lüfterfirmware, auch ohne App oder Wall.

Je Richtung gelten mindestens 60 und höchstens 180 Sekunden. Nach der Anlaufzeit werden alle fünf Sekunden Temperaturen erfasst. Über 30 Sekunden dürfen sie höchstens 0,2 °C schwanken und sich zwischen Anfang und Ende höchstens um 0,1 °C verändern; diese Bedingung muss weitere 30 Sekunden bestehen. Bei konstanten Werten ist typischerweise nach etwa 80 Sekunden ein Ergebnis verfügbar. Beide Lüfter müssen die aktuelle Richtung stabil bestätigt haben, bevor sie gemeinsam wechseln.

Ohne stabiles Ergebnis endet die Runde ohne neue Kühlfreigabe. Nach dem eingestellten Messintervall folgt ein neuer Versuch. Das Intervall zählt im adaptiven Modus ab Messende; laufende Messungen werden nicht unterbrochen. Sensorfehler, fehlende Gruppenfreigaben und Stillstand setzen die Messprüfung zurück. Die feste Messdauer bleibt auswählbar und ist bei bestehenden Einstellungen zunächst aktiv.

**Benötigte Versionen:** Android **3.3.25**, Lüfterfirmware **3.3.22 Beta auf allen Gruppenmitgliedern**, für die neue Wall-Auswahl **Wall 0.6.7 Beta**. Zuerst die App, danach alle beteiligten Lüfter und gegebenenfalls Wall aktualisieren. Gleiche Sommerparameter aller Gruppenlüfter sind erforderlich. Gemischte Firmwarestände erhalten keine automatische Kühlfreigabe.

**Auswahl:** App → Gruppeneinstellungen → Sommerautomatik; Wall → Gruppe → Sommer / Auto → Sommerautomatik → Messung: bis stabil; Wall-Webseite → Gruppenkarte; Lüfter-Webseite → Lüftungsart → Messdauer für die Gruppe. Speichern schaltet den Modus nicht automatisch ein. Die App und Wall prüfen individuelle Antworten. Die Lüfter-Webseite bestätigt lokal und meldet den Versand des Gruppenauftrags; den vollständigen Gruppenstand anschließend prüfen.

Stabile Sensorwerte allein beweisen noch nicht, dass der Wärmespeicher keinen Einfluss mehr hat. Die thermische Messgüte muss nach Installation am echten Lüfter mit einem unabhängigen Thermometer geprüft werden. Längere Messläufe können länger warme Außenluft hereinführen.

Automatisierte Regelungs-, Protokoll-, Build- und Bedienprüfungen durchgeführt; kein realer Gerätetest dieses Updates. Die Veröffentlichung installiert nichts automatisch. Einstellungen, Kopplungen und Einrichtungs-AP bleiben erhalten.

Für LILYGO T-Display ESP32 mit vorhandenem 16-MiB-Layout. Reguläres App-Slot-Update, kein Vollflash. Inventar und Kopplungen bleiben erhalten. Nextion HMI 302 bleibt unverändert; kein TFT-Update nötig. Die unveränderte TFT-Datei liegt der Vollständigkeit halber bei.
