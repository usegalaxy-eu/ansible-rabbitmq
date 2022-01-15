usegalaxy_eu.rabbitmqserver
=======
Ansible role to deploy and configure a RabbitMQ server on a Centos8 node.
It is possible to create users, administrator or regular one, virtual hosts and bind them together.
Will be exposed the following ports:
* 5671: used by AMQP 0-9-1 and AMQP 1.0 clients with TLS
* 15672: HTTP API clients, management UI and rabbitmqadmin

RabbitMQ runs into a docker container

Requirements
------------
Ansible >= 2.11

Role Variables
--------------
See [defaults/main.yml](defaults/main.yml).

Playbook usage example
-------------
Together with roles:
* [galaxyproject.nginx](https://github.com/galaxyproject/ansible-nginx)
* [usegalaxy_eu.certbot](https://github.com/usegalaxy-eu/ansible-certbot)

this role allows you to create an encrypted RabbitMQ server

See [playbook_example](playbook_example) for details
     
License
-------
GPLv3

Author Information
------------------
[Galaxy Europe](https://galaxyproject.eu)
