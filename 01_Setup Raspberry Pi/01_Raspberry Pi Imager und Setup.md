# Raspberry Pi Imager und Setup

1.	Rufe die Website www.raspberrypi.com/software/ auf
2.	Lade den Raspberry Pi Imager für dein Betriebssystem (Windows/macOS/Ubuntu for x86) die passende Version herunter.
3.	Stecke die SD-Karte in den SD-Kartenleser deines Computers. 
4.	Installiere den Raspberry Pi Imager, indem du den Download durch einen Doppelklick startest. <br />
4.1.	Wähle das Betriebssystem „Raspberry PI OS (32 Bit)“ aus.<br />
4.2.	Drücke anschließend die Tasten Strg+shift+x, sodass sich ein weiteres Fenster mit „Erweiterten Optionen“ öffnet.<br />
4.2.1.	Setze den Hacken bei „SSH aktivieren“. Wähle ein Passwort für die Authentifizierung aus und lege ein Passwort für den Raspberry Pi fest.<br />
![](/Bilder/01_1-1_SSH_aktivieren.png)<br/>
4.2.2.	Scrolle in den Erweiterten Optionen nach unten und richte dein Wifi ein. Trage hierfür unter SSID den Netzwerk Name und unter Passwort das Netzwerkpasswort ein <br/>
![](/Bilder/01_1-1_WiFi_einrichten.png)<br/>
4.2.3.	Lege die Spracheinstellungen fest<br/>
![](/Bilder/01_1-1_Sprache.png)<br/>
4.2.4.	Speicher deine Änderungen.<br/>
4.3.	Wähle die entsprechende SD-Karte, die du nutzt, aus.<br/>
4.4.	Führe den Button „Schreiben“ durch Anklicken aus und klicke dich mit der weiter Taste durch die Installation bis du am Ende angekommen bist und der Installationsteil abgeschlossen ist.<br/>
4.4.1.	Sollten noch Daten auf der SD-Karte vorhanden sein, drücken sie in der Auswahl, dass alle vorherigen Daten gelöscht werden dürfen. Bitte beachten sie, dass nach einer Überschreibung keine Daten wiederhergestellt werden können.<br/>
5.	Entferne die SD-Karte aus dem SD-Kartenleser deines Computers und stecke sie in den Raspberry Pi. Den Raspberry Pi musst du folgend an das Stromnetz, an einen Bildschirm mit HDMI-Eingang (Computer), sowie vorteilhaft an eine Maus und eine Tastatur anschließen.<br/>
5.1.	Warte bis der Raspberry Pi sich mit deinem WLAN verbunden hat.<br/>
6.	Lade dir auf dem PC/Laptoop PuTTY von der Website www.putty.org/ herunter und installiere dies.<br/>
7.	Starte den PuTTY und verbinde ihn mit dem Raspberry Pi.<br/>
8.	Trage unter Host Name (or IP address) entweder den Gerätenamen (siehe 8.1) des Raspberry Pi oder die IP-Adresse (siehe 8.2) ein.<br/>
8.1.	Gib unter Host Name (or IP address) „raspberrypi“ ein. Folgende Meldung erscheint, welche du mit „Accept“ bestätigen musst. <br/>
![](/Bilder/01_1-1_PuttyAlert.png)<br/>
8.2.	Alternativ: Öffne die Kommandozeile auf dem RaspberryPi und führe den Befehl: „ifconfig“ aus.  Dort kannst du nun die IP-Adresse des Raspberry Pi’s ablesen.<br/>
8.3.	Trage den Wert 22 unter Port ein.<br/>
8.4.	Wähle SSH bei Connection type aus.<br/>
![](/Bilder/01_1-1_PuttyConfig.png)<br/>
9.	PuTTY-Eingaben:<br/>
9.1.	Login as: „pi“ à Enter<br/>
9.2.	Password: Passwort aus Schritt 4.2.1. à Enter<br/>
![](/Bilder/01_1-1_PWabfrage.png)<br/>
9.3.	Eingabe 1: „sudo apt update“ à Enter<br/>
9.4.	Eingabe 2: „sudo apt upgrade“ à Enter (ggfs. zusätzliche Bestätigung mit „Y“ à Enter)<br/>



Nächster Schritt: **[FHEM Setup](https://github.com/doenisf/HomeAutomationProjektGruppe2/blob/main/01_Setup%20Raspberry%20Pi/02_FHEM%20Setup.md)**
            
