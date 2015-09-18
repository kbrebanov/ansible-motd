motd
====

[![Ansible Role](https://img.shields.io/ansible/role/3305.svg)](https://galaxy.ansible.com/list#/roles/3305)

Generate MOTD file.

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name            | Default                           | Description                               |
|-----------------|-----------------------------------|-------------------------------------------|
| motd_ascii_logo | ""                                | ASCII logo to be displayed before message |
| motd_message    | Welcome to {{ ansible_hostname }} | MOTD message                              |

Dependencies
------------

CentOS:
  - kbrebanov.selinux

Example Playbook
----------------

Generate MOTD file using default ASCII logo and message.
```
- hosts: all
  roles:
    - { role: kbrebanov.motd }
```

Generate MOTD file using default ASCII logo and custom message.
```
- hosts: all
  roles:
    - { role: kbrebanov.motd, motd_message: This is the new message }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
