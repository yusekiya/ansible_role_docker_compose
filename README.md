Ansible Role: docker_compose
=========

Install docker-compose on system with x86_64 or armv7l architecture.
Only raspbian is supported for armv7l.

All the tasks need root privilege.


Requirements
------------

None.

Role Variables
--------------

``` yaml
# Version of docker-compose
# This variable affects install on x86_64 architecture for now
docker_compose_version: 1.9.0
```

Dependencies
------------

None.

Example Playbook
----------------

``` yaml
- hosts: all
  vars_files:
      - vars/main.yml
  roles:
      - {role: docker_compose, become: yes}
```

License
-------

MIT

