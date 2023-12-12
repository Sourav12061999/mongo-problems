<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write Mongo query to retrieve the `name` and `city` from the `customers` where the `age` is less than `30`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "name": "Jane Doe",
    "city": "Los Angeles"
  }
]
```

<h4 style="color:#397ce7">Sample Database:</h4>

```javascript
customers: {
  [
    {
      _id: 1,
      name: "John Smith",
      age: 35,
      email: "john@example.com",
      address: {
        street: "123 Main St",
        city: "New York",
        state: "NY",
        zip: "10001",
      },
      orders: [
        { id: 1, date: "2022-03-01", total: 50.25 },
        { id: 2, date: "2022-03-15", total: 25.5 },
        { id: 3, date: "2022-04-01", total: 75.0 },
      ],
    },
    {
      _id: 2,
      name: "Jane Doe",
      age: 28,
      email: "jane@example.com",
      address: {
        street: "456 Elm St",
        city: "Los Angeles",
        state: "CA",
        zip: "90001",
      },
      orders: [
        { id: 4, date: "2022-04-15", total: 100.0 },
        { id: 5, date: "2022-05-01", total: 75.0 },
      ],
    },
    {
      _id: 3,
      name: "Bob Johnson",
      age: 42,
      email: "bob@example.com",
      address: {
        street: "789 Oak St",
        city: "Chicago",
        state: "IL",
        zip: "60601",
      },
      orders: [
        { id: 6, date: "2022-05-15", total: 50.75 },
        { id: 7, date: "2022-06-01", total: 25.5 },
        { id: 8, date: "2022-06-15", total: 35.0 },
      ],
    },
    {
      _id: 4,
      name: "Alice Lee",
      age: 23,
      email: "alice@example.com",
      address: {
        street: "321 Pine St",
        city: "San Francisco",
        state: "CA",
        zip: "94101",
      },
      orders: [{ id: 9, date: "2022-07-01", total: 125.5 }],
    },
    {
      _id: 5,
      name: "Tom Wilson",
      age: 37,
      email: "tom@example.com",
      address: {
        street: "654 Maple St",
        city: "Boston",
        state: "MA",
        zip: "02101",
      },
      orders: [
        { id: 10, date: "2022-08-01", total: 75.25 },
        { id: 11, date: "2022-08-15", total: 50.0 },
        { id: 12, date: "2022-09-01", total: 30.5 },
      ],
    },
  ];
}
```

## Problem Statement

- What is the name of the customer with the email "jane@example.com"?
