# Kubuntu

 1. Mettre à jour et redemarrer le système d'exploitation <br>
    `sudo apt update` <br>
    `sudo apt upgrade`

 3. Faire un `sudo snap refresh`

 4. Installer curl `sudo apt install curl` 

 5. Configurer Git <br>
    `git config --global user.name "John Doe"` <br>
    `git config --global user.email johndoe@example.com`
 
 6. Installer PHP et Composer via la CLI de Laravel <br>
    `/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.4)"`
    Redémarrer le terminal

 7. Installer NodeJS <br>
    `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash` <br>
    Redémarrer le terminal <br>
    `nvm install 22`

 8. Installer MariaDB <br>
    `sudo apt install mariadb-server` <br>
    `sudo mysql_secure_installation` <br>
    `sudo mariadb` <br>
    `GRANT ALL ON *.* TO 'admin'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;` <br>
    `FLUSH PRIVILEGES;` <br>
    `exit`

 9. Installer VSCode
