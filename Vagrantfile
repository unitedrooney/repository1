Vagrant.configure("2") do |config|
   
  config.vm.define "master" do |subconfig|
	subconfig.vm.box = "ubuntu/trusty64"
    subconfig.vm.hostname = "master"
	subconfig.vm.network "private_network", ip: "192.168.10.12"

	subconfig.vm.synced_folder ".", "/vagrant", type: "virtualbox"

	subconfig.vm.provider "virtualbox" do |vb|
     vb.memory = "512"
	 vb.cpus = "1"
	end
	 
  end 
  
  config.vm.define "slave" do |subconfig|
	subconfig.vm.box = "ubuntu/trusty64"
    subconfig.vm.hostname = "slave"
	subconfig.vm.network "private_network", ip: "192.168.10.13"

	subconfig.vm.synced_folder ".", "/vagrant", type: "virtualbox"

	subconfig.vm.provider "virtualbox" do |vb|
     vb.memory = "512"
	 vb.cpus = "1"
	end
	
  end 
  
    config.vm.define "slave2" do |subconfig|
	subconfig.vm.box = "ubuntu/trusty64"
    subconfig.vm.hostname = "slave2"
	subconfig.vm.network "private_network", ip: "192.168.10.14"

	subconfig.vm.synced_folder ".", "/vagrant", type: "virtualbox"

	subconfig.vm.provider "virtualbox" do |vb|
     vb.memory = "512"
	 vb.cpus = "1"
	end
	
  end 
  
  
  
end