# here we will learn how to set up your database 
go to https://community.c9.io/t/setting-up-mongodb/1717 
install mongodb server:
sudo apt-get install -y mongodb-org
config it:
$ mkdir data
$ echo 'mongod --bind_ip=$IP --dbpath=data --nojournal --rest "$@"' > mongod
$ chmod a+x mongod

** note: you could install mongodb and the data directory anywhere 
but to make sure you dont accidently delete it, we install it outside of workspace 

