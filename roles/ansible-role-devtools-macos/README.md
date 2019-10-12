Ansible Role Devtools for (MacOS)
=========

A bundle of projects to help developer tools installations.

Requirements
------------

* Homebrew Installation
* Python
* Ansible
* Pip

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew update
brew install python
brew install ansible

# Install pip
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
sudo python get-pip.py
pip install --upgrade pip
pip install regex
```

Role Variables
--------------
```yaml
// Oh My ZSH
zsh_pref:
  home: $HOME/.oh-my-zsh
  theme: awesomepanda
  plugins:
    - git
    - zsh-syntax-highlighting
    - zsh-autosuggestions
```

More details are into [defaults](defaults)

Dependencies
------------

None.

Example Playbook
----------------

```yaml
    - hosts: localhost
      roles:
         - { role: ansible-role-devtools-macos}
```

License
-------

BSD

Author Information
------------------
Sammer Valgas - XGH Expert / Devops Specialist
