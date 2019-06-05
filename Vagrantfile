Vagrant.configure("2") do |config|

  (1..2).each do |i|
    config.vm.define vm_name="web0#{i}" do |node|
      node.vm.box = "krastin/xenial64"
      node.vm.hostname = vm_name
      node.vm.provision "shell", path: "provision/web.sh"
    end
  end

  config.vm.define vm_name="mysql" do |node|
    node.vm.box = "krastin/xenial64"
    node.vm.hostname = vm_name
    node.vm.provision "shell", path: "provision/mysql.sh"
  end
end
