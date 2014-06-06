icinga-ansible
==============

Ansible playbooks to exploit ansible's inventory and use it as topology provider for dynamically building icinga's host and service configuration files. Since we have all the available information about what hosts and host groups we have in the datacenter already declared in inventory, it can be used as a discovery point to assign service checks in different kind of hosts or even groups of hosts. 

The necessary configuration files are created remotely on each host and then transfered back to icinga server in a form of individual files. Then a compination process takes place and the individual files are compined in order to produce the final host and service configurations.

Currently there is only support for CentOS 5/6.
