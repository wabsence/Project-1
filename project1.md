# DOCUMENTATION

## Step 1: APACHE INSTALLATION

#### Command: sudo apt update (Packages update in Package Manager)
#### Output:

![packages Updated](https://github.com/wabsence/Project-1/blob/master/images/packagesUpdateOutput.png "packages update process")

#### Command: sudo apt install apache2 (Apache 2 Installation)
#### Output:

![apache2 Installation](https://github.com/wabsence/Project-1/blob/master/images/apache2Installation.png "apache2 installation process")

#### Command: sudo systemctl status apache2 (Apache Status Confirmation)
#### Output:

![apache2 Installation](https://github.com/wabsence/Project-1/blob/master/images/apacheStatus.png "apache in running state")

#### Command:  curl http://127.0.0.1:80 (Using curl to access server via IP address)
#### Output:

![Accessingg Server](https://github.com/wabsence/Project-1/blob/master/images/curlAccessServerViaIP.png "accessing server via IP address")

#### Command:  http://100.26.144.182/ (Accessing IP address via browser)
#### Output:

![Accessingg Server](https://github.com/wabsence/Project-1/blob/master/images/apacheServer.png "accessing apache server")

## PROJECT-1 GIT INITIALIZATION AND FIRST COMMIT i.e running git commit for Step 1.

#### Command:  git init & git status (Project-1 git initialization and check status to see changes)
#### Output:

![Git initialization](https://github.com/wabsence/Project-1/blob/master/images/project1GitInitialization.PNG "git initialization")

#### Commands:  git add . | git status | git commit (Staging and commiting files)
#### Outputs:

![Staging](https://github.com/wabsence/Project-1/blob/master/images/gitAdd.PNG "Staging all files to commit")

![Commiting all files](https://github.com/wabsence/Project-1/blob/master/images/step1Done.PNG "Files Commited")

## Step 2: MYSQL INSTALLATION

#### Command: sudo apt install mysql-server (Mysql Installation)
#### Output:

![MYSQL](https://github.com/wabsence/Project-1/blob/master/images/MySQL.PNG "MYSQL Installation")

#### Command: $ sudo mysql (Mysql Installation)
#### Output:

![MYSQL](https://github.com/wabsence/Project-1/blob/master/images/MySQL2.PNG "MYSQL Installation")

#### Command: $ sudo mysql_secure_installation (Mysql Installation)
#### Output:

![MYSQL](https://github.com/wabsence/Project-1/blob/master/images/MySQL3.PNG "MYSQL Installation")


## Step 2: MYSQL INSTALLATION

![MYSQL](https://github.com/wabsence/Project-1/blob/master/images/MySQL4.PNG "MYSQL Console login")

## PROJECT-1 git commit for Step 2.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step2](https://github.com/wabsence/Project-1/blob/master/images/gitCommit2.PNG "step 2 commit")

## Step 3: PHP INSTALLATION

#### Command: $ sudo apt install php libapache2-mod-php php-mysql (Php and other packages Installation)
#### Output:

![PHP](https://github.com/wabsence/Project-1/blob/master/images/php.PNG "PHP Installation")

#### Command: $ php -V (Php  Installation Confirmation)
#### Output:

![PHP](https://github.com/wabsence/Project-1/blob/master/images/php2.PNG "PHP Installation Confirmation")

## PROJECT-1 git commit for Step 3.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step3](.https://github.com/wabsence/Project-1/blob/master/images/gitCommit3.PNG "step 3 commit")

## Step 4: CREATING VIRTUAL HOST USING APACHE

#### Command:  sudo vi /etc/apache2/sites-available/projectlamp.conf (Creating a config file)
#### Output:

![config_file](https://github.com/wabsence/Project-1/blob/master/images/VH2.PNG "Config file")

#### Commands:  sudo a2ensite projectlamp, sudo a2dissite 000-default and sudo systemctl reload apache2 (Enabling Virtrual Host, disabling apache default websit and reloading apache)
#### Output:

![VH](https://github.com/wabsence/Project-1/blob/master/images/VH.PNG)

#### Commands:  sudo echo 'Hello LAMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) 'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectlamp/index.html (create index.html with content)
#### Output:

![Index](https://github.com/wabsence/Project-1/blob/master/images/index.PNG)

#### Commands: http://100.26.144.182/  (website is up and running)
#### Output:

![WS](https://github.com/wabsence/Project-1/blob/master/images/WS.PNG)

## Step 4: ENABLE PHP ON WEBSITE

#### Commands: sudo vim /etc/apache2/mods-enabled/dir.conf (changing the order of index.php)
#### Output:

![DirConf](https://github.com/wabsence/Project-1/blob/master/images/dirConf.PNG)

#### Commands:  vim /var/www/projectlamp/index.php (create index.php with content)
#### Output:

![Index](https://github.com/wabsence/Project-1/blob/master/images/index2.PNG)