# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.ssh.insert_key = false

  config.vm.provider :virtualbox do |vb|
    vb.memory = 1024
    vb.cpus = 2
  end

  config.vm.synced_folder "./app", "/home/vagrant/app"

  config.vm.define 'ubuntu' do |ubuntu|
    ubuntu.vm.box = "bento/ubuntu-16.04"
    ubuntu.vm.network :private_network, ip: '192.168.33.112'
  end

  # config.vm.define 'centos' do |centos|
  #   centos.vm.box = "bento/centos-6"
  #   centos.vm.network :private_network, ip: '192.168.33.113'
  # end
end
