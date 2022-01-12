Vagrant.configure("2") do |config|
  config.vm.box = "generic/debian11"
  config.vm.hostname = "??????"
  config.vm.provider "virtualbox" do |v|
    # v.gui = true
    v.name = "?????????"
    v.memory = 2048
    v.cpus = 2
    v.customize ['modifyvm', :id, '--clipboard', 'bidirectional']     
  end
  
  config.vm.network "forwarded_port", guest: ??, host: ???? 
  config.vm.network "forwarded_port", guest: ??, host: ????
         
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update -y
    sudo apt-get upgrade -y
    sudo apt-get install -y net-tools
    sudo apt-get install -y aptitude
    sudo apt-get install -y whois
    sudo apt-get install -y apache2 apache2-doc libapache2-mod-php php7.3 
    sudo apt-get install -y openssh-server openssh-sftp-server
    sudo groupadd -g ???? ??????
    sudo useradd  ?????? -u ???? -g ?????? -d /home/?????? -m -s /bin/bash -p $(mkpasswd ??????????)  
  SHELL

end
