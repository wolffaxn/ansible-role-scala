# Ansible Role - Scala

[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub last commit (branch)](https://img.shields.io/github/last-commit/wolffaxn/ansible-role-scala/master.svg)](https://github.com/wolffaxn/ansible-role-scala)

**Table of Contents**

<!-- toc -->

- [About](#about)
- [Requirements](#requirements)
- [Role Variables](#role-variables)
- [Dependencies](#dependencies)
- [Example Playbook](#example-playbook)
- [License](#license)

<!-- tocstop -->

## About 

Installs Scala for RedHat/CentOS linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    scala_version: 2.12.0

    scala_download_dir: /tmp
    scala_download_cleanup: true
    scala_install_dir: /usr/share/scala
    scala_link_default: default
    scala_link_binaries: true

    scala_set_scala_home: true

## Dependencies

None.

## Example Playbook

For RHEL / CentOS

```yaml
---
- hosts: localhost
  become: true
  become_method: sudo
  remote_user: root
  roles:
    - ansible-role-scala
```
## License

This project is licensed under the terms of the [MIT license](LICENSE).
