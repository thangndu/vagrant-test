
Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  # management server
  config.vm.define "mgmt" do |mgmt|
    mgmt.vm.hostname = "mgmt"
    mgmt.vm.network "private_network", ip: "192.168.56.200"
  end   

  # application server
  config.vm.define "app" do |app|
    app.vm.hostname = "app"
    app.vm.network "private_network", ip: "192.168.56.202"
  end   

  # database server
  #config.vm.define "db" do |db|
  #  db.vm.hostname = "db"
  #  db.vm.network "private_network", ip: "192.168.56.203"
  #end
  

  
  # ansbile provision
  #config.vm.provision "ansible" do |ansbile|
  #  ansbile.playbook = "playbook.yml"
  #end  

  # SHELL
  #config.vm.provision "shell", inline: <<-SHELL
  #  pip install flask
  #SHELL

end
