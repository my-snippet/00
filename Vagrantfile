# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.provider "virtualbox" do |vb|
    config.vm.network "private_network",
                      # :type => 'dhcp',
                      # :name => 'vboxnet0',
                      :ip => ENV['VBOXNET0_IP'],
                      :adapter => 2
  end

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "provision.yml"
  end
end
