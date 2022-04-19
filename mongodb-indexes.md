# MongoDB Indexes

## References
1. https://www.mongodb.com/docs/manual/indexes/


## Main Points

* Without index -> **collection scan** on queries. 
* With index -> limit the number of document to inspect.
* MongoDB defines indexes at the collection level and supports indexes on any field or sub-field of the documents in a MongoDB collection.
* MongoDB creates a unique index on the **\_id** field during the creation of a collection.


## Single Field
![image](https://user-images.githubusercontent.com/11683340/163942199-f5b45eac-b61e-4c44-832e-3e4e6422f3ef.png)
* For a single-field index and sort operations, the sort order (i.e. ascending or descending) of the index key does not matter because MongoDB can traverse the index in either direction.


## Compound Index
![image](https://user-images.githubusercontent.com/11683340/163942280-47717f17-d0f4-45e3-bb9d-330e1435ff2a.png)
* For compound indexes and sort operations, the sort order (i.e. ascending or descending) of the index keys can determine whether the index can support a sort operation.
* ESR (Equality, Sort, Range) Rule for creation efficient indexes: https://www.mongodb.com/docs/manual/tutorial/equality-sort-range-rule/#std-label-esr-indexing-rule.

## Multikey Index
![image](https://user-images.githubusercontent.com/11683340/163942400-ab954998-f139-439a-8dd5-3eac69edfa2b.png)

## Other indexes
* Geospatial Index
* Text Indexes
* Hashed Indexes

