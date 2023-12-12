### Queries

1. db.accounts.aggregate([
  {
    $group: {
      _id: null,
      avgBalance: { $avg: "$balance" }
    }
  }
])



- Expected Output -

```
{
  _id: null,
  avgBalance: 16000
}
```
