# Pop!\_OS

1. Désactiver le secure boot du BIOS avant installation.

2. Mettre à jour via `sudo apt update && upgrade` puis redémarrer

3. Installer PHP et Composer via la CLI de Laravel (ou apt) <br>
    `/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.4)"`

4. Installer NodeJS <br>
    `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash` <br>
    Redémarrer le terminal <br>
    `nvm install 22`

5. Installer MariaDB <br>
    `sudo apt install mariadb-server` <br>
    `sudo mysql_secure_installation` <br>
    `sudo mariadb` <br>
    `GRANT ALL ON *.* TO 'admin'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;` <br>
    `FLUSH PRIVILEGES;` <br>
    `exit`

6. Installer VSCode (via flatpack ou apt ou paquet .deb)