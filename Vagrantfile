$useraddscript = <<SCRIPT
useradd -m martijn
usermod -aG sudo martijn
echo martijn:Welcome01 | chpasswd

SCRIPT


Vagrant.configure('2') do |config|
    config.ssh.insert_key = false

    # set default settings
    config.vm.box = "ubuntu/bionic64"
    config.vm.provider "virtualbox" do |vb|
        vb.memory = 2048
        vb.cpus = 1
    end

	# set vm name and network
    config.vm.define :Ubuntu_eind, primary: true do |machine|
        machine.vm.host_name = "ubuntu.local"
        machine.vm.network "private_network", ip: "192.168.10.101"

        machine.vm.provider "virtualbox" do |vb|
            vb.cpus = 1
        end

	# Copy from folder to notes
        machine1.vm.provision "shell", inline: $useraddscript
        machine.vm.synced_folder "Opdracht/", "/home/vagrant/opdracht"
        machine.vm.provision "file", source: "~/.vagrant.d/insecure_private_key", destination: "$HOME/.ssh/id_rsa"
    end
end
