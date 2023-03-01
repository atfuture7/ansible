Role Name
=========

Roll to install cpp related tools

Requirements
------------

Please refer to ins-essential/README.md
test playbook located at ins-essential/tests/test.yml
ins-cpp/files contains:



Role Variables
--------------

defaults/main.yml stores variables for all installation files 


Dependencies
------------

Tools used in more than 1 role will move to essential. 
Tools for java only stay here.

Example Playbook
----------------

Please refer to ins-essential/README.md

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

LinkedIn: Jia jia Tang
