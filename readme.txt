motd-role.yml - Ansible playbook that invokes the motd role
roles/stats/templates/motd.j2 - Ansible template that renders the role variable system email and other variables(CPU, Memory Usage, Kernel)
roles/stats/defaults/main.yml - Default value of role variable
roles/stats/tasks/main.yml - Contains the tasks for rendering the template

How to trigger the playbook:
vagrant@vagrant:~/solution$ ansible-playbook motd-role.yml

*************
Output:
*************
 [WARNING]: provided hosts list is empty, only localhost is available. Note that the implicit localhost does not match 'all'


PLAY [use motd role playbook] *************************************************************************************************************************************************************************************

TASK [Gathering Facts] ********************************************************************************************************************************************************************************************
ok: [localhost]

TASK [stats : copy motd file] *************************************************************************************************************************************************************************************
changed: [localhost]

PLAY RECAP ********************************************************************************************************************************************************************************************************
localhost                  : ok=2    changed=1    unreachable=0    failed=0
