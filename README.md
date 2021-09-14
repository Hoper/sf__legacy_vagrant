# sf__legacy_vagrant

## Dependences
VirtualBox

https://www.oracle.com/ru/virtualization/technologies/vm/downloads/virtualbox-downloads.html

You need install Vagrant, look here https://www.vagrantup.com/downloads
```sh
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install vagrant
```

## Installation
```sh
git clone https://github.com/Hoper/sf__legacy_vagrant
cd sf__legacy_vagrant
vagrant up
vagrant ssh
```
you will get ubuntu 20.04 and PstGreSQL 8.4
