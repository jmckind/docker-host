Vagrant.configure(2) do |config|
    config.vm.box = "ubuntu/trusty64"
    config.vm.hostname = "docker-host"

    config.vm.provider "virtualbox" do |vb|
        vb.name = "docker-host"
        vb.memory = 2048
        vb.cpus = 2
    end

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "provision.yml"
    end
end
