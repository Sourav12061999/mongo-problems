### Queries

1. db.account_holders.find({ "accounts": 557378 })

- Expected Output -

```
{
  _id: ObjectId("6446704b9435fece47735373"),
  username: 'lyoung',
  name: 'Kaitlin Miller',
  address: '546 Tyler Prairie\n' +
    'Marybury, AL 54175',
  birthdate: 1985-05-27T08:39:47.000Z,
  email: 'mariahmcpherson@gmail.com',
  accounts: [
    794875,
    931314,
    557378
  ]
}
```
