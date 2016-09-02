
Vagrant.configure(2) do |config|
  config.vm.define "gateone-test" do |conf|
    conf.vm.box = "ubuntu/trusty64"
    # helpful for recovery from `virtualbox` console
    conf.ssh.username = "vagrant"
    conf.ssh.password = "vagrant"
    conf.vm.hostname = "gateone.atmo.cloud"
    conf.vm.network "private_network", ip: "192.168.72.33"
    conf.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

  if Vagrant.has_plugin?("vagrant-cachier")
    config.cache.scope = :box
  end
end
