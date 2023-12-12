### Queries

1. 
```json
db.users.find({age:{$lte:29}})
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
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a019"),
    name: 'Alice',
    age: 20,
    email: 'alice@example.com',
    gender: 'female'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01a"),
    name: 'Tom',
    age: 27,
    email: 'tom@example.com',
    gender: 'male'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01b"),
    name: 'Mary',
    age: 29,
    email: 'mary@example.com',
    gender: 'female'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01d"),
    name: 'Emily',
    age: 28,
    email: 'emily@example.com',
    gender: 'female'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01e"),
    name: 'Max',
    age: 24,
    email: 'max@example.com',
    gender: 'male'
  }
]
```
