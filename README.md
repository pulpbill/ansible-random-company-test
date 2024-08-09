# Local environment:
WSL2 (Ubuntu 20.04)

# First steps
Check ansible's availability:
 ```
 ansible --version
 ```

If not installed, follow the steps depending on your OS release:
https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html#installing-ansible-on-ubuntu

To run this playbook:
```
ansible-playbook -i inventory.ini test-example.yml --ask-become-pass
```

A dry run it's recommended before going straight to the results:
```
ansible-playbook -i inventory.ini test-example.yml --ask-become-pass --check
```