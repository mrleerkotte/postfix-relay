Role Name
=========

This role installs postfix and configures it to relay mail to a host.

Requirements
------------

Set the postfix_relay_host variable to point to your smarthost.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

	postfix_relay_host: ""

Specify the host to relay mail on to.

  postfix_relay_tls: false

Specify whether to use SMTP over TLS or not. 

Dependencies
------------

None.

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: mrleerkotte.postfix-relay, postfix_relay_host: "<your smarthost>" }

License
-------

BSD-3

Author Information
------------------

This role was created in 2017 by [Marlon Leerkotte](https://linkedin.com/in/marlonleerkotte).
