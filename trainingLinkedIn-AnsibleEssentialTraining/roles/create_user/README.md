create_user
=========

Create a user.

Requirements
------------

No specific.

Role Variables
--------------

# Define the name of the user you want to create
user_name = default

# Define the state of the user present or absent 
user_state = present

Dependencies
------------

None.

Example Playbook
----------------

---
- name: CREATE A REMOTE USER
  hosts: all
  become: yes
  tasks:
    - include_role:
        name: create_user
      vars:
          user_name: oliver
          ssh_key: ~/.ssh/id_rsa.pub


License
-------

GPL

Author Information
------------------

None.github@oepaud.com
