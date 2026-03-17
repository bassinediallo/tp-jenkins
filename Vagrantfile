Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/focal64"
    config.vm.hostname = "jenkins-server"
    config.vm.box_check_update = false
    config.vm.network "forwarded_port", guest: 8080, host: 9090
    config.vm.provider "virtualbox" do |vb|
      vb.memory = "4096"
      vb.cpus = 2
    end
  end