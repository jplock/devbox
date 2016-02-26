devbox
======
[![Build Status](https://travis-ci.org/jplock/devbox.svg?branch=master)](https://travis-ci.org/jplock/devbox)

Ansible playbook for a development VM running various services. You can exclude any services from being launched by modifying the `Vagrantfile` and skipping certain tags.

### Current Services

* [Cassandra](http://cassandra.apache.org) v3.0.3 (port 9042)
* [Docker](https://www.docker.com) v1.10.2
* [ElasticSearch](https://www.elastic.co) v2.2.x (port 9200)
* [Kafka](http://kafka.apache.org) v0.9.0 (port 9092)
* [Kong](https://getkong.org) v0.6.1 (port 8000)
* [InfluxDB](https://influxdata.com/time-series-platform/influxdb/) v0.10.1 (port 8086)
* [Marathon](https://mesosphere.github.io/marathon/) v0.15.3 (port 8080)
* [Mesos](http://mesos.apache.org) v0.27.1 (port 5050)
* [MongoDB](https://www.mongodb.org) v3.0.9 (port 27017)
* [MySQL](http://dev.mysql.org) v5.5.46 (port 3306)
* [PostgreSQL](http://www.postgresql.org) v9.5.1 (port 5432)
* [RabbitMQ](http://www.rabbitmq.com) v3.6.0 (port 5672)
* [Redis](http://www.redis.io) v3.0.7 (port 6379)
* [RethinkDB](http://rethinkdb.com) v2.2.5 (port 28015)
* [Riak KV](http://basho.com/products/riak-kv/) v2.1.3 (ports 8087 and 8098)
* [Riemann](http://riemann.io) v0.2.10 (port 5555)
* [Zookeeper](http://zookeeper.apache.org) v3.4.8 (port 2181)

### Administration

* [Kong](https://getkong.org/docs/0.6.x/admin-api/) administrative API is at [http://127.0.0.1:8001](http://127.0.0.1:8001)
* [RabbitMQ](http://www.rabbitmq.com/management.html) management console is at [http://127.0.0.1:15672](http://127.0.0.1:15672) (username: guest, password: guest)
* [Riak Control](http://docs.basho.com/riak/latest/ops/advanced/riak-control/) is at [http://127.0.0.1:8098/admin](http://127.0.0.1:8098/admin)
* [InfluxDB](https://docs.influxdata.com/influxdb/v0.9/introduction/overview/) is at [http://127.0.0.1:8083](http://127.0.0.1:8083) (username: root, password: root)
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
