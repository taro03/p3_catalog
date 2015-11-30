# Fullstack Udacity Project - Catalog

OAuth2.0
Starter Code for Auth&amp;Auth course

### About
Develop an application that provides a list of items within a variety of categories as well as provide a user registration and authentication system using OAuth2.0. Registered users will have the ability to make change of catalog

### Requirements
* python
* [flask](http://flask.pocoo.org) 
* [sqlalchemy](http://www.sqlalchemy.org)
* [vagrant](https://www.vagrantup.com/downloads)

### Setup
1.Fetch the Source Code and VM Configuration

**Windows:** Use the Git Bash program (installed with Git) to get a Unix-style terminal.  
**Other systems:** Use your favorite terminal program.

From the terminal, run:

    git clone https://github.com/taro03/p3_catalog.git

This will give you a directory named **p3_catalog** complete with the source code for the flask application, a vagrantfile, and a bootstrap.sh file for installing all of the necessary tools. 

2.Edit the /templates/login.html with your own google and facebook application id

line 17:    `data-clientid="your google app id"`

line 63:    `appID:'your facebook app id'`

Follow below links to know how to create Google and Facebook app id
- Google app id: https://www.youtube.com/watch?v=8aGoty0VXgw
- Facebook app id: https://www.youtube.com/watch?v=3FRNU35Km2s


### Usage
1.Initialize the Vagrant vm via `vagrant up`, which should set up on `localhost:5000`.
2.Connect to the virtual machine: `vagrant ssh`.
3.Navigate to the catalog directory: `cd /vagrant/p3_catalog`
4.Setup the databse and add fake data the the database
```bash
[yourmachine@p3_catalog] python database_setup.py
[yourmachine@p3_catalog] python lotsofmenus.py
```
5.Start the application
```bash
[yourmachine@p3_catalog] python project.py
```
6.Open the web browser and enter
```bash
http://localhost:5000
```
