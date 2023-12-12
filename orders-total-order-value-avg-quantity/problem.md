### Problem Description

## Given below pizza-orders json data to perform mongo queries.

```
"inventory:[
   {
      "_id" : 1,
      "item" : "ABC1",
      sizes: [ "S", "M", "L"]
   }
]
```

## Problem Statement

- write query for aggregation uses the `$unwind` stage to output a document for each element in the sizes array?
