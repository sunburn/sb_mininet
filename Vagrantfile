# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.ssh.forward_x11 = true
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get -qy install git
    sudo apt-get -qy install graphviz
    git clone git://github.com/mininet/mininet
    mininet/util/install.sh -a
    sudo mn --test pingall

  SHELL
end
