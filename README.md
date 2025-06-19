# LB2_m122_Bash_ausslastung_ueberwachenSkript_Inf24D_Betsch_Gigly
Projektname: Systemressourcen-Monitoring

Ziel: Automatisierte Überwachung der CPU- und RAM-Auslastung auf einem Linux-System. 
Das Script liest alle 5 Minuten die Auslastungswerte aus, speichert sie in einer Logdatei 
und schreibt eine Warnmeldung, falls die Werte über definierte Schwellwerte steigen.

Das Script arbeitet ohne Benutzereingabe und führt eine Fehlerprüfung durch, 
z.B. prüft Schreibrechte auf die Logdatei und gültige Datenwerte.

Das Script kann in einem Cronjob ausgeführt werden und besitzt eine Konfigurationsdatei, 
um Schwellwerte und Logpfad flexibel anzupassen.







Bereich	Beschreibung
Ziel	Automatisierte Überwachung von CPU- und RAM-Auslastung auf einem Linux-System
Eingabedaten	Systeminterne Daten: CPU- und RAM-Auslastung über /proc oder top
Verarbeitung	Auslesen der Werte, Vergleich mit definierten Schwellwerten, Fehlerprüfung
Ausgabe	Logdatei mit Zeitstempel, Warnmeldung bei Überschreitung der Schwellwerte
Fehlerbehandlung	Meldung bei nicht auslesbaren Daten, Abbruch bei fehlenden Schreibrechten auf Logdatei
Automatisierung	Ausführung als Cronjob alle 5 Minuten
Konfiguration	Konfigurationsdatei monitor.cfg für Schwellwerte und Logpfad
Anforderungen an das Script	Keine Benutzereingaben nötig, robust gegen Fehler, klare Logs
Schnittstellen	Zugriff auf Linux-Systemdaten, Logdatei, Cronjob
Abhängigkeiten	Linux-Bash Umgebung, Standardbefehle wie top, awk, date
