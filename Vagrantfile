Vagrant.configure("2") do |config|
  # Linux OS CentOS
  config.vm.box = "geerlingguy/centos7";
  config.vm.network "public_network"
  # Web server
  config.vm.define "db-server" do |db|
    db.vm.hostname = "mongodb";
    # static ip address
    db.vm.network :private_network, ip: "192.168.60.4"
  end
end