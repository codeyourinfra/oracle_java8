# oracle_java8

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub release](https://img.shields.io/github/release/codeyourinfra/oracle_java8.svg)]() [![Build status](https://travis-ci.org/codeyourinfra/oracle_java8.svg?branch=master)](https://travis-ci.org/codeyourinfra/oracle_java8)

Ansible role to install Oracle Java 8.

## Example Playbook

```yml
---
- hosts: servers
  roles:
    - codeyourinfra.oracle_java8
```

## Build process

The build process is performed in [Travis CI](https://travis-ci.org/codeyourinfra/oracle_java8). During the build, the role is tested by using [Ubuntu Docker images with Python 3](https://hub.docker.com/r/codeyourinfra/python3).

If the build is succeeded, dependent roles may have also its builds triggered, thanks to the [travis-dependent-builds project](https://github.com/stephanmg/travis-dependent-builds). One example is the [Codeyourinfra Jenkins Ansible role](https://galaxy.ansible.com/codeyourinfra/jenkins).

## Author Information

[@gustavomcarmo](https://github.com/gustavomcarmo) is a contributor of [Codeyourinfra](https://github.com/codeyourinfra). Get on board too! :)
