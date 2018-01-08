# Install Favorite Apps
```bash
# update mirrors
sudo pacman-mirrors -g
# synchonize repositories and update installed packages
sudo pacman -Syyu
# only for slow HDs -- not recommended for SSDs!
if [[ $@ == "--optimize" ]]; then
	sudo pacman-optimize && sync
fi
# apps from standard repositories
sudo pacman -S git tk bash-completion nodejs python-pip postgresql dbeaver asciiquarium sl 
# apps from AUR
yaourt -Syua
yaourt -S --noconfirm tilix-bin webstorm pycharm-professional datagrip sublime-text-dev visual-studio-code atom-editor-bin google-chrome vivaldi spotify franz-bin
```

# Clock format
`<b>%R</b>%n%d/%m/%Y`
