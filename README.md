Stouts.ansible
==========

[![Build Status](http://img.shields.io/travis/Stouts/Stouts.ansible.svg?style=flat-square)](https://travis-ci.org/Stouts/Stouts.ansible)
[![Galaxy](http://img.shields.io/badge/galaxy-Stouts.ansible-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/1703)
[![Tag](http://img.shields.io/github/tag/Stouts/Stouts.ansible.svg?style=flat-square)]()

An ansible role which installs and configures the Ansible.

#### Variables

```yaml
ansible_enabled: yes                # The role is enabled

ansible_ppa: ppa:rquillo/ansible    # Launchpad PPA

ansible_hosts: []                   # Setup ansible hosts
                                    # List of strings (will be simple copied to ansible hosts)
                                    # ansible_hosts:
                                    #   - [group_name]
                                    #   - host1 ansible_ssh_host=192.0.0.1
                                    #   - host2 ansible_ssh_host=192.0.0.1

ansible_vars: {}                    # Setup ansible vars (all group)
                                    # ansible_vars:
                                    #   ansible_ssh_user: root
                                    #   environment: production
```


#### Usage

Add `Stouts.ansible` to your roles and set vars in your playbook file.

Example:

```yaml

- hosts: all

  roles:
    - Stouts.ansible
```

#### License

Licensed under the MIT License. See the LICENSE file for details.

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Stouts/Stouts.ansible/issues)!
