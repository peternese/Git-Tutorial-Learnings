# Wichtige Learnings aus dem Github Tutorial

Tutorial Referenz von freecodecamp: https://www.youtube.com/watch?v=RGOj5yH7evk&t=1494s

# Terminal Befehle

Leeren des Terminals:  
$ clear 

Ordner wechseln, Directory changen:  
$ cd Name 

Ordner wechseln, Directory changen eine Ebene höher:
$ cd ../Name 

Auflisten der vorhandenen Dateien:
$ ls 

Auflisten der vorhandenen Dateien + Systemdateien/versteckte Libraries: 
$ ls -la 

Statusabfrage der git notierten Dateien im Ordner: 
$ git status 

Git Befehlhilfe: 
$ git help 

Hinzufügen von Dateien ins Repository: 
$ git add Name / . <- für alle 

Ordner als Repository initialisieren:
$ git init   -b NAME optional um die branch zu definieren 

Bevor ein Push geschieht, muss ein origin master festgelegt werden, in dem Falle von github, remote das github repository: 
$ git remote add origin https://github.com/peternese/Git-Tutorial-Learnings.git 

Bevor gepusht wird, wird der commit bezeichnet mit einem Titel und einer Beschreibung: 
$ git commit -m 'Titel hier' -m 'Beschreibung hier' 

Der Push erfolgt im Anschluss und committed das repository: 
$ git push origin master 

Für zukünftige lässt sich der Befehl abkürzen das nur noch git push benötigt wird: 
$ git push -u origin master 

