# Ansible Role - Scala

Installs Scala for RedHat/CentOS linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    scala_version: 2.11.8

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

Licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Author Information

This role was created by Alexander Wolff.
