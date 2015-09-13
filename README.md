devbox
======
[![Build Status](https://travis-ci.org/jplock/devbox.svg?branch=master)](https://travis-ci.org/jplock/devbox)

Ansible playbook for a development VM running various services. You can exclude any services from being launched by modifying the `Vagrantfile` and skipping certain tags.

### Current Services

* [Cassandra](http://cassandra.apache.org) v2.2.1 (port 9042)
* [Docker](http://www.docker.com) v1.8.2
* [ElasticSearch](http://www.elasticsearch.org) v1.7.x (port 9200)
* [Kafka](http://kafka.apache.org) v0.8.2.1 (port 9092)
* [InfluxDB](http://influxdb.com) v0.9.3 (port 8086)
* [Marathon](https://mesosphere.github.io/marathon/) v0.10.1 (port 8080)
* [Mesos](http://mesos.apache.org) v0.23.0 (port 5050)
* [MongoDB](http://www.mongodb.org) v3.0.6 (port 27017)
* [MySQL](http://www.mysql.org) v5.5.44 (port 3306)
* [PostgreSQL](http://www.postgresql.org) v9.4.4 (port 5432)
* [RabbitMQ](http://www.rabbitmq.com) v3.5.4 (port 5672)
* [Redis](http://www.redis.io) v3.0.3 (port 6379)
* [RethinkDB](http://rethinkdb.com) v2.1.1 (port 28015)
* [Riak](http://www.basho.com/riak) v2.1.1 (ports 8087 and 8098)
* [Riemann](http://riemann.io) v0.2.9 (port 5555)
* [Zookeeper](http://zookeeper.apache.org) v3.4.6 (port 2181)

### Administration

* [RabbitMQ](http://www.rabbitmq.com/management.html) management console is at [http://127.0.0.1:15672](http://127.0.0.1:15672) (username: guest, password: guest)
* [Riak Control](http://docs.basho.com/riak/latest/ops/advanced/riak-control/) is at [http://127.0.0.1:8098/admin](http://127.0.0.1:8098/admin)
* [InfluxDB](https://influxdb.com/docs/v0.9/introduction/overview.html) is at [http://127.0.0.1:8083](http://127.0.0.1:8083) (username: root, password: root)
* [RethinkDB](http://rethinkdb.com/docs/quickstart/) is at [http://127.0.0.1:8180](http://127.0.0.1:8180)
* [Marathon](https://mesosphere.github.io/marathon/docs/) is at [http://127.0.0.1:8080](http://127.0.0.1:8080)
* Mesos WebUI is at [http://127.0.0.1:5050](http://127.0.0.1:5050)

### Dependencies

* [Vagrant](http://www.vagrantup.com)
* [VirtualBox](https://www.virtualbox.org)

### Getting Started

1. `git clone https://github.com/jplock/devbox.git`
2. `cd devbox`
3. `vagrant up`
