create_user
=========

A brief description of the role goes here.

Requirements
------------

ssh public key for logging into the new account

Role Variables
--------------

    Define the ssh public key
    ~/.ssh/id_rsa.pub

    Define the user you would like to create
    user_name: default

    Define the user state present or absent
    user_state: present

Dependencies
------------

None

Example Playbook
----------------

    ---
    - name: create role
      hosts: all
      become: yes
      tasks:
      - include_role:
        name: create_user
        vars:
          ssh_key: ~/.ssh/id_rsa.pub

License
-------

MIT

Author Information
------------------

kevin@hotmail.com
