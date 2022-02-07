Vagrant.configure("2") do |config|

  if Vagrant.has_plugin? "vagrant-vbguest"
    config.vbguest.no_install = true
    config.vbguest.auto_update = false
    config.vbguest.no_remote = true
  end

  config.vm.define :clienteCentOS do |clienteCentOS|
    clienteCentOS.vm.box = "centos/stream8"
    clienteCentOS.vm.network :private_network, ip: "192.168.56.2"
    clienteCentOS.vm.hostname = "clienteCentOS"
    end

  config.vm.define :servidorCentOS do |servidorCentOS|
      servidorCentOS.vm.box = "centos/stream8"
      servidorCentOS.vm.network :private_network, ip: "192.168.56.3"
      servidorCentOS.vm.hostname = "servidorCentOS"
      end
  end
