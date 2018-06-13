# Cinder Development Environment Setup

This contains an Ansible playbook to quickly set up a Cinder development
environment by installing all system and python packages needed and
cloning all Cinder team repos.

After running this with:

```
sudo ansible-pull -U https://github.com/stmcginnis/cinder-dev-setup
``

you should then be able to successfully run:

```
cd ~/src/openstack/cinder
tox -e all
```

