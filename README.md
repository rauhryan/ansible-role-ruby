# Ansible Role: Install Ruby
[![Build Status](https://travis-ci.org/ferrarimarco/ansible-role-ruby.svg?branch=master)](https://travis-ci.org/ferrarimarco/ansible-role-ruby)

An Ansible role that installs Ruby using ruby-install.

Ruby is installed in:
- `/home/{{ user running the playbook }}/.rubies` if [Privilege Escalation](http://docs.ansible.com/ansible/become.html) is not enabled (`become: no`)
- `/opt/rubies` if Privilege Escalation is enabled (`become: yes`)

## Using the role
### Installation
```
ansible-galaxy install ferrarimarco.ruby
```

### Variables
```
ruby_version: 2.3.0
```

### Example Playbooks
#### No privilege escalation
```
  - hosts: all
    roles:
      - ferrarimarco.ruby
```

#### With privilege escalation
```
  - hosts: all
    roles:
      - {role: ferrarimarco.ruby, become: yes}
```
