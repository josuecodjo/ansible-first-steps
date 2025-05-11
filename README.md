# Ansible first Steps

- `ansible all -i inventory/hosts -m ping`
- `ansible-playbook -i inventory/hosts playbooks/os-update.yml`
- `ansible-playbook -i inventory/hosts playbooks/ufw.yml`