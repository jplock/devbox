devbox
======

Ansible playbook for a development VM running various services. You can exclude any services from being launched by modifying the `Vagrantfile` and skipping certain tags.

### Current Services

* [Riak](http://www.basho.com/riak) v2.0.0
* [MongoDB](http://www.mongodb.org) v2.6.4
* [PostgreSQL](http://www.postgresql.org) v9.3.5
* [MySQL](http://www.mysql.org) v5.5.37
* [Redis](http://www.redis.io) v2.8.17
* [Zookeeper](http://zookeeper.apache.org) v3.4.6
* [ElasticSearch](http://www.elasticsearch.org) v1.3
* [Docker](http://www.docker.com) v1.2.0
* [RabbitMQ](http://www.rabbitmq.com) v3.3.5
* [Kafka](http://kafka.apache.org) v0.8.1.1
* [Mesos](http://mesos.apache.org) v0.20.1
* [Marathon](https://mesosphere.github.io/marathon/) v0.7.0

### Dependencies

* [Vagrant](http://www.vagrantup.com)
* [VirtualBox](https://www.virtualbox.org)

### Getting Started

1. `git clone https://github.com/jplock/devbox.git`
2. `cd devbox`
3. `vagrant up`