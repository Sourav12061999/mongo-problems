### Queries

1. db.transactions.find({ "account_id": 674364 })

- Expected Output -

```
[
  {
    _id: ObjectId("6446aeeed59b37a08d87c346"),
    account_id: 674364,
    transactions: [
      { date: { '$date': '2014-08-29T00:00:00.000Z' }, amount: 9592 },
      { date: { '$date': '2016-11-21T00:00:00.000Z' }, amount: 1035 },
      { date: { '$date': '1978-07-10T00:00:00.000Z' }, amount: 7301 },
      { date: { '$date': '2009-12-11T00:00:00.000Z' }, amount: 3822 },
      { date: { '$date': '2016-11-04T00:00:00.000Z' }, amount: 8282 },
      { date: { '$date': '2002-05-03T00:00:00.000Z' }, amount: 7061 },
      { date: { '$date': '2013-10-22T00:00:00.000Z' }, amount: 2853 },
      { date: { '$date': '2016-06-09T00:00:00.000Z' }, amount: 8001 },
      { date: { '$date': '2015-08-12T00:00:00.000Z' }, amount: 990 },
      { date: { '$date': '2007-11-26T00:00:00.000Z' }, amount: 5418 },
      { date: { '$date': '2011-09-15T00:00:00.000Z' }, amount: 9456 },
      { date: { '$date': '2015-11-05T00:00:00.000Z' }, amount: 1515 },
      { date: { '$date': '2006-09-29T00:00:00.000Z' }, amount: 9135 },
      { date: { '$date': '2016-06-16T00:00:00.000Z' }, amount: 4501 }
    ]
  }
]
```
