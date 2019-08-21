db
=========

Ansible role to install and configure MongoDB for OTUS course homework:
https://github.com/otus-devops-2019-05/alakhno_infra

Requirements
------------

This role requires Ansible 2.4 or higher.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them
are as follows. For all variables, take a look at [defaults/main.yml](defaults/main.yml).

```yaml
# Example values for stage environment
mongo_port: 27017
mongo_bind_ip: 0.0.0.0
env: stage
```

Example Playbook
----------------

```yaml
- name: Install and configure MongoDB
  hosts: db
  become: true
  roles:
    - db
```

License
-------

BSD

Author Information
------------------

Aleksei Lakhno
