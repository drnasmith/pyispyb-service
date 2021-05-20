# For shared folders use geerlingguy/centos7 instead of centos/7
Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  config.vm.define "pyispyb" do |pyispyb|
    # Either use private network or expose ports on localhost
    pyispyb.vm.network "private_network", ip: "192.168.33.40"
    pyispyb.vm.hostname="pyispyb.example.org"

    # Comment out next two definitions if on Windows
    # pyispyb.vm.provision "ansible" do |ansible|
    #   ansible.playbook = "playbooks/pyispyb.yml"
    # end
  end

end
