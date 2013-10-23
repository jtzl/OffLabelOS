VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  time = Time.new
  config.vm.box = "OffLabelOS_v001"
  config.vm.hostname = "Off-Label-#{ENV['USER'].gsub('_','-')}-#{time.strftime('%Y%m%d%H%M%S')}"
  config.vm.provider :virtualbox do |vb|
     vb.gui = true
     vb.customize ["modifyvm", :id, "--memory", "2048"]
   end

end
