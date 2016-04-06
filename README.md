# Ansible Role: Install Ruby
[![Build Status](https://travis-ci.org/ferrarimarco/ansible-role-ruby.svg?branch=master)](https://travis-ci.org/ferrarimarco/ansible-role-ruby)

An Ansible role that installs Ruby using ruby-install.

## Using the role
### Installation
```
ansible-galaxy install ferrarimarco.ruby
```

### Variables
```
ruby_version: 2.3.0
```

### Example Playbook
```
  - hosts: all
    roles:
      - ferrarimarco.ruby
```
