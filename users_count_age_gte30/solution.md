### Queries

1. 
```json
db.users.countDocuments({age:{$gte:30}})
```
2. 
```json 
db.users.count({age:{$gte:30}})
```
--> result 
```json
4
```
