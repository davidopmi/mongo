1: show created collections:
show collections

2: create a new collection 
db.createCollection('dogs')

note: in no-sql database, you dont need to predefine the schema of a collection! and it can host any value/columes

3: or if you want to create a collection and at the same time insert a record:
db.dogs.insert({name:"david", sex:"male"})

4: drop/delete a collection
db.dogs.drop()

note: db refers to the current database you are on 

