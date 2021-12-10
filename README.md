# Ansible Role: Telepresence

[![CI](https://github.com/rholmboe/ansible-role-telepresence/actions/workflows/ci.yml/badge.svg)](https://github.com/rholmboe/ansible-role-telepresence/actions/workflows/ci.yml)
[![Ansible Role](https://img.shields.io/ansible/role/57220?logo=ansible)](https://galaxy.ansible.com/rholmboe/telepresence)
[![Ansible Quality Score](https://img.shields.io/ansible/quality/57220?logo=ansible)](https://galaxy.ansible.com/rholmboe/telepresence)

Installs [Telepresence](https://github.com/telepresenceio/telepresence), a Go-based local development against Kubernetes or OpenShift cluster.

An honest duplication of [ansible-role-packer](https://github.com/geerlingguy/ansible-role-packer/) by [Jeff Geerling](https://www.jeffgeerling.com/)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
    telepresence_version: "2.4.9"
```

The telepresence version to install.

```
    telepresence_arch: "amd64"
```

The system architecture (e.g. `386` or `amd64`) to use.

```
    telepresence_bin_path: /usr/local/bin
```

The location where the telepresence binary will be installed (should be in system `$PATH`).

The user/group which should own binary.

```
    telepresence_user: "root"
    telepresence_group: "root"
```

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - rholmboe.telepresence

## License

MIT / BSD

## Author Information

This role was created in 2021 by [Richard Holmboe](https://about.me/rholmboe)
