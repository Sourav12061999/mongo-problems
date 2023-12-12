### Queries

1. 

```json
db.users.aggregate([{$group: {_id: null, avgAge: {$avg: "$age"}}}]).next().avgAge
```
 --> result 
 
 ``` json
 28.1
 ```