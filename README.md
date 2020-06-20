Ansible learning

Reference: https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html#directory-layout

Examples directory: https://github.com/ansible/ansible-examples

Running the playbook

```bash
# run with prompt for the sudo command
ansible-playbook site -K

# after sudoers don't require password
ansible-playbook site.yml 
```