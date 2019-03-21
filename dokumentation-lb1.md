# Dokumentation LB 1
**Zum Modul 300 von Marius Rutz**
***
## Inhaltsverzeichnis

* Persönlicher Wissensstand
* Toolumgebung
* Ubuntu mit Apacheserver
  
## Persönlicher Wissensstand

**Linux**  
In Modulen an der TBZ spärlich genutzt. Auf privaten Computern verwende ich Ubuntu.
Im Geschäfft verwenden wir Windows.
**Virtualisierung**  
VMware im Geschäfft und in der Schule verwendet. Aktuell den ÜK zum Thema absolviert. In der Schule in diversen Modulen genutzt.
**Vagrant**  
Noch nie benutzt vor M300.  
**Systemsicherheit**  
Wenig Erfahrung im konfigurieren von Firewalls. 
## Lernumgebung
**Git**  
Gemäss Anleitung im M300 Reppository:  
*Github*
  1. Auf www.github.com ein Benutzerkonto erstellen (Angabe von Username, E-Mail und Passwort)
  2. E-Mail zur Verifizierung des Kontos bestätigen und anschliessend auf GitHub anmelden

*Repository*
1. New Repository auswählen
2. Name: M300
3. Public
4. Initialize this repository with a README auswählen
5. Create a repository

*Git Client*  
Git-2.20.1-64-bit.exe als Administrator ausführen.  
Standardwerte wurden während der Installation verwenden.  
Konfiguration mit:  
 $ git config --global user.name "<Payreno>"
 $ git config --global user.email "<marius.rutz@protonmail.ch>"  

*SSH Key*  
ssh-keygen -t rsa -b 4096 -C "marius.rutz@protonmail.ch"  
Enter a file in which to save the key (~/.ssh/id_rsa): [Press enter]  
Enter passphrase (empty for no passphrase): []  
Enter same passphrase again: [] 
*%HOME%/.ssh/id_rsa.pub mit Notepad öffnen und Schlüssel kopieren  
Auf Github unter Settings->SSH and GPG keys angeben

*Repository klonen*  
Modulrepo:  
  * git clone https://github.com/mc-b/M300  
  * cd M300  
  * git pull  
  * git status
     
Meinrepo:  
  * git clone git@github.com:Payreno/M300.git  
  * git pull --> Um zu aktualisieren  
  * git status --> Um  Status der lokalen Kopie anzuzeigen  





**Virtualbox**  
**Vagrant**  
**Visualstudio Code**  


## Visualstudio-Code

## Ubuntu mit Apacheserver

#PIHole