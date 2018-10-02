# _*_ mode: ruby _*_
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "geerlingguy/centos7"
  config.ssh.insert_key = false
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.provider :virtualbox do |v|
    v.memory = 256
    v.linked_clone = true
  end

  # Application server 1
  config.vm.define "app1" do |app|
    app.vm.hostname = "orc-app1.dev"
    app.vm.network :private_network, ip: "10.0.0.2"
  end

  # Application server 2
  config.vm.define "app2" do |app|
    app.vm.hostname = "orc-app2.dev"
    app.vm.network :private_network, ip: "10.0.0.3"
  end

  # Database server
  config.vm.define "db" do |db|
    db.vm.hostname = "orc-db.dev"
    db.vm.network :private_network, ip: "10.0.0.4"
  end
end
