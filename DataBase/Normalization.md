why not Normalization?
A large database defined as a single relation may result in data duplication. This repetition of data may result in:

- Making relations very large.
- It isn't easy to maintain and update data as it would involve searching many records in relation.
- Wastage and poor utilization of disk space and resources.
- The likelihood of errors and inconsistencies increases.

So to handle these problems, we should analyze and decompose the relations with redundant data into smaller, simpler, and well-structured relations that are satisfy desirable properties. Normalization is a process of decomposing the relations into relations with fewer attributes.

## What is Normalization?

- Normalization is the process of organizing the data in the database.
- Normalization is used to minimize the redundancy from a relation or set of relations. It is also used to eliminate undesirable characteristics like Insertion, Update, and Deletion Anomalies.
- Normalization divides the larger table into smaller and links them using relationships.
- The normal form is used to reduce redundancy from the database table.

Why do we need Normalization?

The main reason for normalizing the relations is removing these anomalies. Failure to eliminate anomalies leads to data redundancy and can cause data integrity and other problems as the database grows. Normalization consists of a series of guidelines that helps to guide you in creating a good database structure.

**Data modification anomalies can be categorized into three types:**

- **Insertion Anomaly:** Insertion Anomaly refers to when one cannot insert a new tuple into a relationship due to lack of data.
- **Deletion Anomaly:** The delete anomaly refers to the situation where the deletion of data results in the unintended loss of some other important data.
- **Updating Anomaly:** The update anomaly is when an update of a single data value requires multiple rows of data to be updated.

## Types of Normal Forms:
|Normal Form|Description|
|---|---|
|[1NF](https://www.javatpoint.com/dbms-first-normal-form)|A relation is in 1NF if it contains an atomic value.|
|[2NF](https://www.javatpoint.com/dbms-second-normal-form)|A relation will be in 2NF if it is in 1NF and all non-key attributes are fully functional dependent on the primary key.|
|[3NF](https://www.javatpoint.com/dbms-third-normal-form)|A relation will be in 3NF if it is in 2NF and no transition dependency exists.|
|BCNF|A stronger definition of 3NF is known as Boyce Codd's normal form.|
|[4NF](https://www.javatpoint.com/dbms-forth-normal-form)|A relation will be in 4NF if it is in Boyce Codd's normal form and has no multi-valued dependency.|
|[5NF](https://www.javatpoint.com/dbms-fifth-normal-form)|A relation is in 5NF. If it is in 4NF and does not contain any join dependency, joining should be lossless.|
