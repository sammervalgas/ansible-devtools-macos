Ansible Playbook DevTools (MACOS)
================

 > Note: Playbook was tested with yosemite and mojave macos versions.

Requirements
----------------

* [Homebrew](https://brew.sh/index_pt-br)
* [Ansible >= 2.4](https://www.ansible.com/resources/get-started)
* [Python](https://www.python.org/)

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew update
brew install python
brew install ansible

# Install pip
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
sudo python get-pip.py
pip install --upgrade pip
```

Playbook Tools
----------------
This playbook contains a bunch of tools for developers:

* atom
* docker
* git-config (aliases)
* intellij
* ionic
* iterm2
* java
* nodejs
* oh_my_zsh
* spectacle
* terraform
* virtualbox
* visual-studio-code


Example Runner
-----------------

```bash
git clone https://github.com/sammervalgas/ansible-devtools-macos.git
cd ansible-devtools-macos
ansible-playbook -i inventory/hosts provision.yml -K

# For a specific tool
ansible-playbook -i inventory/hosts provision.yml --tags nodejs -K
ansible-playbook -i inventory/hosts provision.yml --tags terraform -K

# To Run via node
npm run provision
npm run provision -- --tags java
```

Author
----------------
SAMMER VALGAS - DEVOPS SPECIALIST / XGH EXPERT
