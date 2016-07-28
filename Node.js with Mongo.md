
![Log](https://www.learn2crack.com/wp-content/uploads/2014/04/node-cover.png)


## Retrieve all data from database
```
ModelName.find({}, fucntion(error, allData){
  if(error){
    console.log("ERROR", error)
    }else{
      console.log(allData)
    }
});
```
## Retrieve data ids only (ObjectID)
```
ModelName.find({},{_id:1}, function(error, dataID){
  if(error){
    console.log("ERROR", error)
  }else{
      console.log(dataID)
  }
}):
```
## Create new data entry 
```
var modelForm = {
  name:"firstName",
  aga :"useAge"
}
```
- note: modelForm is an JSON object
```
ModelName.create(modelForm, function(err, newData){
        if(err){
            console.log(err);
        } else {
           consnole.log(newData)
        }
    });
```

## find data by ID
```
var id = req.params.id;
```
-note: id is taken from the rout  ("/user/:id")
```
 ModelName.findById(id, function(error, foundData) {
        if (error){
            console.log(err);
        }else{
             console.log(foundData);
        }
    });

```    

##Find data by Id and Update
```
var id = req.params.id;
var firstName = req.body.firstName;
```
- note firstName is taken from the Model Schema
```
ModelName.findByIdAndUpdate(id, firstName, function(error, updatedPost){
       if (error){
            console.log(err);
        }else{
             console.log(updatedPost);
        }
    });
```

## Find data by ID and Remove 
 ```
 var postId = req.params.id;
 ```
  ```
  ModelName.findByIdAndRemove(postId, function(error, removedPost){
       if (error){
            console.log(err);
        }else{
             console.log(removedPost);
        }
       
   });
  ```  

## Get OjectID mongodb entry:
```
var id = mongoose.Types.ObjectId(this.id)
```
