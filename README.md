# ansible-rspamd

ansible-rspamd is an Ansible role to install rspamd on a debian based OS.

It performs: 

* installation of rspamd key and repo
* installation of rspamd package(s)

## Install
### Clone
```bash
git clone https://github.com/lgaggini/ansible-rspamd.git
```
## Configuration

The configuration is done by vars listed and explained in [defaults/main.yml](https://github.com/lgaggini/ansible-rspamd/blob/master/defaults/main.yml) file.

## Usage

```
- name: bootstrap an ubuntu cloud image for dovecot
  hosts: imapserver
  vars_files:
    - group_vars/rspamd.yml

  roles:
    - { role: rspamd, tags: ['rspamd'] }
```
