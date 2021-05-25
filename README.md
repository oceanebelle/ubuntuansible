Ansible learning

Reference: https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html#directory-layout

Examples directory: https://github.com/ansible/ansible-examples

Running the playbook

```bash
# run with prompt for the sudo command
ansible-playbook site -K

# after sudoers don't require password
ansible-playbook site.yml 

# if ui applications are not to be installed
ansible-playbook site.yml --skip-tags=desktop


# creating encrypted files
ansible-vault create foo.yml

# Running ansible script for crc - the pullsecret is encrypted and requires the password
ansible-playbook ubuntucrc.yml --ask-vault-pass

# Running ansible playbook on raspberry pi
ansible-playbook -i inventories/pi/hosts pi.yml

# Running ansible playbook to install minikube (crc alternative) for experimenting with Kubernetes
ansible-playbook ubuntuminikube.yml
```




Items
- [x] Add common apt libraries
- [x] Add java and maven including environment variables
- [x] Add Ubuntu snap packages for most used tools
- [x] Add refresh for snap packages
- [x] Add docker
- [x] Add crc 
- [x] Run ansible playbooks on a remote host (pi)
- [ ] Use inventories directory structure