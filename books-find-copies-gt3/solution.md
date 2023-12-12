### Queries

1. db.books.aggregate([ { $match: { available_copies: { $gt: 2 } } }, { $project: { _id: 0, title: 1 } }])

- Expected Output -

```
[
  { title: 'The Great Gatsby' },
  { title: 'To Kill a Mockingbird' }
]
```
