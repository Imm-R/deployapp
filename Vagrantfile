Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.ssh.forward_agent = true
  config.vm.hostname = "dev-simple"
  config.vm.box_check_update = false
  config.vm.network :private_network, ip: "10.245.1.222"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
 end

end

