### Queries

1. db.customers.aggregate([
  // unwind the orders array
  { $unwind: "$orders" },

  // match orders made in August 2022
  { $match: { "orders.date": { $regex: "^2022-08" } } },

  // count unique customers by their _id
  { $group: { _id: "$_id" } },

  { $count: "customerCount" }
]).next().customerCount

- 1
