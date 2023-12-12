### Queries

1. 
```json
db.users.find({$and:[{gender:"male"},{age:{$gt:25}},{age:{$lt:35}}]})
```

 --> result

```json
[
  {
    _id: ObjectId("642d1cace7c92502a7c0a01a"),
    name: 'Tom',
    age: 27,
    email: 'tom@example.com',
    gender: 'male'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01c"),
    name: 'David',
    age: 32,
    email: 'david@example.com',
    gender: 'male'
  }
]
```
