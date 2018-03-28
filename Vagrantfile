VAGRANTFILE_API_VERSION = '2'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu-16.04"

  # VM
  config.vm.define :'host1' do |host|
    host.vm.hostname = 'host1'
    host.vm.network :private_network, ip: "127.168.100.13", netmask: "255.255.255.0"
  end

  config.vm.define :'host2' do |host|
    host.vm.hostname = 'host2'
    host.vm.network :private_network, ip: "127.168.100.14", netmask: "255.255.255.0"
  end
  
  config.vbguest.auto_update = false
end
