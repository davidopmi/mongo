1: to insert one record: pass in a js object
db.dogs.insert({name:"lee", sex:"male"})

2: to insert multiple record, how to pass in an array 
db.dogs.insert([{name:"david", sex:"male"}, {name:"jack", sex:"female"}])
db.dogs.insert([{name:"d1", age: 50, isMale: true}, 
{name:"d2", age:40, isMale:false}, 
{name:"d3", age:30, isMale:true}])

note: please refer to the supported data types in mongodb
common ones: 
String "", 
Integer : 50 , 
Double: 35.5, 
Boolean: true/false
js object, Date: create object of Date and passing day, month, year into it. 
Null: null
Binary data: like image or file 