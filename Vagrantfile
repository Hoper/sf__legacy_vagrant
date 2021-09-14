# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.provision "shell", inline: <<-SHELL
    echo "deb http://apt.postgresql.org/pub/repos/apt/ focal-pgdg main" | sudo tee -a /etc/apt/sources.list.d/pgdg.list
    wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
    sudo apt-get update
    sudo DEBIAN_FRONTEND=noninteractive apt-get -y install postgresql-8.4
    #sudo apt-get install postgresql-8.4 -y -f
    #apt-get install -y apache2
  SHELL
end
