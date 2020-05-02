Vagrant.configure("2") do |config|
  config.vm.box = "gbailey/amzn2"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "tests/test.yml"
    ansible.become = true
    ansible.limit = "all"
    ansible.compatibility_mode = "2.0"
  end
end
