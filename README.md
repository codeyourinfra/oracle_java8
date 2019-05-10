# oracle_java8

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub release](https://img.shields.io/github/release/codeyourinfra/oracle_java8.svg)](https://github.com/codeyourinfra/oracle_java8/releases/latest) [![Build status](https://travis-ci.org/codeyourinfra/oracle_java8.svg?branch=master)](https://travis-ci.org/codeyourinfra/oracle_java8) [![Ansible Role](https://img.shields.io/ansible/role/29189.svg)](https://galaxy.ansible.com/codeyourinfra/oracle_java8) [![Ansible Role downloads](https://img.shields.io/ansible/role/d/29189.svg)](https://galaxy.ansible.com/codeyourinfra/oracle_java8)

Ansible role to install Oracle Java 8. :warning: This role has been deprecated due to the impossibility of downloading the binaries from Oracle automatically ([see more](https://launchpad.net/~webupd8team/+archive/ubuntu/java)).

## Example Playbook

```yml
---
- hosts: servers
  roles:
    - codeyourinfra.oracle_java8
```

The role requires the *ansible_distribution* variable, obtained through the [gathering facts phase](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html#information-discovered-from-systems-facts). So please don't turn off facts.

## Build process

The build process is performed in [Travis CI](https://travis-ci.org/codeyourinfra/oracle_java8). During the build, the role is tested by using [Molecule](https://molecule.readthedocs.io).

## Test yourself

Inside your [Python virtual environment](https://docs.python.org/3/tutorial/venv.html), run:

`pip install -r requirements.txt`

And then:

`molecule test`

## Author Information

[@gustavomcarmo](https://github.com/gustavomcarmo) is a contributor of [Codeyourinfra](https://github.com/codeyourinfra). Get on board too! :)
