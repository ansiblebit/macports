macports
========

An [Ansible](http://www.ansible.com) role for [macports](http://www.macports.org).

[![License](http://img.shields.io/badge/license-New%20BSD-blue.svg?style=flat)](https://raw.githubusercontent.com/ansiblebit/macports/master/LICENSE)
[![Platforms](http://img.shields.io/badge/platforms-macosx-lightgrey.svg?style=flat)](#)

[![Project Stats](https://www.openhub.net/p/ansiblebit-macports/widgets/project_thin_badge.gif)](https://www.openhub.net/p/ansiblebit-macports/)

Requirements
------------

- ansible >= 1.7.2

Role Variables
--------------

User defined variables:

| variable | default value | description |
|:--------:|:-------------:|:------------|
| macports_version | 2.3.3 | the macports version to be installed. |
| macports_upgrade_outdated | yes | flag to determine if outdated ports should be upgraded after the installation process. |


Default variables:

| variable | description |
|:--------:|:------------|
| macports_tarball | the file name of the macports tarball. |
| macports_tarball_url | the prefix for the URL from which the macports tarball will be downloaded. |
| macports_build_from_source | flag to determine if macports is to be installed from source (not supported yet). |
| macports_installer | hash that contains the filename and SHA256 checksum of the macports files for each supported OS family and distribution. |

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansiblebit.macports, macports_version: 2.3.3, macports_upgrade_outdated: yes }

License
-------

BSD

Author Information
------------------

- [steenzout](http://github.com/steenzout)
