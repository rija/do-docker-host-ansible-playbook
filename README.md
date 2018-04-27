Ansible playbook for creating a fully setup docker host droplet on Digital Ocean (Work in progress)

### Requirements:

It assumes you have both python2 and python3, and ansible is installed in a python2.x virtualenv.

Make sure you have dopy installed as well.

The official version of dopy breaks with the "basestring" error. You can obtain a patched version here:
https://github.com/rija/dopy/


### Usage: 

create a ``hosts`` file from the ``hosts-sample``  example, modify it to suit your particular need.


```bash
$ cd do-docker-host-ansible-playbook
$ cp hosts-sample hosts
$ ansible-playbook -vvv -i hosts create-docker-host.yml
```
