### Queries

1. db.customers.find({name:"Alice Lee"}).next().orders[0].date
- '2022-07-01'
2. db.customers.findOne({name:"Alice Lee"}).orders[0].date
- '2022-07-01'