# Ansible for SysAdmin

## Módulo 10

### slides

* 089 - Ansible-doc:

```
ansible-doc -l
ansible-doc awx.awx.user
ansible-doc -l -t shell
ansible-doc -l -t httpapi

```

* 090 - ansible-inventory:

```
ansible-inventory -i hosts --list
ansible-inventory -i hosts --list -y
ansible-inventory -i hosts --host ubuntu
ansible-inventory -i hosts --graph

```

* 091 - ansible-vault:

```
ansible-vault encrypt playbooks/091_passwd.yaml ### password=123
ansible-vault view playbooks/091_passwd.yaml
ansible-vault edit playbooks/091_passwd.yaml

ansible-playbook -u ansible --private-key /etc/ansible/ansible_rsa -i hosts -l redhat -b playbooks/091-vault.yaml --ask-vault-password

```

* 092 - ansible-console:

```
ansible-console -u ansible --private-key /etc/ansible/ansible_rsa -i hosts -b 
```


