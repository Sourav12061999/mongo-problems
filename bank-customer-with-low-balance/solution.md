### Queries

1. db.accounts.aggregate([
  {
    $sort: { balance: 1 }
  },
  {
    $limit: 1
  }
])


- Expected Output -

```
{
  _id: ObjectId("6446b061d59b37a08d87c353"),
  account_id: 557378,
  balance: 10000
}
```
