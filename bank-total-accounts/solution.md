### Queries

1. db.accounts.aggregate([
   {
   $group: {
   _id: null,
   count: { $sum: 1 }
   }
   }
   ])

- Expected Output -

```
{
  _id: null,
  count: 4
}
```
