macports
========

An [Ansible](http://www.ansible.com) role for [macports](http://www.macports.org).

[![Build Status](https://travis-ci.org/ansiblebit/macports.svg?branch=master)](https://travis-ci.org/ansiblebit/macports)
[![License](https://img.shields.io/badge/license-New%20BSD-blue.svg?style=flat)](https://raw.githubusercontent.com/ansiblebit/macports/master/LICENSE)

[![Project Stats](https://www.openhub.net/p/ansiblebit-macports/widgets/project_thin_badge.gif)](https://www.openhub.net/p/ansiblebit-macports/)

Requirements
------------

- ansible >= 1.7.2

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

- macports_version (default=2.3.3)

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
