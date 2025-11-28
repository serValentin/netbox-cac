# Netbox configuration as code

@netbox-vault.yml
vm_username: <>
vm_password: <>
postgres_user: <>
postgres_password: <>

ansible-playbook -i inventory.ini -e "@.netbox-vault.yml" netbox_installation.yml --ask-vault-pas
ansible-playbook -i inventory.ini -e "@.netbox-vault.yml" netbox_config.yml --ask-vault-pas