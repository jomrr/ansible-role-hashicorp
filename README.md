# Ansible role hashicorp

![GitHub](https://img.shields.io/github/license/jomrr/ansible-role-hashicorp) ![GitHub last commit](https://img.shields.io/github/last-commit/jomrr/ansible-role-hashicorp) ![GitHub issues](https://img.shields.io/github/issues-raw/jomrr/ansible-role-hashicorp)

**Ansible role to add the hashicorp repository for supported distributions.**

## Description

Add the hashicorp linux repository for supported distributions.

## Prerequisites

This role has no special prerequisites.

### System packages (Fedora)

- `python3` (>= 3.9)

### Python (requirements.txt)

- ansible >= 2.15

## Dependencies (requirements.yml)

```yaml
collections:
  - community.general

roles: []
```

## Supported Platforms

| OS Family | Distribution | Version | Container Image |
|-----------|--------------|---------|-----------------|
| RedHat | AlmaLinux | latest | [jomrr/molecule-almalinux:latest]( https://hub.docker.com/r/jomrr/molecule-almalinux ) |
| Debian | Debian | latest | [jomrr/molecule-debian:latest]( https://hub.docker.com/r/jomrr/molecule-debian ) |
| RedHat | Fedora | latest | [jomrr/molecule-fedora:latest]( https://hub.docker.com/r/jomrr/molecule-fedora ) |
| Debian | Ubuntu | latest | [jomrr/molecule-ubuntu:latest]( https://hub.docker.com/r/jomrr/molecule-ubuntu ) |

## Role Variables

No role default variables specified, see [defaults/main.yml](defaults/main.yml).

## Example Playbook

Example playbooks(s) that show how to use this role.

## Simple example playbook

A simple default example playbook for using jomrr.hashicorp.
```yaml
---
# name: "jomrr.hashicorp"
# file: "playbook_hashicorp.yml"

- name: "PLAYBOOK | hashicorp"
  hosts: "hashicorp_hosts"
  gather_facts: true
  roles:
    - role: "jomrr.hashicorp"
```

## Author(s) and License

- :octocat:                 Author::    [jomrr](https://github.com/jomrr)
- :triangular_flag_on_post: Copyright:: 2024, Jonas Mauer
- :page_with_curl:          License::   [MIT](LICENSE)

## References

- [Official Packaging Guide](https://www.hashicorp.com/official-packaging-guide)

---
