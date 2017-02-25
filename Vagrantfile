# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.network "forwarded_port", guest: 4000, host: 4000

  config.vm.synced_folder ".", "/vagrant", fsnotify: true

  config.vm.provision "ansible" do |ansible|
      ansible.playbook = "provision.yml"
  end
end
