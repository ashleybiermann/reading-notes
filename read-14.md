## Read: 14a - DB Normalization
[Database Normalization Explained in Simple English](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)
- **Database normalization** process used to organize a database into tables and columns
- limit a table to one purpose
- But Why?...
  1. minimize duplicate data
  2. minimize or avoid data modification issues
  3. simplify queries
- Modification Anomalies
  - Insert anomaly - can't enter part of the data because the key is still unknown
  - Update anomaly - need to update many rows to change one piece of duplicated data
  - Deletion anomaly - important info was tied to a outdate, and deleted, row
- Search and Sort Issues
  - difficult ot compare data across many columns, easier to do this with more tables
