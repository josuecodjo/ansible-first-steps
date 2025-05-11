# Ansible first Steps

## On the controller node

- `ssh-keyben -t rsa -b 4096`
- Copy the public key and paste it to authorized_keys on web01 and web02

- `ansible all -i inventory/hosts -m ping`
- `ansible-playbook -i inventory/hosts playbooks/os-update.yml`
- `ansible-playbook -i inventory/hosts playbooks/ufw.yml`