[![Build Status](https://travis-ci.org/mongrelion/ansible-role-telegraf.svg?branch=master)](https://travis-ci.org/mongrelion/ansible-role-telegraf)

Telegraf
=========

Installs Telegraf

Requirements
------------

None

Role Variables
--------------

  - `db_url`: the URL where the InfluxDB instance is listening on, including port (e.g. http://localhost:8086)  
    Default: _http://127.0.0.1:8086_

  - `db_name`: the target database for metrics.  
    Default: _telegraf_

Dependencies
------------

None

Example Playbook
----------------

Install Telegraf pointing to an InfluxDB instance listening on *1.2.3.4:8086* and using *metrics* as the database:

    - hosts: servers
      roles:
         - { role: mongrelion.telegraf, db_url: "http://1.2.3.4:8086", db_name: "metrics" }

License
-------

MIT

Author Information
------------------

You can find me on Twitter: [@mongrelion](https://twitter.com/mongrelion)
