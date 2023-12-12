### Queries

1. 
```json
db.users.find({gender: "male", age:{$gt:30}})
```

2. 
```json
db.users.find({$and:[{gender:"male"},{age:{$gt:30}}]})
```

--> result

```
[
  {
    _id: ObjectId("642d1cace7c92502a7c0a018"),
    name: 'Bob',
    age: 35,
    email: 'bob@example.com',
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