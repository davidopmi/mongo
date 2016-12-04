# here we will learn how to set up your database 
go to https://community.c9.io/t/setting-up-mongodb/1717 
install mongodb server:
sudo apt-get install -y mongodb-org
config it:
$ mkdir data
$ echo 'mongod --bind_ip=$IP --dbpath=data --nojournal --rest "$@"' > mongod
$ chmod a+x mongod

mongod is the Daemon: program to run the mongodb server 
a daemon is a computer program that runs as a background process, 
rather than being under the direct control of an interactive user. 

to run the server(have to run it obove the workspace folder): ./mongod
to run the client(you can run it anywhere): mongo 
to stop the server/client : ctrl+c 

** note: you could install mongodb and the data directory anywhere 
but to make sure you dont accidently delete it, we install it outside of workspace 

*** please close your mongodb server before you end your program 

## command to try:
help 