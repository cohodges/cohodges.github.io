---
layout: page
title: MongoDB & Map Reduce
---

## MongoDB & Map Reduce

One of the rudiments I completed for CPSC 350 during this semster was practice using Map Reduce to execute processes on large sets of data, stored in MongoDB.

### Map Reduce

Map Reduce is a method for processing large data sets by attempting to distribute subsets of the data with a parallel algorithm. Map Reduce approaches use:

*   A Map() function to filter and sort the data into subsets.

*   A Reduce() function to summarize the subsets.

*   And sometimes, an optional Finalize() function that performs a final procedure on the summarized data.

### MongoDB

MongoDB is a free, open-source NoSQL database program. Processes can be carried out on the data through JSON files.

### Map Reduce vs. SQL

Map Reduce was much faster than an SQL query was at carrying out the same process--one of the jobs took 18 seconds for Map Reduce, and it aalmost took 2 minutes for the SQL query. Map Reduce is a powerful method for processing large batches of data, and it is even more effective when used with a cluster of computers.

#### Just be careful when ending your MongoDB session...

While working on this rudiment, I came across an issue because I didn't properly shut down mongod.

To start MongoDB, you simply type the following command into the terminal:

```
mongod
```

But if you don't properly shut down mongod, your database files can potentially become corrupt. When this happened to me, I didn't have any luck with the recovery steps I could find online, so I had to recreate the databases.

To avoid this situation, remember to properly shut down mongod by entering the following commands into the terminal:

```
use admin
db.shutdownServer()
```
