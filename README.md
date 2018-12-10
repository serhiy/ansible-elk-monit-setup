# Ansible utilitity for setting up Monit service on ELK infrastructure

In order to be able to use the utility, you need to have ansible installed on the node which will execute the script, slaves do not require any agent, but must have Python installed.

1. Fill respective configuration into ```variables.yml``` file.
2. Fill the ```hosts``` file (each of the groups can have multiple hosts, but the rule is to have one host per line)
3. Run the following command:
```
ansible-playbook monit-elk-setup.yml -i hosts --extra-vars "@variables.yml"
```
