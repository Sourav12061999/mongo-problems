### Queries

1. 
```json
db.users.find({}, {name: 1, age: 1})
```

 --> result

```
[
  {
    _id: ObjectId("642d1cace7c92502a7c0a016"),
    name: 'John',
    age: 25
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a017"),
    name: 'Jane',
    age: 30
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a018"),
    name: 'Bob', a
    age: 35
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a019"),
    name: 'Alice',
    age: 20
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a01a"),
    name: 'Tom', a
    ge: 27
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a01b"),
    name: 'Mary',
    age: 29
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a01c"),
    name: 'David',
     age: 32
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a01d"),
    name: 'Emily',
    age: 28
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a01e"),
    name: 'Max', a
    ge: 24
  },

  {
    _id: ObjectId("642d1cace7c92502a7c0a01f"),
    name: 'Sophia',
    age: 31
  }
]
```
