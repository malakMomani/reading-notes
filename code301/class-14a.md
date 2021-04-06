## Database Normalization

**What is Database Normalization ?**
> it's processing to organize your DB, your tables, and your columns, trying to make it meaningful, readable, efficient & useful, By separate your tables, make every table present one topic, add correct relations between them and avoid redundant data in your DB

**Reasons of Normalization :**
- minimize duplicate data
- minimize or avoid data modification issues
- simplify queries

**There are three common forms of normalization :**
- First Normal Form : The information is stored in a relational table and each column contains atomic values, and there are not repeating groups of columns.
- Second Normal Form : The table is in first normal form and all the columns depend on the table’s primary key.
- Third Normal Form : The table is in second normal form and all of its columns are not transitively dependent on the primary key.