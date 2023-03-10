# DOCUMENTATION

## Step 1: APACHE INSTALLATION

#### Command: sudo apt update (Packages update in Package Manager)
#### Output:

![packages Updated](./images/packagesUpdateOutput.png "packages update process")

#### Command: sudo apt install apache2 (Apache 2 Installation)
#### Output:

![apache2 Installation](./images/apache2Installation.png "apache2 installation process")

#### Command: sudo systemctl status apache2 (Apache Status Confirmation)
#### Output:

![apache2 Installation](./images/apacheStatus.png "apache in running state")

#### Command:  curl http://127.0.0.1:80 (Using curl to access server via IP address)
#### Output:

![Accessingg Server](./images/curlAccessServerViaIP.png "accessing server via IP address")

#### Command:  http://100.26.144.182/ (Accessing IP address via browser)
#### Output:

![Accessingg Server](./images/apacheServer.png "accessing apache server")

## PROJECT-1 GIT INITIALIZATION AND FIRST COMMIT i.e running git commit for Step 1.

#### Command:  git init & git status (Project-1 git initialization and check status to see changes)
#### Output:

![Git initialization](./images/project1GitInitialization.PNG "git initialization")

#### Commands:  git add . | git status | git commit (Staging and commiting files)
#### Outputs:

![Staging](./images/gitAdd.PNG "Staging all files to commit")

![Commiting all files](./images/step1Done.PNG "Files Commited")

## Step 2: MYSQL INSTALLATION

#### Command: sudo apt install mysql-server (Mysql Installation)
#### Output:

![MYSQL](./images/MySQL.PNG "MYSQL Installation")

#### Command: $ sudo mysql (Mysql Installation)
#### Output:

![MYSQL](./images/MySQL2.PNG "MYSQL Installation")

#### Command: $ sudo mysql_secure_installation (Mysql Installation)
#### Output:

![MYSQL](./images/MySQL3.PNG "MYSQL Installation")


## Step 2: MYSQL INSTALLATION

![MYSQL](./images/MySQL4.PNG "MYSQL Console login")

## PROJECT-1 git commit for Step 2.

#### Commands:  git add . |  git commit (Staging and commiting files)
#### Outputs:

![step2](./images/gitCommit2.PNG "step 2 commit")

## Step 3: PHP INSTALLATION

#### Command: $ sudo apt install php libapache2-mod-php php-mysql (Php and other packages Installation)
#### Output:

![PHP](./images/php.PNG "PHP Installation")

#### Command: $ php -V (Php  Installation Confirmation)
#### Output:

![PHP](./images/php2.PNG "PHP Installation Confirmation")
