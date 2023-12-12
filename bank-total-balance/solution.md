### Queries

1. db.accounts.aggregate([
  {
    $group: {
      _id: null,
      totalBalance: { $sum: "$balance" }
    }
  }
])


- Expected Output -

```
{
  _id: null,
  totalBalance: 64000
}
```
