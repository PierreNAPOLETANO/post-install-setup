# ArchLinux
1. Booter sur une clef d'installation, sélectionner installer (sans speech), attendre d'avoir le prompt : `root@archiso`
2. Activer les locales en FR (pour clavier AZERTY) : `loadkeys fr-latin1`
3. Brancher réseau filaire, passer au point **4** directement.
Si pas de reseau filaire, activer le wi-fi

    a. Lancer l'utilitaire **iwctl** avec la commande `iwctl`, un nouveau prompt apparait  
    b. Lancer `device list` pour avoir la liste des device. On utilisera **wlanO** comme exemple.  
    c. Activer le device avec `device wlan0 set-property Powered on`  
    d. Faire un scan du réseau avec `station wlan0 scan` (la commande ne renvoie rien)  
    e. Lister les réseaux scannés précédemment avec `station wlan0 get-networks`  
    f. Se connecter au réseaux SSID avec `station wlan0 connect SSID`  
    g. Entrer le code wifi (passphrase)  
    h. Quitter l'utilitaire iwct avec `quit`  

4. Tester la connexion internet avec un `ping archlinux.org`
5. Lancer l'installation semi-automatique avec `archinstall`.  
Cette commande va vous aider à créer un fichier de configuration.   
Les locales sont donc à ressaisir pour être intégrées dans le fichier de configuration.  

    - Dans `Profil`, choisir `Desktop` comme profil principal d'installation.  
    Choisir `Xfce-4` et `i3-wm` comme gestionnaire de fenêtre.  
    Sélectionner pilotes `AMD` ou `NVIDIA` suivant votre carte graphique.  
    Si carte NVIDIA trop vieille, ne pas sélectionner driver NVIDIA, laisser driver par defaut du système.  
    - Dans `Audio`, choisir `pipewire`.  
    - Dans `Configurer le réseau`, choisir `NetworkManager`.  
    - Dans `Fuseau horaire`, choisir `Europe/Paris`  
    - Activer la `synchronisation NTP`  

11. Choisir `Installer`.  
La configuration sous format fichier est affichée.  
Sélectionner `Oui` pour continuer.    
12. A la fin de l'installation sélectionner `Non` (ne pas chrooter)
13. Redémarrer le système d'exploitation
14. Installer Git
    ```
    sudo pacman -S git
    git config --global user.name "John Doe"
    git config --global user.email johndoe@example.com
    ```
15. Installer un Navigateur WEB (Chromium)
    `sudo pacman -S chromium`
16. Installer PHP et Composer via la CLI de Laravel
    `/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.4)"`  
Redémarrer le terminal  
17. Installer NodeJS
    `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash`  
Redémarrer le terminal
    `nvm install 22`
18. Installer MariaDB
    ```
    sudo pacman -S mariadb
    sudo mariadb-install-db --user=mysql --basedir=/usr --datadir=/var/lib/mysql
    sudo systemctl start mariadb.service
    sudo mariadb-secure-installation
    sudo mariadb
    GRANT ALL ON *.* TO 'admin'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;
    FLUSH PRIVILEGES;
    exit
    ```
19. Installer Vscode
    `sudo pacman -S code`
