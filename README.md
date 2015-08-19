Ansible Loggly Role
===========================

Installs syslog-ng and configures syslog-ng to send syslog to Loggly, securely

Install role:
```bash
sudo ansible-galaxy install kristjanpkristjansson.ansible-loggly
```

Update role, or force install:
```bash
sudo ansible-galaxy install kristjanpkristjansson.ansible-loggly --force
```

Use role in playbook:
```
- name: Add logging to Loggly
  hosts: LogMe
  sudo: true
  roles:
    - kristjanpkristjansson.ansible-loggly
```

Role Variables
--------------

```
loggly:
  tags: ''
  token:
    - ansible
    - syslog-ng
```

Loggly tags is list of multiple tags.
Loggly token variable is your Loggly account token.

Dependencies
------------

None.

License
-------

Licensed under the MIT License. See the LICENSE file for details.

Maintainers
-------

[Kristján Páll Kristjánsson](https://github.com/kristjanpkristjansson)
