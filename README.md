# SchnuppertagPcSettings

## edit sources list
```
sudo nano /etc/apt/sources.list
```
```
deb [trusted=yes] cdrom:[Official Debian GNU/Linux Live 12.5.0 gnome 2024-02-10T11:07:25Z]/ bookworm main non-free-firmware
deb http://deb.debian.org/debian-security/ bookworm-security main
deb-src http://ftp.us.debian.org/debian/ bookworm main contrib non-free
deb http://deb.debian.org/debian bookworm main 
deb-src http://deb.debian.org/debian bookworm main
```
speichern
```
sudo apt update
```
## snapd
```
sudo apt install snapd

sudo systemctl enable --now snapd.socket
```
## add nameservers
```
sudo nano /etc/resolv.conf
```
```
nameserver 8.8.8.8
nameserver 8.8.4.4
```
test :
```
 ping -c 4 deb.debian.org
```
```
sudo systemctl restart networking.service
```
## codium
```
sudo snap install codium --classic
```

## nodejs
```
sudo apt install nodejs
```
## npm
```
sudo apt install npm
```
## gnome extensions
```
sudo apt install gnome-shell-extension-dashtodock
```
Extensions -> Dash to Dock
Settings -> Intelligent autohide off
## gnome tweaks
```
sudo apt install gnome-tweaks
```
Tweaks -> Window Titlebars -> Maximize/Minimize
