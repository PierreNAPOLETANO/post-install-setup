# Ubuntu

 1. Mettre à jour et redemarrer le système d'exploitation

 2. Faire un `sudo snap refresh` et redemarrer

 3. Installer curl et redemarrer

 4. Installer Git <br>
    `sudo apt-get install git`
 
 5. Installer PHP et Composer via la CLI de Laravel <br>
    `/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.4)"`
    Redémarrer le terminal

 6. Installer NodeJS <br>
    `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash` <br>
    Redémarrer le terminal <br>
    `nvm install 22`

 7. Installer MariaDB <br>
    `sudo apt install mariadb-server` <br>
    `sudo mysql_secure_installation` <br>
    `sudo mariadb` <br>
    `GRANT ALL ON *.* TO 'admin'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;` <br>
    `FLUSH PRIVILEGES;` <br>
    `exit`

 8. Installer VSCode

 9. Installer "Extensions" via Snap

 10. Installer DashToPanel via un navigateur
