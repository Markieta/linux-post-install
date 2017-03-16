# linux-post-install
Post-installation utility to initialize a fresh Linux installation for my liking.

Install dependencies.

Download and change into project directory.

Run the Playbook.

```
sudo dnf install ansible libselinux-python python2-dnf
git clone https://github.com/Markieta/linux-post-install.git && cd linux-post-install
ansible-playbook -i "localhost," -c local --ask-become-pass workstation.yml
```
