# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname = "dev.local"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "devbox"
    vb.memory = 4096
    vb.cpus = 2
  end

  # ntop
  config.vm.network "forwarded_port", guest: 3000, host: 3000
  # mysql
  config.vm.network "forwarded_port", guest: 3306, host: 3306
  # postgresql
  config.vm.network "forwarded_port", guest: 5432, host: 5432
  # redis
  config.vm.network "forwarded_port", guest: 6379, host: 6379
  # rabbitmq
  config.vm.network "forwarded_port", guest: 5672, host: 5672
  config.vm.network "forwarded_port", guest: 15672, host: 15672
  # riak
  config.vm.network "forwarded_port", guest: 8087, host: 8087
  config.vm.network "forwarded_port", guest: 8098, host: 8098
  # mongodb
  config.vm.network "forwarded_port", guest: 27017, host: 27017
  # zookeeper
  config.vm.network "forwarded_port", guest: 2181, host: 2181
  # elasticsearch
  config.vm.network "forwarded_port", guest: 9200, host: 9200
  # kafka
  config.vm.network "forwarded_port", guest: 9092, host: 9092
  # mesos
  config.vm.network "forwarded_port", guest: 5050, host: 5050
  # marathon
  config.vm.network "forwarded_port", guest: 8080, host: 8080
  # riemann
  config.vm.network "forwarded_port", guest: 5555, host: 5555
  # riemann dashboard
  config.vm.network "forwarded_port", guest: 4567, host: 4567
  # influxdb
  config.vm.network "forwarded_port", guest: 8083, host: 8083
  config.vm.network "forwarded_port", guest: 8086, host: 8086
  # cassandra
  config.vm.network "forwarded_port", guest: 9042, host: 9042
  # rethinkdb
  config.vm.network "forwarded_port", guest: 28015, host: 28015
  config.vm.network "forwarded_port", guest: 8180, host: 8180
  # kong
  config.vm.network "forwarded_port", guest: 8000, host: 8000
  config.vm.network "forwarded_port", guest: 8001, host: 8001

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "site.yml"
    ansible.verbose = "vvvv"
    ansible.install = true
    #ansible.version = "2.0.0.2"
    ansible.inventory_path = "inventory"
  end

end
