Ansible role for fips
==================================

Configured FIPS on compatible systems

[![GitHub Actions](https://github.com/mongodb-ansible-roles/ansible-role-fips/workflows/Molecule%20Test/badge.svg)](https://github.com/mongodb-ansible-roles/ansible-role-fips/actions?query=workflow%3A%22Molecule+Test%22)
[![GitHub Actions](https://github.com/mongodb-ansible-roles/ansible-role-fips/workflows/Release/badge.svg)](https://github.com/mongodb-ansible-roles/ansible-role-fips/actions?query=workflow%3A%22Release%22)

Requirements
------------

None

Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-------:|:--------:|
| `fips_in_container` | This task will not work inside of containers | boolean | `false` | `false` |
| `fips_grub_cmdline` | GRUB command line to specify FIPS | string | `GRUB_CMDLINE_LINUX="console=ttyS0,115200n8 console=tty0   net.ifnames=0 rd.blacklist=nouveau crashkernel=auto boot=/dev/xvda2 fips=1  "` | `false` |
| `fips_grub_file` | Default GRUB file | string | `/etc/default/grub` | `false` |

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - role: ansible-role-fips
```

License
-------

[Apache License](LICENSE)
