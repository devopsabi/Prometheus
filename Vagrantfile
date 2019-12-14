Vagrant.configure("2") do |config|
    
    config.vm.define "prometheus" do |prometheus|

      prometheus.vm.box = "centos/7"

      prometheus.vm.network "private_network", ip: "192.168.33.10"
      prometheus.vm.hostname = "prometheus-node"

      prometheus.vm.provider "virtualbox" do |vb|
         vb.gui = false
         vb.memory = "2048"
      end
        

    end
    
    
    config.vm.define "node01" do |node01|

      node01.vm.box = "centos/7"

      node01.vm.network "private_network", ip: "192.168.33.11"
      node01.vm.hostname = "node01"
        
      node01.vm.provider "virtualbox" do |vb|
         vb.gui = false
         vb.memory = "1024"
      end
    end
    
    config.vm.define "node02" do |node02|

      node02.vm.box = "centos/7"

      node02.vm.network "private_network", ip: "192.168.33.12"
      node02.vm.hostname = "node02"
        
      node02.vm.provider "virtualbox" do |vb|
         vb.gui = false
         vb.memory = "512"
      end
    end
end



