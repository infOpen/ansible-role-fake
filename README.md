# fake

[![CI](https://github.com/infOpen/ansible-role-fake/workflows/CI/badge.svg)](https://github.com/infOpen/ansible-role-fake/actions)
[![Mergify Status][mergify-status]][mergify]
[![Updates](https://pyup.io/repos/github/infOpen/ansible-role-fake/shield.svg)](https://pyup.io/repos/github/infOpen/ansible-role-fake/)
[![Python 3](https://pyup.io/repos/github/infOpen/ansible-role-fake/python-3-shield.svg)](https://pyup.io/repos/github/infOpen/ansible-role-fake/)

Install fake package.

## Requirements

This role requires Ansible 2.8 or higher,
and platform requirements are listed in the metadata file.

## Testing

This role use [Molecule](https://github.com/ansible-community/molecule) to run tests.

Local and Github Actions tests run tests on Docker by default.
See molecule documentation to use other backend.

Currently, tests are done on:
- CentOS 7
- CentOS 8
- Debian Buster
- Debian Stretch
- Ubuntu Bionic
- Ubuntu Focal

and use:
- Ansible 2.8.x
- Ansible 2.9.x

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
    - { role: foobar.fake }
```

## License

MIT

## Author Information

Foo Bar (for Foobar Inc. company)
- http://foo.bar
- foo [at] bar

[mergify]: https://mergify.io
[mergify-status]: https://img.shields.io/endpoint.svg?url=https://gh.mergify.io/badges/infOpen/ansible-role-fake&style=flat
