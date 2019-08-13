[![Build Status](https://travis-ci.org/tjtoml/ansible-role-postgresql.svg?branch=master)](https://travis-ci.org/tjtoml/ansible-role-postgresql) [![role](https://img.shields.io/badge/Galaxy-tjtoml.postgresql-5bbdbf.svg)](https://galaxy.ansible.com/tjtoml/postgresql/)

tjtoml.postgresql  
=========

This role installs `postgresql` from the repositories provided by [The PostgreSQL Global Develepment Group](https://www.postgresql.org/)
instead of the the official distribution repositories. That is *all* it does - this role is primarily to ensure that
`postgresql` is installed so that the Ansible `postgres` module can be used.

Requirements
------------

None.

Role Variables
--------------
`postgres_version: 9.4 #default`
`postgres_release: 3 #default`

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: database_servers
      roles:
         - { role: tjtoml.postgresql, postgres_version: 9.4, postgres_release: 3 }

License
-------

BSD

Author Information
------------------

Written by [tjtoml](https://github.com/tjtoml), primarily for use in his own roles.

Contributing
------------
Please submit pull requests! The purpose of this playbook is emphatically not to be a complete implementation of all the
`postgresql` options, but I'm always interested in adding feautures. 
