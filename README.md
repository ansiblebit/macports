# ansiblebit.macports

[![License](http://img.shields.io/badge/license-New%20BSD-blue.svg?style=flat)](https://raw.githubusercontent.com/ansiblebit/macports/master/LICENSE)
[![Platforms](http://img.shields.io/badge/platforms-macosx-lightgrey.svg?style=flat)](#)

[![Project Stats](https://www.openhub.net/p/ansiblebit-macports/widgets/project_thin_badge.gif)](https://www.openhub.net/p/ansiblebit-macports/)

An [Ansible](http://www.ansible.com) role for [macports](http://www.macports.org).


## Tests

| Family | Distribution | Version | Test Status |
|:-:|:-:|:-:|:-:|
| Darwin | MacOSX  | 10.13  | [![x86_64](http://img.shields.io/badge/x86_64-passed-006400.svg?style=flat)](#) |


## Requirements

- ansible >= 2.4


## Role Variables

- **macports_version**: the macports version to be installed (default: `2.5.2`).
- **macports_upgrade_outdated**: flag to determine if outdated ports should be upgraded after the installation process (default: `yes`).
- **macports_selfupdate**: flag to determine if the latest port revisions should be downloaded (default: `yes`).

- **macports_build_from_source**: flag to determine if macports is to be installed from source (not supported yet).
- **macports_force_install**: flag to indicate if a new install is to be performed even if macports is already present in the server.
- **macports_installer**: hash that contains the filename and SHA256 checksum of the macports files for each supported OS family and distribution.
- **macports_tarball**: the file name of the macports tarball.
- **macports_tarball_url**: the prefix for the URL from which the macports tarball will be downloaded.


## Dependencies

None.

## Playbooks

    - hosts: servers
      roles:
         - role: ansiblebit.macports
