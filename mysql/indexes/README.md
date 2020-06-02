# Indexes & Constraints

When you insert a row into a tale, the server simply places the data in the next available location within the file. When you query a table, therefore, the server will need to inspect every row of the table to answer the query. This type of access is known as a __table scan__.

An _index_ is simply a mechanism for finding a specific item within a resource. Indexes are special tables that unlike normal data tables, _are_ kept in a specific order. Instead of containing _all_ of the data about an entity, however, an index contains only the column/s used to locate rows in the data table, along with information describing where the rows are physically located. Therefore, the role of indexes is to __facilitate the retrieval of a subset of a table's rows and columns without the need to inspect every row in the table__.

## Index Creation

