### Queries

1. db.products.find({ "category": "electronics", "rating.rate": { $gte: 4 }, "rating.count": { $gte: 100 } })

2. db.products.find({$and:[{ "category": "electronics"}, {"rating.rate": { $gte: 4 }}, {"rating.count": { $gte: 100 }}] })

- Result -

```
[
  {
    _id: ObjectId("642e62fea96bc0148062c494"),
    id: 11,
    title: 'Silicon Power 256GB SSD 3D NAND A55 SLC Cache Performance Boost SATA III 2.5',
    price: 109,
    description: '3D NAND flash are applied to deliver high transfer speeds Remarkable transfer speeds that enable faster bootup and improved overall system performance. The advanced SLC Cache Technology allows performance boost and longer lifespan 7mm slim design suitable for Ultrabooks and Ultra-slim notebooks. Supports TRIM command, Garbage Collection technology, RAID, and ECC (Error Checking & Correction) to provide the optimized performance and enhanced reliability.',
    category: 'electronics',
    image: 'https://fakestoreapi.com/img/71kWymZ+c+L._AC_SX679_.jpg',
    rating: { rate: 4.8, count: 319 }
  },
  {
    _id: ObjectId("642e62fea96bc0148062c495"),
    id: 12,
    title: 'WD 4TB Gaming Drive Works with Playstation 4 Portable External Hard Drive',
    price: 114,
    description: "Expand your PS4 gaming experience, Play anywhere Fast and easy, setup Sleek design with high capacity, 3-year manufacturer's limited warranty",
    category: 'electronics',
    image: 'https://fakestoreapi.com/img/61mtL65D4cL._AC_SX679_.jpg',
    rating: { rate: 4.8, count: 400 }
  }
]
```
