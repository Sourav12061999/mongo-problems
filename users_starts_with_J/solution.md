### Queries

1.
```json
  db.users.find({name:/^J/})

```

2. 
```json
db.users.find({name:{$regex:/^J/}})
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
    _id: ObjectId("642d1cace7c92502a7c0a017"),
    name: 'Jane',
    age: 30,
    email: 'jane@example.com',
    gender: 'female'
  }
]
```
