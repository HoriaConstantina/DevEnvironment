# STEPS TO INITIALIZE VAGRANT

- create new folder (mkdir folder_name)
- create new file Vagrantfile (nano Vagrantfile)
- go inside the Vagrantfile (nano Vagrantfile)
- inside the file paste the following:
	- Vagrant.configure("2") do |config|
	-  config.vm.box = "ubuntu/xenial64" 
	-  config.vm.network "private_network", ip: "192.168.10.100" 
	- end

- save the file (CTRL + X then Y then ENTER)
- run Git Bash as administrator
- type in the Git Bash terminal vagrant up
- check the status with vagrant status
- if the virtual machine is running do vagrant ssh
- once you are inside the virtual machine type sudo apt-get update -y
- then sudo apt-get upgrade -y
- then sudp apt-get install nginx -y
- open the browser and type in the URL: 192.168.10.100
- to destroy your vagrant type vagrant destroy
