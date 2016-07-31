git-archlinux
==============

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-git-archlinux.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-git-archlinux)

Install git on Arch Linux.

https://galaxy.ansible.com/suzuki-shunsuke/git-archlinux/

Role Variables
--------------

* git_upgrade: Whether upgrade git if git has already installed. The default value is "no".
* git_nonroot: Whether the remote_user is root or not. This variable is set automatically, and is used to execute tasks with the become option.

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - { role: suzuki-shunsuke.git-archlinux, git_upgrade: no }
```

License
-------

MIT
