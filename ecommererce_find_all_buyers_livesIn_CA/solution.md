### Queries

1. db.buyers.find( { "address.state": { $in: [ "CA" ] } } )

   --> result

```
[
  {
    _id: 2,
    name: 'Jane Doe',
    email: 'jane@example.com',
    address: {
      street: '456 Elm St',
      city: 'Los Angeles',
      state: 'CA',
      zip: '90001'
    }
  },
  {
    _id: 4,
    name: 'Alice Lee',
    email: 'alice@example.com',
    address: {
      street: '321 Pine St',
      city: 'San Francisco',
      state: 'CA',
      zip: '94101'
    }
  }
]

```
