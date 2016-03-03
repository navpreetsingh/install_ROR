# Install_ROR

Please Install **Ruby on Rails** on your machines using **RVM**. Below commands work in Ubuntu O.S.

## Requirements

* [RVM](https://rvm.io/rvm/install)
* [Ruby](https://www.ruby-lang.org/en/)
* [Rails](http://rubyonrails.org/)

## Installing Ruby on Rails using RVM

```sh
$ gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
$ sudo apt-get install curl
$ \curl -sSL https://get.rvm.io | bash -s stable --rails
```

## Check Ruby & Rails Version

```sh
$ ruby --version
$ rails --version
```

## MAKING 2 SAMPLE APPS IN YOUR SYSTEM

**Run the below commands to create 2 sample projects**

```sh
$ rails new sample_app_1
$ rails new sample_app_1
```

**NOTE:** Copy the content in file **Gemfile_mysql** to your **Gemfile**, if you want to keep the database **mySQL**, else just copy the content of file **Gemfile_sqlite3** to your **Gemfile**\

## If choose **MYSQL** Db
**Run the below command.**
```sh
$ sudo apt-get install libmysqlclient-dev
```

**Install the Bundle**

```sh
$ bundle install
```

**Note:** If you choose mysql as the database, then copy the content of file **database_mysql.yml** to your file **config/database.yml**. Please change the **password** in **database** file.

**Create Database**

```sh
$ rake db:create
```

## HEROKU
**Create an Account on HEROKU**
* [HEROKU](https://www.heroku.com/)

**Install Heroku on System**

* [Install Heroku](https://toolbelt.heroku.com/debian)

**Check Version of Heroku**

```sh
$ heroku version
```

**Login to HEROKU**

```sh
$ heroku login
```

## ADDING SSH KEY TO YOUR SYSTEM

If you have **SSH** key in your system, then please skip this part

**Generating New SSH Key**
* [Generate SSH Key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

## ADDING SSH KEY TO HEROKU

```sh
$ heroku keys:add
```