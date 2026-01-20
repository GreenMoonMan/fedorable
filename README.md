# fedorable
Fedorable is a set of ansibleplaybooks/roles intended to configure and customize fedora exactly to my liking.
Some playbooks/roles may be generalizable to other setups, but the overall configuration is very personalized

## Roles
### workstation-base
This role defines the basic fedora setup for me.
It performs the following:
- Performs basic system setup
	- enable rpm fusion
	- install non-free codecs, media drivers, etc.
	- configure flathub as the only remote
- Install various applications
	- installs various system tools and other useful applications
	- installs various useful flatpak applications
	- installs docker
	- installs vscodium
- Sets up btrfs snapshots
	- snapshots home directory every hour
	- snapshots root every day

### workstation-personalized
Personalized applications and settings
It performs the following:
- Installs additional packages
	- installs theming
	- installs gnome extensions
	- installs a list of flatpak applications I use
- Customizes gnome
	- Uses dconf to customize the gnome shell user interface
	- Customizes shell extensions

