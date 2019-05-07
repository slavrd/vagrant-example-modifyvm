
Vagrant.configure("2") do |config|

  config.vm.box = "slavrd/nginx64"

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end

  vmCount = 1

  (1..vmCount).each do |i|

    vm_name = "vm%02d" % [i]
    config.vm.define vm_name do |m|
      m.vm.hostname = vm_name
    end

  end

end
