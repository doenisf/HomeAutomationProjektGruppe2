# FHEM Setup

Um das FHEM Setup herzustellen, musst du auf Basis der vorherigen Ausgangssituation weitermachen. Solltest du den PuTTY bereits geschlossen haben, so beginnst du bei Kapitel 1.1 mit dem Schritt 7. Solltest du soweit sein kannst du mit den folgenden Schritten weitermachen. <br/>

<ol>
<li>
Befehl<br>

```
sudo wget -O- https://debian.fhem.de/archive.key | gpg --dearmor | sudo tee /usr/share/keyrings/debianfhemde-archive-keyring.gpg
```
</li>
<li>
Wechsel ins Verzeichnis “/etc/apt/“. Hierhin gelangst du mit dem cd Befehl ( <code>cd /etc/apt/</code> à Enter) ins Verzeichnis.
</li>
<li>
Öffne die Datei „sources.list“. Hierfür kannst du den Befehl <code>sudo nano sources.list</code> nutzen.
<ol>
<li>
Füge in die geöffnete Datei  

```
deb [signed-by=/usr/share/keyrings/debianfhemde-archive-keyring.gpg] https://debian.fhem.de/nightly/ /
``` 
ein.
</li>
<li>
Speicher die Datei mit der Taste F3 à Enter
</li>
<li>
Schließe die Datei mit Strg + x
</li>
</ol>
</li>
<li>
Befehl <code>sudo apt update</code>
</li>
<li>
Befehl <code>sudo apt install fhem</code> und gegebenenfalls mit <code>Y</code> bestätigen.
</li>
</ol>

Nächster Schritt: [FTUI Setup](/01_Setup%20Raspberry%20Pi/03_FTUI%20Setup.md)
