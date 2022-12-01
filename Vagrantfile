Vagrant.configure("2") do |config|
  config.vm.define "rhel8" do |rhel8|
    rhel8.vm.box = "generic/rhel8"
    rhel8.vm.network "private_network", ip: "192.168.58.10"
    rhel8.vm.hostname = "rhel8"
    rhel8.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
    #rhel8.vm.network "forwarded_port", guest: 80, host: 8090
  end
  config.vm.define "stream" do |stream|
    stream.vm.box = "centos/stream8"
    stream.vm.network "private_network", ip: "192.168.58.11"
    stream.vm.hostname = "stream"
    stream.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/focal64"
    ubuntu.vm.network "private_network", ip: "192.168.58.12"
    ubuntu.vm.hostname = "ubuntu"
    ubuntu.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
end
