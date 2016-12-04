1: to check available databases:
show dbs 
2: to check the current database you are using:
db 
3: to create(if not exist)/or use an existing database:
use mydb
> switched to db mydb

note: if your database does not have any collections in it, then show dbs will not show you the database

4: drop/delete database
db.dropDatabase() 
>{ "dropped" : "mydb", "ok" : 1 }
