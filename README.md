# linux-post-install
Post-installation utility to initialize a fresh Linux installation for my liking.

Install dependencies:

`sudo dnf install ansible libselinux-python python2-dnf`

Download and change into project directory:

`git clone https://github.com/Markieta/linux-post-install.git && cd linux-post-install`

Run the Playbook:

`ansible-playbook -i "localhost," -c local --ask-become-pass workstation.yml`
