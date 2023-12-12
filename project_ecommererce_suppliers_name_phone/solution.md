### Queries

1.

```json
db.suppliers.aggregate([
  {$project:{name:1,phone:1,_id:0}}
  ])
```

--> result

```json
[
  {
    "name": "Samsung",
    "phone": "82-2-2255-0114"
  }
]
```
