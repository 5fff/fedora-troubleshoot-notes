### Install KDE:
sudo dnf groupinstall "KDE Plasma Workspaces"
### Install Fcitx5 

Refer to: https://wiki.archlinux.org/title/Fcitx5
Use im-chooser to chose Fcitx5 as defaut IME
Install fcitx5-rime

Set the following environment variables in `~/.config/environment.d/im.conf`, this is for fixing IME not working in apps such as Firefox
```
GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx
```
