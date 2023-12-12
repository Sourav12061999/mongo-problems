### Queries

1. db.customers.findOne({email:"john@example.com"}).address.city
- 'New York'
2. db.customers.find({email:"john@example.com"}).next().address.city
- 'New York'