# FHEM Setup

Um das FHEM Setup herzustellen, musst du auf Basis der vorherigen Ausgangssituation weitermachen. Solltest du den PuTTY bereits geschlossen haben, so beginnst du bei Kapitel 1.1 mit dem Schritt 7. Solltest du soweit sein kannst du mit den folgenden Schritten weitermachen. <br/>
1.	Befehl: <br/>
    
    “sudo wget -O- https://debian.fhem.de/archive.key | gpg --dearmor | sudo tee /usr/share/keyrings/debianfhemde-archive-keyring.gpg”


2.	Wechsel ins Verzeichnis “/etc/apt/“. Hierhin gelangst du mit dem cd Befehl ( „cd /etc/apt/“ à Enter) ins Verzeichnis.
3.	Öffne die Datei „sources.list“. Hierfür kannst du den Befehl „sudo nano sources.list“ nutzen.
3.1.	Füge in die geöffnete Datei  
„deb [signed-by=/usr/share/keyrings/debianfhemde-archive-keyring.gpg] https://debian.fhem.de/nightly/ /“ ein.
3.2.	Speicher die Datei mit der Taste F3 à Enter
3.3.	Schließe die Datei mit Strg + x
4.	Befehl: „sudo apt update“
5.	Befehl: „sudo apt install fhem“ (ggfs. zusätzliche Bestätigung mit „Y“ à Enter)
