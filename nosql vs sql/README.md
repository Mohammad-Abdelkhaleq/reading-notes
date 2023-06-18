# nosql vs sql

1- What type of database is the best fit for the complex query intensive environment?

SQL databases are good fit for the complex query

2-What type of database is the best fit for hierarchical data storage?

NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data

3-Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

For scalability: In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

<hr>

# sql modeling techniques

1-Among data tables, what is a one-to-many relationship and how do we “relate” them?

an entry in one table can be related to more than one entry in another.

2-Prior to designing your relational database, it might be useful to ___ draw in UML ___ of the database tables and their relationships.

3-Explain the difference between a primary and foreign key.

A primary key is a unique identifier for each record in a table, ensuring data integrity. A foreign key is a column that references the primary key of another table, establishing a relationship between the two tables.

<hr>

1-How do we treat keywords and parameters differently in SQL syntax?

Keywords in SQL are reserved words that have predefined meanings and functions within the language. They are used to specify actions, conditions, or clauses in SQL statements. Examples of keywords include SELECT, INSERT, UPDATE, DELETE, FROM, WHERE, and ORDER BY.

Parameters in SQL are placeholders or bind variables used to represent values that are passed into a SQL statement at runtime. They provide flexibility and reusability to the statement by allowing different values to be substituted without modifying the structure of the statement. Parameters are typically written with a prefix like a colon (:) or a question mark (?), followed by a name or position identifier. They are commonly used with prepared statements or parameterized queries.


2-Define normalization within the context of schemas and data.


Normalization is the process of organizing data in a database to eliminate redundancy and improve data integrity. It involves dividing large tables into smaller ones and establishing relationships between them. The goal is to minimize data duplication and ensure consistency. Normalization is achieved through a series of normal forms, such as 1NF, 2NF, and 3NF, which provide guidelines for structuring data effectively.

3-Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

the diffrence is in the ER relation between tables (connecrted columns)



















