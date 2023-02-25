ins-essential
=========

Essential installarion put here. 
main control: ins-essential/test/test-all.yml
role: ins-essential/test/test.yml 

Requirements
------------

put host list (inventory.yml) in ins-essential/defaults/
ansible-playbool -i ins-essential/defaults/ Ansible will include all inventory files. 
expand ansible supported default folders in where inventory files located. 
define host related variables in host_vars/hostname.yml
define group related variables in group_vars/groupname.yml
ref. https://docs.ansible.com/ansible/latest/inventory_guide/intro_inventory.html
ref. https://www.adaltas.com/en/2022/03/15/ansible-variables/


Role Variables
--------------

Role variables are set in default/main.yml , vars/main.yml 
Inventory defalut variable: check previous section: Requirements
if need dynamic include, vars_file: for playbook, module include_vars: for tasks
ref. https://www.toptechskills.com/ansible-tutorials-courses/ansible-include-import-variables-tutorial-examples/


Dependencies
------------

No. This role should be self-content

Example Playbook
----------------

On the uper level of ins-essential, 
command: ansible-playbook ins-essential/tests/test.yml

In test.yml

    - hosts: servers
      roles:
         - ins-essential


useful commands: 
ansible-galaxy init :role:
ansible-playbook playbook.yml -t inventory-fl-fd -K --check -vvv
-K ask for become pass
--check dry run
-vvv debug mode
--syntax-check

License
-------

BSD

Author Information
------------------

LinkedIn: Jia jia Tang