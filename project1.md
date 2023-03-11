# DOCUMENTATION

## Step 1: APACHE INSTALLATION

#### Command: sudo apt update (Packages update in Package Manager)
#### Output:

![packages Updated](/Project-1/images/packagesUpdateOutput.png?raw=true "packages update process")

#### Command: sudo apt install apache2 (Apache 2 Installation)
#### Output:

![apache2 Installation](/Project-1/images/apache2Installation.png?raw=true "apache2 installation process")

#### Command: sudo systemctl status apache2 (Apache Status Confirmation)
#### Output:

![apache2 Installation](/Project-1/images/apacheStatus.png?raw=true "apache in running state")

#### Command:  curl http://127.0.0.1:80 (Using curl to access server via IP address)
#### Output:

![Accessingg Server](/Project-1/images/curlAccessServerViaIP.png?raw=true "accessing server via IP address")

#### Command:  http://100.26.144.182/ (Accessing IP address via browser)
#### Output:

![Accessingg Server](/Project-1/images/apacheServer.png?raw=true "accessing apache server")

## PROJECT-1 GIT INITIALIZATION AND FIRST COMMIT i.e running git commit for Step 1.

#### Command:  git init & git status (Project-1 git initialization and check status to see changes)
#### Output:

![Git initialization](/Project-1/images/project1GitInitialization.PNG?raw=true "git initialization")

#### Commands:  git add . | git status | git commit (Staging and commiting files)
#### Outputs:

![Staging](/Project-1/images/gitAdd.png?raw=true "Staging all files to commit")

![Commiting all files](/Project-1/images/step1Done.png?raw=true "Files Commited")

## Step 2: MYSQL INSTALLATION

#### Command: sudo apt install mysql-server (Mysql Installation)
#### Output:

![MYSQL](/Project-1/images/MySQL.PNG?raw=true "MYSQL Installation")

#### Command: $ sudo mysql (Mysql Installation)
#### Output:

![MYSQL](/Project-1/images/MySQL2.PNG?raw=true "MYSQL Installation")

#### Command: $ sudo mysql_secure_installation (Mysql Installation)
#### Output:

![MYSQL](/Project-1/images/MySQL3.PNG?raw=true "MYSQL Installation")


## Step 2: MYSQL INSTALLATION

![MYSQL](/Project-1/images/MySQL4.PNG?raw=true "MYSQL Console login")

## PROJECT-1 git commit for Step 2.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step2](/Project-1/images/gitCommit2.PNG?raw=true "step 2 commit")

## Step 3: PHP INSTALLATION

#### Command: $ sudo apt install php libapache2-mod-php php-mysql (Php and other packages Installation)
#### Output:

![PHP](/Project-1/images/php.PNG?raw=true "PHP Installation")

#### Command: $ php -V (Php  Installation Confirmation)
#### Output:

![PHP](/Project-1/images/php2.PNG?raw=true "PHP Installation Confirmation")

## PROJECT-1 git commit for Step 3.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step3](/Project-1/images/gitCommit3.PNG?raw=true "step 3 commit")

## Step 4: CREATING VIRTUAL HOST USING APACHE

#### Command:  sudo vi /etc/apache2/sites-available/projectlamp.conf (Creating a config file)
#### Output:

![config_file](/Project-1/images/VH2.png?raw=true "Config file")

#### Commands:  sudo a2ensite projectlamp, sudo a2dissite 000-default and sudo systemctl reload apache2 (Enabling Virtrual Host, disabling apache default websit and reloading apache)
#### Output:

![VH](/Project-1/images/VH.PNG?raw=true)

#### Commands:  sudo echo 'Hello LAMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) 'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectlamp/index.html (create index.html with content)
#### Output:

![Index](/Project-1/images/index.PNG?raw=true)

#### Commands: http://100.26.144.182/  (website is up and running)
#### Output:

![WS](/Project-1/images/WS.png)

## Step 4: ENABLE PHP ON WEBSITE

#### Commands: sudo vim /etc/apache2/mods-enabled/dir.conf (changing the order of index.php)
#### Output:

![DirConf](/Project-1/images/dirConf.PNG?raw=true)

#### Commands:  vim /var/www/projectlamp/index.php (create index.php with content)
#### Output:

![Index](/Project-1/images/index2.PNG?raw=true)