# sf__legacy_vagrant

You need install Vagrant, look here https://www.vagrantup.com/downloads

curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install vagrant

then

git clone https://github.com/Hoper/sf__legacy_vagrant
cd sf__legacy_vagrant
vagrant up
vagrant ssh
