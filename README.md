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
| name | desc | type | default | required |

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
