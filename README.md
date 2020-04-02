# Linux eindopdracht
De eindopdracht Linux N3 leerjaar 2

## Voorwaarden software

De volgende software is nodig
```
* Virtualbox 5.0 or hoger
* Git bash voor Windows
* Vagrant 2.2.6 or hoger
```
Installatie
```
* Installeer Virtualbox: https://www.virtualbox.org/wiki/Downloads
* Installeer Git bash for Windows: https://gitforwindows.org/
* Installeer Vagrant for Windows: https://www.vagrantup.com/downloads.html
```

## Het starten van vagrant
Open <b>Git Bash</b> in Windows en typ de volgende commandos
```
cd Documents
mkdir vagrant && cd vagrant
git clone https://github.com/borahuho/DevOps1
cd DevOps1
vagrant up
vagrant ssh
```
## Opdracht
```
Je vind je opdracht in /opdracht
```
## Network
De Vagrant VM zal 2 netwerk adapters hebben
```
Nat : DHCP
Localhost : 192.168.10.4
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
