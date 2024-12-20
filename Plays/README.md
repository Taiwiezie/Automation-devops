# ANSIBLE Deploy
The Ansible deployment configuration can be found in this location

## Start the services up
ansible-playbook -i ../inventory deploy_docmost.yml -l controller --tags=start_service --ask-vault-password
Supply the password for the service start.

## Stop the services
ansible-playbook -i ../inventory deploy_docmost.yml -l controller --tags=stop_service