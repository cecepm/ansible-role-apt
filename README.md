# Ansible Role: Apt

Set ubuntu apt repository to nearest/fastest mirror.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    apt_mirror: "http://kambing.ui.ac.id/ubuntu"

Dependencies
------------

None.

## Example Playbook

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Cecep Mahbub](http://ngadimin.org/).
