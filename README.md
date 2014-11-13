# Ansible Role: Apt

[![Build Status](https://travis-ci.org/cecepm/ansible-role-apt.svg?branch=master)](https://travis-ci.org/cecepm/ansible-role-apt)

Set ubuntu apt repository to nearest/fastest mirror.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    apt_mirror: "http://kambing.ui.ac.id/ubuntu"

## Dependencies

None.

## Install (using git clone)

Clone this role to your ansible roles directory, ie:

    cd my-ansible-project/roles
    git clone https://github.com/cecepm/ansible-role-apt.git apt

### Example playbook

    - hosts: servers
      roles:
         - { role: apt }

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Cecep Mahbub](http://ngadimin.org/).
