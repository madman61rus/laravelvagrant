Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/vivid64"

  config.vm.provision :shell, path: "bootstrap.sh"

# memory size
config.vm.provider "virtualbox" do |v|

# memory size
  v.memory = 1024

end

# forward network
  config.vm.network :forwarded_port, guest: 80, host: 8080
end
