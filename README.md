# linux-post-install
Post-installation utility to initialize a fresh Linux installation for my liking.

Install dependencies.

Download and change into project directory.

Run the Playbook.

```bash
sudo dnf install -y ansible
git clone https://github.com/Markieta/linux-post-install.git && cd linux-post-install
ansible-playbook -i "localhost," -c local --ask-become-pass workstation.yml
```

## gTile (Interim)

```bash
# Generate config
dconf dump /org/gnome/shell/extensions/gtile/ > files/gtile

# Import config
dconf load /org/gnome/shell/extensions/gtile/ < files/gtile
```

[Source](https://github.com/gTile/gTile/issues/121#issuecomment-657667892)
