# DOCUMENTATION

## Step 1: APACHE INSTALLATION

#### Command: sudo apt update (Packages update in Package Manager)
#### Output:

![packages Updated](./image/packagesUpdateOutput.png "packages update process")

#### Command: sudo apt install apache2 (Apache 2 Installation)
#### Output:

![apache2 Installation](./image/apache2Installation.png "apache2 installation process")

#### Command: sudo systemctl status apache2 (Apache Status Confirmation)
#### Output:

![apache2 Installation](./image/apacheStatus.png "apache in running state")

#### Command:  curl http://127.0.0.1:80 (Using curl to access server via IP address)
#### Output:

![Accessingg Server](./image/curlAccessServerViaIP.png "accessing server via IP address")

#### Command:  http://100.26.144.182/ (Accessing IP address via browser)
#### Output:

![Accessingg Server](./image/apacheServer.png "accessing apache server")

## PROJECT-1 GIT INITIALIZATION AND FIRST COMMIT i.e running git commit for Step 1.

#### Command:  git init & git status (Project-1 git initialization and check status to see changes)
#### Output:

![Git initialization](./image/project1GitInitialization.PNG "git initialization")

#### Commands:  git add . | git status | git commit (Staging and commiting files)
#### Outputs:

![Staging](./image/gitAdd.PNG "Staging all files to commit")

![Commiting all files](./image/step1Done.PNG "Files Commited")

## Step 2: MYSQL INSTALLATION

#### Command: sudo apt install mysql-server (Mysql Installation)
#### Output:

![MYSQL](./image/MySQL.PNG "MYSQL Installation")

#### Command: $ sudo mysql (Mysql Installation)
#### Output:

![MYSQL](./image/MySQL2.PNG "MYSQL Installation")

#### Command: $ sudo mysql_secure_installation (Mysql Installation)
#### Output:

![MYSQL](./image/MySQL3.PNG "MYSQL Installation")


## Step 2: MYSQL INSTALLATION

![MYSQL](./image/MySQL4.PNG "MYSQL Console login")

## PROJECT-1 git commit for Step 2.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step2](./image/gitCommit2.PNG "step 2 commit")

## Step 3: PHP INSTALLATION

#### Command: $ sudo apt install php libapache2-mod-php php-mysql (Php and other packages Installation)
#### Output:

![PHP](./image/php.PNG "PHP Installation")

#### Command: $ php -V (Php  Installation Confirmation)
#### Output:

![PHP](./image/php2.PNG "PHP Installation Confirmation")

## PROJECT-1 git commit for Step 3.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step3](./image/gitCommit3.PNG "step 3 commit")

## Step 4: CREATING VIRTUAL HOST USING APACHE

#### Command:  sudo vi /etc/apache2/sites-available/projectlamp.conf (Creating a config file)
#### Output:

![config_file](./image/VH2.PNG "Config file")

#### Commands:  sudo a2ensite projectlamp, sudo a2dissite 000-default and sudo systemctl reload apache2 (Enabling Virtrual Host, disabling apache default websit and reloading apache)
#### Output:

![](./image/VH.PNG)

#### Commands:  sudo echo 'Hello LAMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) 'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectlamp/index.html (create index.html with content)
#### Output:

![](./image/index.PNG)

#### Commands: http://100.26.144.182/  (website is up and running)
#### Output:

![](./image/WS.PNG)

## Step 4: ENABLE PHP ON WEBSITE

#### Commands: sudo vim /etc/apache2/mods-enabled/dir.conf (changing the order of index.php)
#### Output:

![](./image/dirConf.PNG)

#### Commands:  vim /var/www/projectlamp/index.php (create index.php with content)
#### Output:

![](./image/index2.PNG)