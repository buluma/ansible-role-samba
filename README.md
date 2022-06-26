# [samba](#samba)

Samba for RHEL/CentOS.

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-samba/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-samba/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-samba/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-samba)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/samba)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/samba)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-samba.svg)](https://github.com/buluma/ansible-role-samba/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-samba.svg)](https://github.com/buluma/ansible-role-samba/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-samba.svg)](https://github.com/buluma/ansible-role-samba/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: Converge
  hosts: all
  become: true

  pre_tasks:
    - name: Update apt cache.
      apt: update_cache=true cache_valid_time=600
      when: ansible_os_family == 'Debian'

  roles:
    - role: buluma.samba
```



## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-samba/blob/main/requirements.txt).


## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-samba/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|el|7, 8|
|fedora|all|
|ubuntu|all|
|debian|all|

The minimum version of Ansible required is 2.0, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-samba/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-samba/blob/master/CHANGELOG.md)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
