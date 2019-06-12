# serverctl is a control suite for daily server management tasks

# Roles

## fastboot
ansible-playbook ./roles/fastboot/create_fastboot.yml -e Server=servername -e RemoteUser=username -i inventory

## pacemaker cluster

pacemaker status = online/offline

pacemaker enabled = yes/no

ansible-playbook ./pcs.yml -e RemoteUser=username -e pacemaker=online_yes -i inventory
