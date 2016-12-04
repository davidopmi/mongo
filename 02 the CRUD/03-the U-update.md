.update() is used to update document into a collection

1: to replace the existing document with the document passed in
>db.COLLECTION_NAME.update(SELECTION_CRITERIA, UPDATED_DATA)
db.dogs.update({name:"d1"},{country:"CHN"})

2: to update value but not overwrite 
db.dogs.update({name:"d2"},{$set:{country:"CHN"}})

3: to update multiple records 
db.dogs.update({age:{$gte: 30}},{$set:{country:"usa"}},{multi:true})