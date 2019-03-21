# Dokumentation LB 1
**Zum Modul 300 von Marius Rutz**
***
![M300](pictures/index.png)  
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
**Versionsverwaltung / Git**  
Keine.  
**Systemsicherheit**  
Wenig Erfahrung im Konfigurieren von Firewalls. 

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
1. Git-2.20.1-64-bit.exe als Administrator ausführen.  
2. Standardwerte wurden während der Installation verwenden.  
3. Öffnen und Konfiguration mit:  
 $ git config --global user.name "Payreno"  
 $ git config --global user.email "<marius.rutz@protonmail.ch>"  

*SSH Key*  
1. Im Terminal:
   * ssh-keygen -t rsa -b 4096 -C "marius.rutz@protonmail.ch"  
   * Enter a file in which to save the key (~/.ssh/id_rsa): [Press enter]  
   * Enter passphrase (empty for no passphrase): []  
   * Enter same passphrase again: []

2. *%HOME%/.ssh/id_rsa.pub mit Notepad öffnen und Schlüssel kopieren  
3. Auf Github unter Settings->SSH and GPG keys angeben

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
Virtualbox ist eine Opensource Virtualisierungssoftware.  
Für die Verwendung im Modul reicht die Installation mit Standardwerten.

**Vagrant**  
Vagrant ermöglicht es, dass ich in Virtualbox automatisiert eine VM mit Service installieren kann.  
Für die Verwendung im Modul reicht die Installation mit Standardwerten.  

**Visualstudio Code**  
Visualstudio Code ist ein Editor von Microsoft. Es ist möglich ein Repository darin zu öffnen und Änderungen gleich zu pushen.  
Für die Verwendung im Modul reicht die Installation mit Standardwerten.  
Zusätzlich instalierte folgende 3 vorgegebenen Extensions:

* Markdown All in One
* Vagrant Extension
* vscode-pdf Extension  

Sie ermöglichen das einfachere bearbeiten von dieser Dokumentation und dem Vagrant file.

Damit beim Dateien mit den Endungen .git / .svn / .hg / .vagrant / .DS_store nicht in das Repository hinaufgeladen werden, habe ich im setting.json file folgenden code eingefügt:
   // Konfiguriert die Globmuster zum Ausschließen von Dateien und Ordnern.
 "files.exclude": {
   "**/.git": true,
   "**/.svn": true,
   "**/.hg": true,
   "**/.vagrant": true,
   "**/.DS_Store": true
 },  
 Allerdings musste ich feststellen, dass der in der Anleitung beschriebene Abschnitt nicht existiert. 


## Virtualbox  

Vagrant

Ubuntu mit Apacheserver

## Vagrant
Folgende Befehle werden verwendet um Vagrant über die Kommandozeile zu steuern:

