# -*- mode: ruby -*-
# vi: set ft=ruby :
#
# cpu = # cpu per VM
cpu = 1

#
# mem = MB ram per VM
#
mem = 512

Vagrant.configure(2) do |config|

    #
    # vm specs
    #
  config.vm.provider "virtualbox" do |v|
    v.memory = mem
    v.cpus = cpu
  end

  #
  # Use insecure key
  config.ssh.insert_key = false
  #

  config.vm.define "ansible" do |node|
    node.vm.box = 'centos/7'
    node.vm.hostname = 'ansible'
    node.vm.network :forwarded_port, guest: 22, host: 2222, id: "ssh"
    node.vm.network "private_network", ip: "10.0.0.10"

    puts "Provisioning with Ansible started"
    node.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
      ansible.limit = "all"
    end
  end
end
