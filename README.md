# ansible-local-multi

Just a simpl Ansible setup to do some pacakge and configuration on multiple
workstations, using `localhost` on each rather than specifying inventory etc.

Install requirements:

```sh
ansible-galaxy install -r requirements.yml
```

Run a host-specific playbook:

```sh
ansible-playbook <playbook-name>.yml --ask-become-pass
```

e.g.

```sh
ansible-playbook hyprframe.yml -K
```
