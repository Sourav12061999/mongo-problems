### Queries

1.

````json
db.orders.aggregate([{
    $lookup: {from: "buyers", localField: "customer_id", foreignField: "_id", as: "customer"}
    },
    {
    $match: {"customer.address.city": "New York", status: "shipped"}
    }
    ])
    ```

- Result -

```json
[
  {
    _id: 1,
    customer_id: 1,
    order_date: '2022-03-01',
    ship_date: '2022-03-05',
    status: 'shipped',
    total: 50.25,
    customer: [
      {
        _id: 1,
        name: 'John Smith',
        email: 'john@example.com',
        address: {
          street: '123 Main St',
          city: 'New York',
          state: 'NY',
          zip: '10001'
        }
      }
    ]
  },
  {
    _id: 2,
    customer_id: 1,
    order_date: '2022-03-15',
    ship_date: '2022-03-18',
    status: 'shipped',
    total: 25.5,
    customer: [
      {
        _id: 1,
        name: 'John Smith',
        email: 'john@example.com',
        address: {
          street: '123 Main St',
          city: 'New York',
          state: 'NY',
          zip: '10001'
        }
      }
    ]
````
