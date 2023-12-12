### Problem Description

## Given below bank account holders json data to perform mongo queries.

- given data - accounts, account holders, transactions

```
"accounts": [
  {
    "account_id": 557378,
    "balance": 10000,
  },
  {
    "account_id": 198100,
    "balance": 15000,
  },
  {
    "account_id": 674364,
    "balance": 18000,
  },
  {
    "account_id": 278603,
    "balance": 21000,
  }
]

"account_holders": [
  {
    "username": "lyoung",
    "name": "Kaitlin Miller",
    "address": "546 Tyler Prairie\nMarybury, AL 54175",
    "birthdate": {
      "$date": "1985-05-27T08:39:47.000Z"
    },
    "email": "mariahmcpherson@gmail.com",
    "accounts": [
      794875,
      931314,
      557378
    ]
  },
  {
    "username": "earroyo",
    "name": "Teresa Smith",
    "address": "477 Wall Inlet\nJasonhaven, NM 02213",
    "birthdate": {
      "$date": "1991-07-15T18:11:02.000Z"
    },
    "email": "melissapatrick@yahoo.com",
    "accounts": [
      198100,
      674364,
      278603,
      383777,
      209363
    ],
  }
]

"transactions": [
  {
    "account_id": 674364,
    "transactions": [
      {
        "date": {
          "$date": "2014-08-29T00:00:00.000Z"
        },
        "amount": 9592,
      },
      {
        "date": {
          "$date": "2016-11-21T00:00:00.000Z"
        },
        "amount": 1035,
      },
      {
        "date": {
          "$date": "1978-07-10T00:00:00.000Z"
        },
        "amount": 7301,
      },
      {
        "date": {
          "$date": "2009-12-11T00:00:00.000Z"
        },
        "amount": 3822,
      },
      {
        "date": {
          "$date": "2016-11-04T00:00:00.000Z"
        },
        "amount": 8282,
      },
      {
        "date": {
          "$date": "2002-05-03T00:00:00.000Z"
        },
        "amount": 7061,
      },
      {
        "date": {
          "$date": "2013-10-22T00:00:00.000Z"
        },
        "amount": 2853,
      },
      {
        "date": {
          "$date": "2016-06-09T00:00:00.000Z"
        },
        "amount": 8001,
      },
      {
        "date": {
          "$date": "2015-08-12T00:00:00.000Z"
        },
        "amount": 990,
      },
      {
        "date": {
          "$date": "2007-11-26T00:00:00.000Z"
        },
        "amount": 5418,
      },
      {
        "date": {
          "$date": "2011-09-15T00:00:00.000Z"
        },
        "amount": 9456,
      },
      {
        "date": {
          "$date": "2015-11-05T00:00:00.000Z"
        },
        "amount": 1515,
      },
      {
        "date": {
          "$date": "2006-09-29T00:00:00.000Z"
        },
        "amount": 9135,
      },
      {
        "date": {
          "$date": "2016-06-16T00:00:00.000Z"
        },
        "amount": 4501,
      }
    ]
  },
  {
    "account_id": 557378,
    "transactions": [
      {
        "date": {
          "$date": "2006-10-06T00:00:00.000Z"
        },
        "amount": 2561,
      },
      {
        "date": {
          "$date": "2000-06-19T00:00:00.000Z"
        },
        "amount": 9153,
      },
      {
        "date": {
          "$date": "2013-11-06T00:00:00.000Z"
        },
        "amount": 18,
      },
      {
        "date": {
          "$date": "2012-03-19T00:00:00.000Z"
        },
        "amount": 25,
      },
      {
        "date": {
          "$date": "2006-07-20T00:00:00.000Z"
        },
        "amount": 3265,
      },
      {
        "date": {
          "$date": "2002-10-24T00:00:00.000Z"
        },
        "amount": 4088,
      },
      {
        "date": {
          "$date": "2005-06-30T00:00:00.000Z"
        },
        "amount": 3037,
      },
      {
        "date": {
          "$date": "2010-08-20T00:00:00.000Z"
        },
        "amount": 154,
      },
      {
        "date": {
          "$date": "2016-09-02T00:00:00.000Z"
        },
        "amount": 7469,
      },
      {
        "date": {
          "$date": "2014-01-27T00:00:00.000Z"
        },
        "amount": 9837,
      },
    ]
  },
  {
    "account_id": 198100,
    "transactions": [
      {
        "date": {
          "$date": "2016-11-02T00:00:00.000Z"
        },
        "amount": 5202,
      },
      {
        "date": {
          "$date": "2006-07-20T00:00:00.000Z"
        },
        "amount": 4424,
      },
      {
        "date": {
          "$date": "2005-07-11T00:00:00.000Z"
        },
        "amount": 7914,
      },
      {
        "date": {
          "$date": "2016-10-06T00:00:00.000Z"
        },
        "amount": 3629,
      },
    ]
  },
  {
    "account_id": 278603,
    "transactions": [
      {
        "date": {
          "$date": "2000-05-22T00:00:00.000Z"
        },
        "amount": 247,
      },
      {
        "date": {
          "$date": "2015-08-17T00:00:00.000Z"
        },
        "amount": 9433,
      },
      {
        "date": {
          "$date": "2000-05-22T00:00:00.000Z"
        },
        "amount": 1832,
      },
      {
        "date": {
          "$date": "2016-01-11T00:00:00.000Z"
        },
        "amount": 5748,
      },
      {
        "date": {
          "$date": "2003-01-16T00:00:00.000Z"
        },
        "amount": 8183,
      },
      {
        "date": {
          "$date": "2012-06-27T00:00:00.000Z"
        },
        "amount": 511,
      },
      {
        "date": {
          "$date": "2015-07-17T00:00:00.000Z"
        },
        "amount": 9638,
      },
      {
        "date": {
          "$date": "2015-10-12T00:00:00.000Z"
        },
        "amount": 9145,
      },
      {
        "date": {
          "$date": "2000-02-11T00:00:00.000Z"
        },
        "amount": 191,
      },
      {
        "date": {
          "$date": "2015-07-02T00:00:00.000Z"
        },
        "amount": 6214,
      },
      {
        "date": {
          "$date": "2013-09-19T00:00:00.000Z"
        },
        "amount": 883,
      },
      {
        "date": {
          "$date": "1979-10-22T00:00:00.000Z"
        },
        "amount": 7723,
      },
      {
        "date": {
          "$date": "2010-11-16T00:00:00.000Z"
        },
        "amount": 837,
      },
      {
        "date": {
          "$date": "2010-07-20T00:00:00.000Z"
        },
        "amount": 9044,
      },
    ]
  }
]
```

### Query

- Retrieve all transactions for the account with an account_id of `674364` ?
