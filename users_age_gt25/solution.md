### Queries

1.

```json
db.users.find({age:{$gt:25}})
```

--> result

```json
[
  {
    _id: ObjectId("642d1cace7c92502a7c0a017"),
    name: 'Jane',
    age: 30,
    email: 'jane@example.com',
    gender: 'female'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a018"),
    name: 'Bob',
    age: 35,
    email: 'bob@example.com',
    gender: 'male'
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
    _id: ObjectId("642d1cace7c92502a7c0a01c"),
    name: 'David',
    age: 32,
    email: 'david@example.com',
    gender: 'male'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01d"),
    name: 'Emily',
    age: 28,
    email: 'emily@example.com',
    gender: 'female'
  },
  {
    _id: ObjectId("642d1cace7c92502a7c0a01f"),
    name: 'Sophia',
    age: 31,
    email: 'sophia@example.com',
    gender: 'female'
  }
]
```
