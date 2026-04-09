Upadte APT Packages

    sudo apt update

Install Apache Server

    sudo apt install apache2

To check if Apache is running

    sudo systemctl status apache2

Install Mysql Server

    sudo apt install mysql-server

To check if MySQL is running

    sudo systemctl status mysql

Check which PHP versions are available (install the latest)

    apt list php*

Install PHP

    sudo apt install php8.4

Check PHP Version

    php -v

Install PHP Mysqli And Some Necessary Extension For PhpMyAdmin

    sudo apt install php8.3-sqlite3 php8.3-cli php8.3-common php8.3-mbstring php8.3-xml php8.3-curl php8.3-mysql php8.3-zip php8.3-gd php8.3-bcmath php8.3-soap php8.3-intl php8.3-readline -y

Enable PHP Mysqli

    sudo phpenmod mysqli

Setup Composer

    # Update your package list
    sudo apt update
    
    # Install dependencies and Composer
    sudo apt install curl php-cli php-mbstring git unzip -y
    
    # Download and install Composer globally
    curl -sS https://getcomposer.org/installer | php
    sudo mv composer.phar /usr/local/bin/composer

Add Authentication To The PhpMyAdmin Config (config.inc.php) File For Enableing Auto Login

    /* Authentication type */
    $cfg['Servers'][$i]['auth_type'] = 'config';
    $cfg['Servers'][$i]['user'] = 'username';
    $cfg['Servers'][$i]['password'] = 'password';
