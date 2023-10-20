Ansible Role: AD Random Content.
=========

An Ansible role to create a bunch of random content in the domain. This role is basically a wrapper for [BadBlood by @davidprowe and secframe.com](https://github.com/davidprowe/BadBlood). I simply imported the scripts into Ansible and removed the attack vectors.

Requirements
------------

DA credentials. Needs to be run on the DC.

Role Variables
--------------

```yml
user_count: 500
group_count: 100
computer_count: 100
```

Dependencies
------------

None.

Example Playbook
----------------

```yml
- hosts: pdc01
  roles:
    - role: xbufu.ad_random_content
      vars:
        user_count: 500
        group_count: 100
        computer_count: 100
```

License
-------

MIT / BSD

Author Information
------------------

Created by xbufu.
