# Ansible Role: Apt

[![Build Status](https://travis-ci.org/cecepm/ansible-role-apt.svg?branch=master)](https://travis-ci.org/cecepm/ansible-role-apt)

Set ubuntu apt repository to nearest/fastest mirror.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    apt_mirror: "http://kambing.ui.ac.id/ubuntu"
    apt_upgrade: false

## Dependencies

None.

## Example Playbook

    - hosts: server
      roles:
      - cecepm.apt

Another example, upgrade all packages after updating sources.list

    - hosts: server
      vars:
        apt_upgrade: true
      roles:
      - cecepm.apt

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Cecep Mahbub](http://ngadimin.org/).
