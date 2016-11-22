# fuel_inventory
Ansible inventory file to utilise Fuel DB

Provides JSON inventory for Ansible:
- groups are created around environment ID and role
- basic hostvars are provided
- labels are transfered to hostvar for host

Example:
Simple command run on all compute nodes in Fuel environment 9
> ansible -i fuel_inventory -m command -a 'ls' 'cluster_9:&compute'


