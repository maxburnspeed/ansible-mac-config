# ansible-mac-config

Heavily based on Jeff Geerling's Playbook - https://github.com/geerlingguy/mac-dev-playbook

# Installation

Install Apple's command line tools: \
`xcode-select --install to launch the installer`

Install Ansible:

Run the following command to add Python 3 to your $PATH: `export PATH="$HOME/Library/Python/3.9/bin:/opt/homebrew/bin:$PATH"`
Upgrade Pip: sudo pip3 install --upgrade pip
Install Ansible: pip3 install ansible \
Add Ansible PATH `export PATH="$HOME/Library/Python/3.9/bin:$PATH" >> ~/.zshrc` \

Clone or download this repository to your local drive \
In Terminal, navigate to a folder on your local machine that you want to clone the repo into \
`git clone https://github.com/maxburnspeed/ansible-mac-config`

Run ansible-galaxy install -r requirements.yml inside this directory to install required Ansible roles.

Run ansible-playbook main.yml --ask-become-pass inside this directory. Enter your macOS account password when prompted for the 'BECOME' password.

Note: If some Homebrew commands fail, you might need to agree to Xcode's license or fix some other Brew issue. Run brew doctor to see if this is the case.