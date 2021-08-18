# Web-Application-using-Flask-and-Mongodb

#### A simple web application that is developed using python using flask service. This application gives an idea of using multiple VM's for the code execution and the deployment on different virtual machines.

## Commands to setup the flask and python services.
Installation of Python3 and its packages:

•	Please follow the below commands, if there is any difficulty in installing the python packages.

o	Command 1: sudo apt update

o	Command 2: sudo apt install software-properties-common

o	Command 3: sudo add-apt-repository ppa:deadsnakes/ppa

o	Command 4: sudo apt install python3.9

•	Verification of the installation was successful.

o	Command: python3.9 –version

That’s it. Python 3.9 is installed on your Ubuntu, and you can start using it.

## Commands to install python dependencies
1. sudo apt install python3-pip
2. pip3 install Flask
3. pip3 install bson
4. pip3 install pymongo

## Commands to setup the mongodb on the machine.
1. curl -fsSL https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add -
2. apt-key list
3. echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.4.list
4. sudo apt update
5. sudo apt install mongodb-org
6. sudo systemctl start mongod.service
7. sudo systemctl status mongod
8. sudo systemctl enable mongod

## Setting up of the database:
Once the installation of the Mongo db is complete using the commands mentioned above.
Please follow the below stuff to configure the database as required for the application run properly.
1. command 1 : mongo ( This will open the CLI interface in the terminal , connect to the mongo database)
2. Command 2 : show dbs; ( Shows list of databases present)
3. Command 3 : use mymongodb ( Creates a new database)
4. Command 4 : db.createCollection(name) ( Creates an new collection and ensure that the collection name here used is todo). 
Syntax or command that need to be used is : db.createCollection("todo"); This will create the collection under the mymongodb database.

After the completion of the all these setup you can fire up your web based application by using python3 app.py.

## Output : 

Serving Flask app "main" (lazy loading)
 * Environment: production
   WARNING: This is a development server.
   Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Running on http://<ip-address>:5000/ (Press CTRL+C to quit)
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: (random generated)


Use the above generated ip address along with the port number on other Virtual Machine for generating the result.
  
  Good Luck !!!

