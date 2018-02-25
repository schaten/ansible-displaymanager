# ansible-displaymanager
This role (in theory) allows to switch between different display managers easily.
At the moment, only kdm and lightdm (gtk-greeter) are supported.

## Example-Playbook:
- name: graphical target + display-manager
  hosts: clients
  tags: graphics
  vars:
    mydm: 'kdm'
  roles: [{ role: 'ansible-displaymanager'}]
