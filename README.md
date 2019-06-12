# serverctl is a control suite for daily server management tasks

# Roles

## fastboot
ansible-playbook ./roles/fastboot/create_fastboot.yml -e Server=servername -e RemoteUser=username -i inventory

## pacemaker cluster

ansible-playbook ./pcs.yml -e Server=servername -e RemoteUser=username -e pacemaker=online_yes -i inventory
