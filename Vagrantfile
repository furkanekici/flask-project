Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-24.04"
  config.vm.network "forwarded_port", guest: 5000, host: 5000
  config.vm.network "private_network", ip: "192.168.56.10"

  config.vm.define "trusty" do |node|
    node.vm.hostname = "trusty.local"
  end

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.cpus = "2"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "main.yml"
  end

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
  SHELL
end

