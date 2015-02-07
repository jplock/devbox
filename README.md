devbox
======

Ansible playbook for a development VM running various services. You can exclude any services from being launched by modifying the `Vagrantfile` and skipping certain tags.

### Current Services

* [Riak](http://www.basho.com/riak) v2.0.4
* [MongoDB](http://www.mongodb.org) v2.6.7
* [PostgreSQL](http://www.postgresql.org) v9.4.0
* [MySQL](http://www.mysql.org) v5.5.37
* [Redis](http://www.redis.io) v2.8.19
* [Zookeeper](http://zookeeper.apache.org) v3.4.6
* [ElasticSearch](http://www.elasticsearch.org) v1.4.x
* [Docker](http://www.docker.com) v1.4.0
* [RabbitMQ](http://www.rabbitmq.com) v3.4.3
* [Kafka](http://kafka.apache.org) v0.8.2.0
* [Mesos](http://mesos.apache.org) v0.21.1
* [Marathon](https://mesosphere.github.io/marathon/) v0.8.0
* [Riemann](http://riemann.io) v0.2.7

### Dependencies

* [Vagrant](http://www.vagrantup.com)
* [VirtualBox](https://www.virtualbox.org)

### Getting Started

1. `git clone https://github.com/jplock/devbox.git`
2. `cd devbox`
3. `vagrant up`
