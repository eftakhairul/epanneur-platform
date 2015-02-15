# e-panneur Platform    

### Version
0.0.1

### Installation (Tutorial based on OSX)

Install ruby 2.1.5:

```sh
rvm instal 2.1.5
```
Create gemset

```sh
rvm ruby-2.1.5@rails4.2.0  —create
```

Mysql Isntallation (If you don't have installed mysql in your PC)

```sh
brew update
brew doctor
brew upgrade
 	
brew install mysql
```

Restart the mysql 

```sh
mysql.server restart   
```

Start the mysql server at first time  

```sh
mysql.server start   
```

Secure mysql server   

```sh
mysql_secure_installation
```

Create Database
```sh
mysql -u root -p[your_mysql_password]

> create database epanneur_dev;
> create user epanneur identified by 'epanneur';
> use epanneur;
> grant all on epanneur_dev.* to 'epanneur'@localhost;
```

Clone the project

```sh
git clone git@bitbucket.org:epanneur-team/epanneur-platform.git
cd epanneur-platform
```

Run the project at 3000 port 
```sh
rake db:migrate
rails s 
```

Happy developing :) 



