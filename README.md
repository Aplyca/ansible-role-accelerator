# Ansible Role: Accelerator

[![Build Status](https://travis-ci.org/Aplyca/ansible-role-accelerator.svg?branch=master)](https://travis-ci.org/Aplyca/ansible-role-accelerator)
[![Circle CI](https://circleci.com/gh/Aplyca/ansible-role-accelerator.svg?style=svg)](https://circleci.com/gh/Aplyca/ansible-role-accelerator)
Ansible Role that installs and configure a web accelerator based on Varnish on Debian/Ubuntu.

## Requirements

Use hash behavior for variables in ansible.cfg
See example: https://github.com/Aplyca/ansible-role-accelerator/blob/master/tests/ansible.cfg
See official docs: http://docs.ansible.com/intro_configuration.html#hash-behaviour

## Installation

Using ansible galaxy:
```bash
ansible-galaxy install aplyca.Accelerator
```
You can add this role as a dependency for other roles, add the role to the meta/main.yml file of your own role:
```yaml
dependencies:
  - { role: mauricios.Varnish }
```

## Role Variables

See default variables: https://github.com/Aplyca/ansible-role-accelerator/blob/master/defaults/main.yml

## Dependencies

None.

## Testing

Use Vagrant to test the role:

```bash
cd tests;
vagrant box add ubuntu/trusty64;
vagrant up;
```
You should see the Varnish cache running on http://localhost:6081

## License

MIT / BSD

## Author Information

Mauricio Sánchez from Aplyca SAS (http://www.aplyca.com)
