### Queries
```
1. db.customers.aggregate([
  { $unwind: "$orders" },
  {
    $match: {
      "orders.total": { $gt: 50 }
    }
  },
  {
    $group: {
      _id: null,
      totalOrders: { $sum: 1 }
    }
  }
]).next().totalOrders


```
- 7