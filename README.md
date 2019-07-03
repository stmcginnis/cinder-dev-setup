# Cinder Development Environment Setup

This contains an Ansible playbook to quickly set up a Cinder development
environment by installing all system and python packages needed and
cloning all Cinder team repos.

After running this with:

```
sudo ansible-pull -U https://github.com/stmcginnis/cinder-dev-setup
```

you should then be able to successfully run:

```
cd ~/src/openstack/cinder
tox
```

### Requirements

To use this, you should be able to use a fresh install or cloud image.
You may need to install ansible and git if they did not get installed
by default by running the following on Ubuntu:

```
sudo apt install ansible git
```

Or on Red Hat based systems:

```
sudo dnf install ansible git
```

This was tested on Ubuntu 16.04 and Fedora 28 cloud images. Due to some
locking, you may need to run the command a couple times, but it did
eventually pass successfully.


Ansible versions tested was ansible 2.0 (worked OK) and ansible 2.5
(worked better).
