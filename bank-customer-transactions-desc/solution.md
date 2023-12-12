### Queries

1. db.transactions.find({ "account_id": 557378 }).sort({date:-1})

- Expected Output -

```
[
  {
    _id: ObjectId("644670639435fece47735377"),
    account_id: 557378,
    transactions: [
      { date: { '$date': '2006-10-06T00:00:00.000Z' }, amount: 2561 },
      { date: { '$date': '2000-06-19T00:00:00.000Z' }, amount: 9153 },
      { date: { '$date': '2013-11-06T00:00:00.000Z' }, amount: 18 },
      { date: { '$date': '2012-03-19T00:00:00.000Z' }, amount: 25 },
      { date: { '$date': '2006-07-20T00:00:00.000Z' }, amount: 3265 },
      { date: { '$date': '2002-10-24T00:00:00.000Z' }, amount: 4088 },
      { date: { '$date': '2005-06-30T00:00:00.000Z' }, amount: 3037 },
      { date: { '$date': '2010-08-20T00:00:00.000Z' }, amount: 154 },
      { date: { '$date': '2016-09-02T00:00:00.000Z' }, amount: 7469 },
      { date: { '$date': '2014-01-27T00:00:00.000Z' }, amount: 9837 }
    ]
  }
]
```
