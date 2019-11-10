# TIA_EmptyWorkingSet

## Übersicht

Die Speicherverwaltung des TIA-Portals von Siemens ist seit Jahren nicht die beste.
Dieses kleine Programm schafft hier etwas Abhilfe.


Dieses kleine Programm prüft alle 10 Sekunden ob der Speicher der Prozesse:
```
Siemens.Automation.Portal.exe > 600 MB
Siemens.Automation.ObjectFrame.FileStorage.Server.exe > 400 MB
```

Wenn ein Fall davon zutrifft, führt das Programm bei dem entsprechenden Prozess ein [EmptyWorkingSet](https://docs.microsoft.com/en-us/windows/win32/api/psapi/nf-psapi-emptyworkingset) durch.

### Voraussetzungen

:warning: Wenn der Rechner nicht den Hardware-Vorraussetzungen entspricht (16 GB RAM), kann dieses Tool die Speicher-Probleme durch das TIA-Portal auch nicht verhindern, sondern nur etwas hinauszögern.

### Installation (Windows)

Einfach die EXE starten. 


## Author
Thorsten Willert [Homepage](http://www.thorsten-willert.de/)

PsaltyDS at http://www.autoitscript.com/forum

## Lizenz
Das ganze steht unter der [Apache 2.0](https://github.com/THWillert/HomeMatic_CSS/blob/master/LICENSE) Lizenz.
.
