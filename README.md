motd
====

Generate MOTD file.

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

    motd_ascii_logo:
    motd_message:

Dependencies
------------

Example Playbook
----------------

1) Generate MOTD file using default ASCII logo and message.

    - hosts: all
      roles:
         - { role: motd }

2) Generate MOTD file using default ASCII logo and custom message.

    - hosts: all
      roles:
         - { role: motd, motd_message: This is the new message }

License
-------

BSD

Author Information
------------------

Kevin Brebanov
