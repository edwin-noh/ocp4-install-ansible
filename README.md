# ocp4-install-ansible

OCP installation through ansible

## Ansible components

### Inventory

Basically Ansible inventory describes Ansible mananged nodes(hosts) list. Host can be passed in command line but inventory is the way to manage list of nodes with proper grouping to run commands for multiple nodes.

Define hosts

```
ansible-vault create var.yaml
echo -e '\nxxxxxx' > .vault_pass
echo -e '\n.vault_pass' >> .gitignore
```

Add vault secret in config file

[defaults]
vault_password_file=.vault_pass