# LB2_m122_Bash_ausslastung_ueberwachenSkript_Inf24D_Betsch_Gigly
Projektname: Systemressourcen-Monitoring

Ziel: Automatisierte Überwachung der CPU- und RAM-Auslastung auf einem Linux-System. 
Das Script liest alle 5 Minuten die Auslastungswerte aus, speichert sie in einer Logdatei 
und schreibt eine Warnmeldung, falls die Werte über definierte Schwellwerte steigen.

Das Script arbeitet ohne Benutzereingabe und führt eine Fehlerprüfung durch, 
z.B. prüft Schreibrechte auf die Logdatei und gültige Datenwerte.

Das Script kann in einem Cronjob ausgeführt werden und besitzt eine Konfigurationsdatei, 
um Schwellwerte und Logpfad flexibel anzupassen.
