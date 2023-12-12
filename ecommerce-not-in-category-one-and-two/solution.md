### Queries

1. db.products.find({category_id: {$nin: [1, 2]}})

- Result -

```
[
  {
  _id: 8,
  name: 'Bose QuietComfort 35',
  category_id: 3,
  price: 249.99,
  quantity: 50,
  supplier_id: 7
},
 {
  _id: 7,
  name: 'Beats Studio Buds',
  category_id: 3,
  price: 149.99,
  quantity: 50,
  supplier_id: 6
}
]
```
