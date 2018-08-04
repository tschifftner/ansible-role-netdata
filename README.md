# Ansible Role: netdata

[![Build Status](https://travis-ci.org/tschifftner/ansible-role-netdata.svg?branch=master)](https://travis-ci.org/tschifftner/ansible-role-netdata)

Installs netdata on Debian/Ubuntu linux servers.

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
netdata_version: v1.10.0
netdata_repo_url: https://github.com/firehol/netdata.git
netdata_deps:
  - zlib1g-dev
  - uuid-dev
  - libmnl-dev
  - gcc
  - make
  - git
  - autoconf
  - autoconf-archive
  - autogen
  - automake
  - pkg-config
```

## Dependencies

None.

## Example Playbook

```
- hosts: server
  roles:
    - { role: tschifftner.netdata }
```

## Supported OS

 - Debian 9 (Stretch)
 - Debian 8 (Jessie)
 - Ubuntu 18.04 (Bionic Beaver)
 - Ubuntu 16.04 (Xenial Xerus)
 
## Required ansible version

Ansible 2.5+

## License

[MIT License](http://choosealicense.com/licenses/mit/)

## Author Information

 - [Tobias Schifftner](https://twitter.com/tschifftner), [ambimax® GmbH](https://www.ambimax.de)