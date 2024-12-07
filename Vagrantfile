# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "bento/debian-12"
  config.vm.define "imad"
  config.vm.hostname = "imaddine"
  config.vm.network "private_network", ip: "192.168.56.110"

  config.vm.provider "virtualbox" do |v|
    v.name = "cloud-vm"
    v.memory = 1024
    v.cpus = 1
  end

end