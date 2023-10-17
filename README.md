# Ansible for SysAdmin

##

### slides


* 075 - roles c/ files:

```
ansible-playbook -u ansible --private-key /etc/ansible/ansible_rsa -i hosts -b -l ubuntu playbooks/075-roles_files.yaml
```

* 076 - roles c/ templates:

```
ansible-playbook -u ansible --private-key /etc/ansible/ansible_rsa -i hosts -b -l ubuntu playbooks/076-roles_templates.yaml
```

* 084 - ansible-galaxy:

```
ansible-galaxy collection list
ansible-galaxy collection install community.aws

```

* 085 - Criando uma collection:

```
ansible-galaxy collection init --init-path /ansible/collections tadim.nginx
```

* 086 - Gerenciando roles:

```
ansible-galaxy role list --roles-path /ansible/playbooks/roles/
ansible-galaxy role init r086-novarole --init-path /ansible/playbooks/roles

ansible-galaxy role search nginx
ansible-galaxy role search nginx --galaxy-tags rocky

ansible-galaxy role info aadl.docker-nginx-alpine

```

* 088 - Importando Collection:

```
cd //ansible/collections/rogeriotadimtadim/collection001
ansible-galaxy collection build

ansible-galaxy collection publish --token <token> ./rogeriotadim-collection001-1.0.0.tar.gz

```

