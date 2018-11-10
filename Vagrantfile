# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = 'bento/ubuntu-16.04'
  config.ssh.insert_key = false

  config.vm.provider :virtualbox do |vb|
    vb.memory = 1024
    vb.cpus = 2
  end

  config.vm.define 'server' do |app|
    app.vm.network :private_network, ip: '192.168.33.112'
  end
end
