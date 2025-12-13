# Fedora

## Pas besoin d'installer:
- cURL
- Git

## A installer
1. Mise à jour de l'OS et redemarrer
   
2. Suivre les instructions de cette vidéo <br>
https://www.youtube.com/watch?v=Sn-32PM8Vlo

commandes à executer:
- `sudo dnf install -y --nogpgcheck https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm && sudo dnf install -y rpmfusion-free-appstream-data rpmfusion-nonfree-appstream-data && sudo dnf install -y rpmfusion-free-release-tainted rpmfusion-nonfree-release-tainted`
- `sudo dnf install gstreamer1-plugins-{base,good,bad-free,good-extras,bad-free-extras,ugly-free} gstreamer1-libav`
- `sudo dnf install gstreamer1-plugins-{bad-freeworld,ugly}`
- `sudo dnf install gnome-tweaks`
- `sudo dnf install gnome-extensions-app`

sources
- https://www.youtube.com/watch?v=Sn-32PM8Vlo
- https://www.linuxtricks.fr/wiki/fedora-ajouter-le-depot-rpm-fusion
- https://www.linuxtricks.fr/wiki/fedora-installation-de-codecs
- http://web.archive.org/web/20240329210047/https://docs.fedoraproject.org/en-US/quick-docs/installing-plugins-for-playing-movies-and-music

3. Installer MariaDB (https://www.digitalocean.com/community/tutorials/how-to-install-mariadb-on-debian-11) <br>
`sudo dnf install mariadb-server` <br>
`sudo systemctl start mariadb` <br>
`sudo mysql_secure_installation` <br>
`sudo mariadb`

4. Installer Node JS (https://nodejs.org/fr/download)

5. Installer PHP (https://laravel.com/docs/12.x)

6. Installer Visual Studio Code (https://code.visualstudio.com/docs/setup/linux#_rhel-fedora-and-centos-based-distributions)
