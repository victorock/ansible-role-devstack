Role Name
=========

Ansible role to setup devstack

Requirements
------------

N/A

Role Variables
--------------

Directory to install devstack:
```
devstack_dir: "/var/tmp/devstack"
```

Username to create in the machine and run devstack:
```
devstack_user: "stack"
```

Devstack version/branch to clone from repo:
```
devstack_version: "stable/pike"
```

Default devstack password applied to all services:
```
devstack_password: changeme
```

Dependencies
------------

N/A

Example Playbook
----------------

```
- hosts: all
  gather_facts: true

  roles:
    - role: victorock.devstack
      devstack_password: "-_My_Passw0rd_-"

```

License
-------

BSD
MIT

Author Information
------------------

github.com/victorock
