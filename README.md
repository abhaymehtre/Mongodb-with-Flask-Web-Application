# Web-Application-using-Flask-and-Mongodb

## Commands to setup the mongodb on the machine.
1. curl -fsSL https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add -
2. apt-key list
3. echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.4.list
4. sudo apt update
5. sudo apt install mongodb-org
6. sudo systemctl start mongod.service
7. sudo systemctl status mongod
8. sudo systemctl enable mongod
