### Queries

1.  
```json
db.users.find({ name: /n$/ })
```

2. 

```json
db.users.find({name:{$regex:/n$/}})
```

--> result

```json
[
  {
    _id: ObjectId("642d1cace7c92502a7c0a016"),
    name: 'John',
    age: 25,
    email: 'john@example.com',
    gender: 'male'
  }
]
```
