# Ansible Role: hdparm

[![CI](https://github.com/geerlingguy/ansible-role-hdparm/actions/workflows/ci.yml/badge.svg)](https://github.com/geerlingguy/ansible-role-hdparm/actions/workflows/ci.yml)

Installs hdparm on Debian/Ubuntu Linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    hdparm_manage_config: true

Whether this role should manage the hdparm config.

    hdparm_devices: []
      # - dev: /dev/sda
      #   options:
      #     - "spindown_time = 120"

Options to set per device. Only used if `hdparm_manage_config` is `true`.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - geerlingguy.hdparm

## License

MIT / BSD

## Author Information

This role was created in 2016 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).
