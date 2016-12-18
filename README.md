# WHOOP dev machine setup #

*Work in progress*

Ansible scripts to provision a developer machine.

There's a chicken-and-egg problem with running Ansible on yourself, so to bootstrap:

1. Install [Homebrew](http://brew.sh):
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

2. Install [Ansible](http://docs.ansible.com/ansible/index.html)
```
brew install ansible
```

3. Put some secrets into your environment (the scripts will make them permanent)
```
export AWS_ACCESS_KEY_ID=foo
export AWS_SECRET_ACCESS_KEY=bar
```

4. Overwrite all your settings with mine!
```
ansible-playbook osx.yml
```
