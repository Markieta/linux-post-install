# fedora-post-install
Post-installation utility to initialize a fresh Fedora installation for my liking.

Install dependencies:

`sudo dnf install ansible libselinux-python python2-dnf`

Download and change into project directory:

`git clone https://github.com/Markieta/fedora-post-install.git && cd fedora-post-install`

Run the Playbook:

`sudo ansible-playbook -i "localhost," -c local workstation.yml`
