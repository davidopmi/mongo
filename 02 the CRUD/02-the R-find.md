To query data from MongoDB collection, you need to use MongoDB's .find()method.

1: db.dogs.find() 
will display ALL the documents(records) in a non-structured way

2: db.dogs.find().pretty() 
To display the results in a formatted way

3: db.dogs.findOne():
will display only ONE document 

4: where Clause Equivalents in MongoDB
db.dogs.find({isMale:true})
db.dogs.find({age:{$gte:40}}): greate than equals
* and
db.dogs.find({$and:[{isMale:true},{age:{$gt:30}}]})
* or 
db.dogs.find({$or:[{isMale:true},{age:{$gt:30}}]})