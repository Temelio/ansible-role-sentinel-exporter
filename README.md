# sentinel_exporter

[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://travis-ci.com/Temelio/ansible-role-sentinel-exporter.svg?branch=master)](https://travis-ci.com/Temelio/ansible-role-sentinel-exporter)
[![Updates](https://pyup.io/repos/github/Temelio/ansible-role-sentinel-exporter/shield.svg)](https://pyup.io/repos/github/Temelio/ansible-role-sentinel-exporter/)
[![Python 3](https://pyup.io/repos/github/Temelio/ansible-role-sentinel-exporter/python-3-shield.svg)](https://pyup.io/repos/github/Temelio/ansible-role-sentinel-exporter/)
[![Ansible Role](https://img.shields.io/ansible/role/.svg)](https://galaxy.ansible.com/temelio/sentinel_exporter/)
[![GitHub tag](https://img.shields.io/github/tag/temelio/ansible-role-sentinel-exporter.svg)](https://github.com/Temelio/ansible-role-sentinel-exporter/tags)
[![Build Status](https://travis-ci.org/temelio/ansible-role-sentinel-exporter.svg?branch=master)](https://travis-ci.org/temelio/ansible-role-sentinel-exporter)

Install sentinel_exporter package.

## Requirements

This role requires Ansible 2.6 or higher,
and platform requirements are listed in the metadata file.

## Testing

This role use [Molecule](https://github.com/metacloud/molecule/) to run tests.

Local and Travis tests run tests on Docker by default.
See molecule documentation to use other backend.

Currently, tests are done on:
- Ubuntu Xenial
- Ubuntu Bionic
- Ubuntu Eoan

and use:
- Ansible 2.4.x
- Ansible 2.5.x
- Ansible 2.6.x
- Ansible 2.7.x
- Ansible 2.8.x

### Running tests

#### Using Docker driver

```
$ tox
```

You can also configure molecule options and molecule command using environment variables:
* `MOLECULE_OPTIONS` Default: "--debug"
* `MOLECULE_COMMAND` Default: "test"

```
$ MOLECULE_OPTIONS='' MOLECULE_COMMAND=converge tox
```

## Role Variables

### Default role variables

``` yaml
```

## Dependencies

None

## Example Playbook

``` yaml
- hosts: servers
  roles:
    - { role: temelio.sentinel_exporter }
```

## License

MIT

## Author Information

Lise Machetel (for Temelio company)
- https://temelio.com
- lise.machetel [at] temelio.com
