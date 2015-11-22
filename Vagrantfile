# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "base"

  # Shell provisioner to setup basic environment.
  config.vm.provision :shell, :inline => "/vagrant/blogatico-dependencies"

  # Forwarded ports
  config.vm.network "forwarded_port", guest: 80, host: 8081
end
