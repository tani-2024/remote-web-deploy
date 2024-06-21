Vagrant.configure("2") do |config|
  # Define the first CentOS VM
  config.vm.define "centos1" do |centos1|
    centos1.vm.box = "centos/7"
    centos1.vm.hostname = "scriptbox"
    centos1.vm.network "private_network", ip: "192.168.56.11"
    centos1.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end

  # Define the second CentOS VM
  config.vm.define "centos2" do |centos2|
    centos2.vm.box = "centos/7"
    centos2.vm.hostname = "web02-centos"
    centos2.vm.network "private_network", ip: "192.168.56.12"
    centos2.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end

  # Define the Ubuntu VM
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/bionic64"
    ubuntu.vm.hostname = "web03-ubuntu"
    ubuntu.vm.network "private_network", ip: "192.168.56.13"
    ubuntu.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end
end
