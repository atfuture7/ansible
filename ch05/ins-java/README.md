Role Name
=========

Roll to install java related tools

Requirements
------------

Please refer to ins-essential/README.md
test playbook located at ins-essential/tests/test.yml
ins-java/files contains:
  eclipse-cpp-2022-12-R-linux-gtk-x86_64.tar.gz (for eclipse c++)
  eclipse.desktop (for eclipse c++)
  ideaIC-2022.3.2.tar.gz (for intelliJ)
  BlueJ-linux-510.deb (for blueJ)

  code_1.75.1-1675893397_amd64.deb (for VC code)



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
