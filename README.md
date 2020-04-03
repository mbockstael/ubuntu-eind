![Linux logo](https://www.putorius.net/wp-content/uploads/2019/01/tux.jpg "TUX")

# Linux praktijkopdracht
Het afsluiten van het vak Linux gebeurt door het maken van een praktijkopdracht.In deze praktijkopdracht zullen de  ***meeste*** onderwerpen uit de eerdere lessen terugkomen.

## Voorwaarden software

De volgende software is nodig

* Virtualbox 5.0 of hoger
* Git bash voor Windows
* Vagrant 2.2.6 of hoger

Installatie voor Windows

* Installeer Virtualbox: https://www.virtualbox.org/wiki/Downloads
* Installeer Git bash for Windows: https://gitforwindows.org/
* Installeer Vagrant for Windows: https://www.vagrantup.com/downloads.html


## Het starten van vagrant
Open <b>Git Bash</b> in Windows en typ de volgende commandos

1. cd Documents
2. mkdir vagrant && cd vagrant
3. git clone https://github.com/mbockstael/ubuntu-eind.git
4. **cd ubuntu-eind**
5. vagrant up
6. vagrant ssh

## Opdracht

Je vind je opdracht in ***~/vagrant/opdracht***

## Network
De Vagrant VM zal 2 netwerk adapters hebben
```
Nat : DHCP
Localhost : 192.168.10.101
```
## Vagrant commandos
Vagrant VM opstarten
```
vagrant up
```
Stoppen en afsluiten van de VM
```
vagrant halt
```
Verwijderen van een VM
```
vagrant destroy
```
ssh naar de VM
```
vagrant ssh Ubuntuserver
```
