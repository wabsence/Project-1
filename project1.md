# DOCUMENTATION

## Step 1: APACHE INSTALLATION

#### Command: sudo apt update (Packages update in Package Manager)
#### Output:

![packages Updated](images/packages.png "packages update process")

#### Command: sudo apt install apache2 (Apache 2 Installation)
#### Output:

![apache2 Installation](images/apache2Inst.png "apache2 installation process")

#### Command: sudo systemctl status apache2 (Apache Status Confirmation)
#### Output:

![apache2 Installation](images/apacheState.png "apache in running state")

#### Command:  curl http://127.0.0.1:80 (Using curl to access server via IP address)
#### Output:

![Accessingg Server](images/curlAccess.png "accessing server via IP address")

#### Command:  http://100.26.144.182/ (Accessing IP address via browser)
#### Output:

![Accessingg Server](images/apacheServer.png "accessing apache server")

## PROJECT-1 GIT INITIALIZATION AND FIRST COMMIT i.e running git commit for Step 1.

#### Command:  git init & git status (Project-1 git initialization and check status to see changes)
#### Output:

![Git initialization](images/gitInit.png "git initialization")

#### Commands:  git add . | git status | git commit (Staging and commiting files)
#### Outputs:

![Staging](images/gitAdd.png "Staging all files to commit")

![Commit_Files](images/commitFiles.png "Files Commited")

## Step 2: MYSQL INSTALLATION

#### Command: sudo apt install mysql-server (Mysql Installation)
#### Output:

![MYSQL_1](images/mysq.png "MYSQL Installation")

#### Command: $ sudo mysql (Mysql Installation)
#### Output:

![MYSQL_2](images/mysq2.png "MYSQL Installation")

#### Command: $ sudo mysql_secure_installation (Mysql Installation)
#### Output:

![MYSQL_3](images/mysq3.png "MYSQL Installation")

![MYSQL_4](images/mysq4.png "MYSQL Console login")

## PROJECT-1 git commit for Step 2. 

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![git commit](images/gitCommit2.png "git commit")

## Step 3: PHP INSTALLATION

#### Command: $ sudo apt install php libapache2-mod-php php-mysql (Php and other packages Installation)
#### Output:

![PHP](images/php.png "PHP Installation")

#### Command: $ php -V (Php  Installation Confirmation)
#### Output:

![PHP](images/php2.png "PHP Installation Confirmation")

## PROJECT-1 git commit for Step 3.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![gitCommit](images/gitCommit3.png "git commit")

## Step 4: CREATING VIRTUAL HOST FOR WEBSITE USING APACHE

#### Command:  sudo vi /etc/apache2/sites-available/projectlamp.conf (Creating a config file)
#### Output:

![config_file](images/VH2.png "Config file")

#### Commands:  sudo a2ensite projectlamp, sudo a2dissite 000-default and sudo systemctl reload apache2 (Enabling Virtrual Host, disabling apache default websit and reloading apache)
#### Output:

![VH](images/VH.png)

#### Commands:  sudo echo 'Hello LAMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) 'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectlamp/index.html (create index.html with content)
#### Output:

![Index](images/index1.png)

#### Commands: http://100.26.144.182/  (website is up and running)
#### Output:

![Website](images/WS.png)

## Step 4: ENABLE PHP ON WEBSITE

#### Commands: sudo vim /etc/apache2/mods-enabled/dir.conf (changing the order of index.php)
#### Output:

![DirConf](images/dConf.png)

#### Commands:  vim /var/www/projectlamp/index.php (create index.php with content)
#### Output:

![Index](images/index2.png)
