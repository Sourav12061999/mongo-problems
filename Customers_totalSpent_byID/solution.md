### Queries

1. db.customers.find({_id:5}).next().orders.reduce(
  (accumulator, currentValue) => accumulator + currentValue.total,
  0
);
- 155.75