# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"
  config.vm.hostname = "dev.local"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "devbox"
    vb.memory = 1024
  end

  # mysql
  config.vm.network "forwarded_port", guest: 3306, host: 3306
  # postgres
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

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.host_key_checking = false
    ansible.extra_vars = { ansible_ssh_user: "vagrant", testing: true }

    #ansible.tags = [""]
    #ansible.skip_tags = [""]
    #ansible.verbose = "vvvv"
  end

end
