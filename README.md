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

Neue branches erstellen funktioniert auch.  
So erstellt man neue Branhes wenn man änderungen vornehmen will geonsdern von der production so bspw. eine staging branch oder dev branch  
Dazu lassen sich explizit neue Branches erstellen via:  
$ git checkout -b NAME der branch

sobald diese erstellt wurde kann man sich anschauen welche branches existieren und in welcher branch man sich aktuell befindet:  
$ git branch

Änderungen in der einen Branch sind it der anderen branch zu vergleichen über:  
$ git diff NAME

Möchte man verkürzt eine Änderung committen geht es auch ohne den add befehl und nur über commit:  
$ git commit -am 'UPDATE TITEL'

Standartäßig erstellt man wenn man seine Änderungen imm anderen branch fertig hat einen push auf die branch vor,  
Wenn man allerdings seine abseitige branch updaten möchte mit andererer Änderungen in der main branch,  
muss man seine branch mit den updates der main branch erstmal up to date führen:  
$ git merge BEZUGSBRANCH

-> Achtung es führt erstmal zu einem Konflikt, dieser ist einfach zu beheben mit cmd + shift k lassen sich die lines löschen die man nicht will,  
oder bspw. in vs code mit buttons die schon zur verfügung stehen, danach erneut committen  

Committete changes können nach dem commit aufgehoben werden, der commit wird resettet:  
$ git commit reset

Es lässt sich über die letzten commmits Übersicht fliegen mit dem Befehl:  
$ git log

Mit dem Hash eines commits lässt sich direkt zu einer stagings der letzten commits fliegen:  
$ git reset HASH

Wenn man aber die changes voll rückgängig machen möchte und löschen will:  
$ git reset --hard HASH


## Forking

Wenn man forkt, kann man ein beliebiges repository nehmen, und auf fork klicken.  
Dadurch dupliziert man das repository in ein eigenes, und kann somit den inhalt auf die eigene maschine pullen.  
Änderungen durchführen committen und testen und final dann auch pushen. Sobald man ein Ergebnis erzielt hat und  
es in das Ursprungs repository zuführen möchte, isst ein pull request an den owner des Ursprungsrepos notwendig.