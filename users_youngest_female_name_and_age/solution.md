### Queries

1.

```json
db.users.find({gender:"female"}).sort({age:1}).limit(1).next().name
```

--> result

```json
 Alice
```
