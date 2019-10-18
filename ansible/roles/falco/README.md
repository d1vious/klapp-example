[![Build Status - Master](https://travis-ci.org/juju4/ansible-falco.svg?branch=master)](https://travis-ci.org/juju4/ansible-falco)
[![Build Status - Devel](https://travis-ci.org/juju4/ansible-falco.svg?branch=devel)](https://travis-ci.org/juju4/ansible-falco/branches)
# Falco Behavioral activity monitor ansible role

Ansible role to setup Falco
http://www.sysdig.org/falco/
https://github.com/draios/falco

## Requirements & Dependencies

### Ansible
It was tested on the following versions:
 * 2.0
 * 2.5

### Operating systems

Target Debian/Ubuntu and Redhat/Centos.

## Example Playbook

Just include this role in your list.
For example

```
- host: all
  roles:
    - falco
```

## Variables

Nothing specific for now.

## Continuous integration

This role has a travis basic test (for github), more advanced with kitchen and also a Vagrantfile (test/vagrant).

Once you ensured all necessary roles are present, You can test with:
```
$ cd /path/to/roles/juju4.falco
$ kitchen verify
$ kitchen login
```
or
```
$ cd /path/to/roles/juju4.falco/test/vagrant
$ vagrant up
$ vagrant ssh
```

## Troubleshooting & Known issues

* Not possible to run it inside containers
https://github.com/draios/sysdig/issues/152

## License

BSD 2-clause

