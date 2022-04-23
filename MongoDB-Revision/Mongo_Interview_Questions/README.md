# # Mongo Interview Questions . 👋

### 1. What is SQL Databases? What are some companies who uses Mongo, what type of applications are these ?
```bash
SQL => SQL is Structured Query Language, which is a computer language for storing, manipulating and retrieving data which is stored in a relational database .
=> Forbes, Facebook, Google, Twitter, IBM, Zendesk, gazillion are some companies who uses Mongo .
=> mongoDb uses a JSON-like format to store documents .

mongoDB => MongoDB is an open-source document-oriented database that is designed to store a large scale of data and also allows you to work with that data very efficiently. It is categorized under the NoSQL (Not only SQL) database because the storage and retrieval of data in the MongoDB are not in the form of tables
```
### 2.What is NoSQL Databases ?
```bash
=> When people use the term “NoSQL database,” they typically use it to refer to any non-relational database. Some say the term “NoSQL” stands for “non SQL” while others say it stands for “not only SQL.” Either way, most agree that NoSQL databases are databases that store data in a format other than relational tables.

=> Over time, four major types of NoSQL databases emerged:-

    1. document databases
    2. key-value databases
    3. wide-column stores
    4. graph databases
```
### 3. What is the difference between SQL and NoSQL databases ?
```bash

SQL =>

1. RELATIONAL DATABASE MANAGEMENT SYSTEM (RDBMS)
2. These databases have fixed or static or predefined schema
3. These databases are not suited for hierarchical data storage.
4. These databases are best suited for complex queries
5. Vertically Scalable
6. Follows ACID property
7. In terms of performance, it is much faster than RDBMS.

NoSQL =>

1. Non-relational or distributed database system.
2. These databases are best suited for hierarchical data storage.
3. These databases are not so good for complex queries
4. Horizontally scalable
5. Follows CAP(consistency, availability, partition tolerance)
6. In terms of performance, it is slower than MongoDB.

The Main Differences: -

1. Type – 
=> SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database. 

2. Language – 
SQL databases defines and manipulates data based structured query language (SQL). Seeing from a side this language is extremely powerful. SQL is one of the most versatile and widely-used options available which makes it a safe choice especially for great complex queries. But from other side it can be restrictive. SQL requires you to use predefined schemas to determine the structure of your data before you work with it. Also all of your data must follow the same structure. This can require significant up-front preparation which means that a change in the structure would be both difficult and disruptive to your whole system. 
A NoSQL database has dynamic schema for unstructured data. Data is stored in many ways which means it can be document-oriented, column-oriented, graph-based or organized as a KeyValue store. This flexibility means that documents can be created without having defined structure first. Also each document can have its own unique structure. The syntax varies from database to database, and you can add fields as you go. 

3. The Scalability – 
In almost all situations SQL databases are vertically scalable. This means that you can increase the load on a single server by increasing things like RAM, CPU or SSD. But on the other hand NoSQL databases are horizontally scalable. This means that you handle more traffic by sharding, or adding more servers in your NoSQL database. It is similar to adding more floors to the same building versus adding more buildings to the neighborhood. Thus NoSQL can ultimately become larger and more powerful, making these databases the preferred choice for large or ever-changing data sets. 

4. The Structure – 
SQL databases are table-based on the other hand NoSQL databases are either key-value pairs, document-based, graph databases or wide-column stores. This makes relational SQL databases a better option for applications that require multi-row transactions such as an accounting system or for legacy systems that were built for a relational structure. 

5. Property followed – 
SQL databases follow ACID properties (Atomicity, Consistency, Isolation and Durability) whereas the NoSQL database follows the Brewers CAP theorem (Consistency, Availability and Partition tolerance). 
```
### 4. What are some features of MongoDB ?
```bash

Now a day many companies using MongoDB to create new types of applications, improve performance and availability.

1. Support ad hoc queries
    => In MongoDB, you can search by field, range query and it also supports regular expression searches.

2. Indexing
    =>You can index any field in a document.

3. Replication
    => MongoDB supports Master Slave replication.
    A master can perform Reads and Writes and a Slave copies data from the master and can only be used for reads or back up (not writes)

4. Duplication of data
    => MongoDB can run over multiple servers. The data is duplicated to keep the system up and also keep its running condition in case of hardware failure.

5. Load balancing
    => It has an automatic load balancing configuration because of data placed in shards.


Schema-less Database:- It is the great feature provided by the MongoDB. A Schema-less database means one collection can hold different types of documents in it. Or in other words, in the MongoDB database, a single collection can hold multiple documents and these documents may consist of the different numbers of fields, content, and size. It is not necessary that the one document is similar to another document like in the relational databases. Due to this cool feature, MongoDB provides great flexibility to databases.

Document Oriented:- In MongoDB, all the data stored in the documents instead of tables like in RDBMS. In these documents, the data is stored in fields(key-value pair) instead of rows and columns which make the data much more flexible in comparison to RDBMS. And each document contains its unique object id.

Indexing:- In MongoDB database, every field in the documents is indexed with primary and secondary indices this makes easier and takes less time to get or search data from the pool of the data. If the data is not indexed, then database search each document with the specified query which takes lots of time and not so efficient.

Scalability:- MongoDB provides horizontal scalability with the help of sharding. Sharding means to distribute data on multiple servers, here a large amount of data is partitioned into data chunks using the shard key, and these data chunks are evenly distributed across shards that reside across many physical servers. It will also add new machines to a running database.
Replication: MongoDB provides high availability and redundancy with the help of replication, it creates multiple copies of the data and sends these copies to a different server so that if one server fails, then the data is retrieved from another server.

Aggregation:- It allows to perform operations on the grouped data and get a single result or computed result. It is similar to the SQL GROUPBY clause. It provides three different aggregations i.e, aggregation pipeline, map-reduce function, and single-purpose aggregation methods
High Performance: The performance of MongoDB is very high and data persistence as compared to another database due to its features like scalability, indexing, replication, etc.
```
### 5. What are aggregate queries ?
```bash
=> An aggregate query is a method of deriving group and subgroup data by analysis of a set of individual data entries.  The term is frequently used by database developers and database administrators.
```
### 6. What are pipelines in aggregation ?
```bash
=> An aggregation pipeline consists of one or more stages that process documents:-

* Each stage performs an operation on the input documents. For example, a stage can filter documents, group documents, and calculate values.
* The documents that are output from a stage are passed to the next stage.
```
### 7. How do you do aggregate queries ?
```bash
 ...answer
```
### 8. How can you group by a particular value in MongoDB ?
```bash
 ...answer
```
### 9. How can you paginate on MongoDB ?
```bash
 1) MongoDB pagination by using limit method
    => db.collection_name.find () .limit (number);

2) MongoDB pagination by using skip method
    => db.collection_name.find () .skip (number);
```
### 10. How can you sort in MongoDB ?
```bash
=> 1 Sort ascending.
=> -1 Sort descending.

{ $sort: { <field1>: <sort order>, <field2>: <sort order> ... } }
If sorting on multiple fields, sort order is evaluated from left to right. For example, in the form above, documents are first sorted by <field1>. Then documents with the same <field1> values are further sorted by <field2>.

Limits => You can sort on a maximum of 32 keys.

db.users.aggregate(
   [
     { $sort : { age : -1, posts: 1 } }
   ]
)
=> This operation sorts the documents in the users collection, in descending order according by the age field and then in ascending order according to the value in the posts field.
```
### 11. What is indexing in MongoDB? Why do we need to use indexing? What are pros and cons for indexing ?
```bash
=> The biggest advantage:- of indexing is that it speeds up your find, update and delete queries. Quite naturally because it is easier to search for the elements based on the indexed field.
=> The disadvantages:- of indexing is that 1. It takes up memory (obviously). 2.It slows down write queries.

First of all there are three different kinds of indexes that you should probably know of :-

1.Single index -> Where you sort a collection based on just a single field value.

2.Compound index -> Where you sort a collection first based on a single value and then for the values that have the same first value, you sort the list according to a second field value that you have provided.

3.Partial index -> When you sort the collection based on a field value but only in a particular range (we’ll see how later).
```
### 12. Write the query for indexing a field in MongoDB ?
```bash
db.collection.createIndex()
```
### 13. What is the improvement in performance in MongoDB ?
```bash
 ...answer
```
### 14. What is the data structure used for indexing ?
```bash
B-trees are the most commonly used data structures for indexes as they are time-efficient for lookups, deletions, and insertions. All these operations can be done in logarithmic time. Data that is stored inside of a B-tree can be sorted. Indexes that use hash tables are generally referred to as hash index.
```
### 15. Are values sorted in indexes ?
```bash
When an index has a key with multiple data types, the index is sorted according to the BSON type sort order. If an index key contains an array, the document is sorted according to the type of the first array element.
```
### 16. What are Replica Sets in MongoDB ?
```bash
A replica set in MongoDB is a group of mongod processes that maintain the same data set.

Replica sets provide redundancy and high availability, and are the basis for all production deployments. This section introduces replication in MongoDB as well as the components and architecture of replica sets.
```
### 17. Explain the structure of ObjectID in MongoDB ?
```bash
 ...answer
```
### 18. By default, which index is created by MongoDB for every collection ?
```bash
 ...answer
```
### 19. In which format MongoDB represents document structure ?
```bash
 ...answer
```
### 20. What is the limitation of a document in MongoDB ?
```bash
 ...answer
```
### 21. What is the difference between MongoDB and Redis database ?
```bash
 ...answer
```
### 22. How can you add references between multiple collections ?
```bash
 ...answer
```
### 23. What are lookup in aggregation for MongoDB ?
```bash
 ...answer
```
### 24. What are graph lookups ?
```bash
 ...answer
```
### 25. What is the alternative for lookups in MongoDB ?
```bash
 ...answer
```
### 26. How can you do one to many relation in MongoDB ?
```bash
 ...answer
```
### 27. How can you do many to many relation in MongoDB ?
```bash
 ...answer
```
### 28. How can you do one to zillion relation in MongoDB ?
```bash
 ...answer
 ```