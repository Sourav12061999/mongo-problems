### Queries

1. 
```json
db.users.find().sort({age:-1}).limit(1).next().name
```
--> result

```json
'Bob'
```
