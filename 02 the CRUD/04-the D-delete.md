MongoDB's .remove() method is used to remove a document from the collection. 
remove() method accepts two parameters. One is deletion criteria and second is justOne flag.

1: to remove matching documents: default behaviro 
db.dogs.remove({isMale:true})

2: to remove ONLY one matching document 
db.dogs.remove({isMale:true}, 1)

3: deleate all the documents == truncate table 
db.dogs.remove() 
