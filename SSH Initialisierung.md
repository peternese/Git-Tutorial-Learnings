# Der erste Schritt ist eine SSH Initialisierung

Folger der folgenden Anleitung um eine SSH-Initialisierung vorzunehmen über das Teriminal:  
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Zu beachten, ist die Variablen und Bezeichnungen nach den eigenen Namen zu richten und zu benennen.  
Bei der Key Erstellung ist zu beachten, den public key auszuwählen zur Erstellung für die Github Settings,  
bei den Variablen im Computer (.ssh Ordner erstellen und config beschreiben und agent starten) soll allerdings  
die ssh key datei ohne .pub verwendet werden. Coole Befehler aus dem Tutorial von Freecodecamp:  

$ cat DATEINAME.pub  
Öffnet den key der pub datei und zeigt ihn an.

$ ls | grep DATEINAME  
Sucht nach der Erstellung des Keygens die Datei und zeigt die an.