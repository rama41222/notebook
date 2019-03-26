### How to drop Mongo Database

```
> show dbs

    admin 0.000GB
    local 0.000GB
    abc 0.000GB
    
> use abc
    switched to db abc
    
> db.dropDatabase()
    { "dropped" : "abc", "ok" : 1 }
    
> show dbs
    admin 0.000GB
    local 0.000GB
```
> 
