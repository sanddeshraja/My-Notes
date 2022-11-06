1. DB - Collection of related data in a organized and systematic way

  DBMS?
 -  Uses Real-world entity : DBMS  uses it to design it's architecture
 - Normalization :  Relation based DB  uses this to reduce redundancy
 - Highly Consistent with Constraints
 - DBMS has Query Language to retrieve & manipulate data
  
  
  *Data Definition* : It is used for creation , modification and removal of definition that defines the organiztion of data in the database.
  
  *Data Updation* : It is used for insertion, modification and deletion of actual data in database.

  *Data Retrieval* : It is used to retrieve the data from the database which can be used by applications for various purposes

 *User Administration* : Giving access to the user to administrate the <abbr title="Database">DB</abbr>  more efficiently with Limits.

  ACID Properties
  
  **ATOMICITY** :  The entire transaction takes place at once or doesnt happen at all.
  
 **CONSISTENCY** : Correctness, Integrity constraints must be maintained.
  
 **ISOLATION**  :  
     - Multiple Transaction  -  Concurrently without leading to the inconsistency of  database state .
     - Responsibility of concurrency  control subsystem.
     - Changes occuring  in 1 trans. will not be visible to other transaction until committed.

**DURABILTY** : If a transaction gets committed , the data updation and modification to the DB must be done and stord irrespective of a system failure { The effects of the transaction are never lost.}


*Data Model* : It decides the method of storing data in the database

[[Types of Data Model]]


 Database can be classified into
 
 | Decentralized Database        | Centralized Database    |
 | ----------------------------- | ----------------------- |
 | Data Redundancy               | fast way of processing  |
 | inconsistency in data is high | single computing device |
 | Many small database           | 1 big database          | 


[[EVOLUTION of DBMS]]

[[DBMS  Architecture]]

[[DataBase Schema]]

## RELATIONSHIP IN DBMS

1. Diamond box -> Relation
2. various types of relation -> Unary, Binary, n-nary

### UNARY
- relationship is where there is only entity which is related to itself
- Ex : An entity person is related to itself, relationship married to
-
```math
||{"id":1188838866078}||


```

### BINARY
- 2 different entities assosciated with each other
```math
||{"id":378526210433}||


```
**Participation constraint**
 - Total Participation
            - It specifies that each entity in the entity set must compulsorily participate in at least one relationship instance
            - Also called mandatory participation
	            - Total participation is represented using double line between entity set and relationship set.

```math
||{"id":912677113012}||


```

Partial Participation

A single line between the entities i.e courses and enrolled in a relationship signifies the partial participation, which means there might be some courses where enrollments are not made


![[DBMS 2022-10-18 00.57.59.excalidraw]]

##### Strong Entity
A strong entity is not dependent of any other entity in the schema. A strong entity always will have a primary key. Strong entity - single rectangle
Strong entities together make strong entity set.

##### Weak Entity
A weak entity is dependent on strong entity  to ensure its existence. Unlike a strong entity, a weak entity does not have any primary key.
It instead has a partial discriminator key. A weak entity is represented by a double rectangle.

		![[DBMS 2022-10-18 01.09.01.excalidraw]]

#### Generalization

-  combine  low specific level entities to one high level generalized  entity
-  It's a bottom up approach
-  Ex :  two specific entities such as teacher and student can be made into one generalized  person entity

#### Specialization
-  Its a top down approach
- divide one generalized entity into more than one specific entities
- Ex : a employee entity in a company can be divided into two specific entities - currently working for the company and ex-employee.

#### Aggregation
- Considering two entities in one
- university offering courses can be considered as one entity from student perspective.


## E.F Codd Rules

- Rules for defining RDBMS
Rule 0 -12
0. The foundation Rule :  For any system that is advertised as, or claimed to be, a relational database management system, that system must be able to management system,  that system must be able to manage databases entirely through its relational capabilities.
1. Information Rule :  All the data including meta data must be stored in some cell of the table in the form of rows and columns

2. Guaranteed Access Rule : Every single data element(value)
can be accessed logically with a combination of table-name, primary-key(Row value ) and attribute-name(column value)

3. Systematic treatment of Null value : The Null values in a database must be given  a '' and unifrom treatment. this is very important rule a null can be interpreted as one of the following, data is missing, data is not known or data is not applicable.

4. Active Online Catalog : The structure description of the entire database must be stored in an online catlog. known as data dictionary. which can be accessed by authorized users. Users can Use the same query language to access the catalog which they use to access the database itself

5. Powerful and well structured language : The database should be accessible through a language which supports data definition, data manipulation and transaction management operations. All commercial relational databases , use forms of SQL as their supported language.

 6. View Updating Rule : Data can be presented in different logical combinations called Views. Each View should support the same full range of data manipulation that has direct access to a table available 

  7. High  Level Insert, Update and Delete :  A database must support high level insertion, updation, and Deletion. This must must  not be limited in a single row, that is . It must also support umion, intersection and minus operations to yiels sets of data records.
  
  8. Physical Data Independence : The data stored in a database must be independent of the applications that access the database . Any change in the physical structure of a databse must not have any  impact on how the database must not have any impact on how the data is being accessed by external applications. 

  9. Logical Data Independence : The logical Data in a database must be independent of its user's view ( Application). Any Change in Logical Data must not affect the application using it.

10. Integrity Independence : The database Language (Like SQL) should support constraints on users input that maintain database integrity.
     No Component of a primary key can have a null value.
     If a foreign key is defined in one table, any value in it must exist as a primary key in another table.

11.  Distribution Independence : the end user must not be able to see that the data is distributed over various locations users should always get the impression that the data is located at one site only.{ foundation of distributed database system.} 


12. Non Subversion Rule : There should be no way to modify the database structure other than through the multiple row database language (SQL) most databases today support administrative tools that allows some direct Manipulation of the data structure.


Why keys?
- uniquely identify any record or row of data in a table.
- It is also used to establish and identify relationships between tables

Candidate key : The minimal set of attribute which can uniquely indentify a tuple is known as candidate key
more than one candidate key.
Unique and not-null for every tuple.
can have one or more attribute as a candidate key
Ex : UserName, UserID 

Super Key : The set of attribute which can uniquely identify a tuple is known as Super key. if we ass zero or more attributes to candidates key generates super key.

Primary key : While there can be more than one candidate keys in the table to uniquely identify.
Primary key is a uniquely and non-null key which identify a record uniquely in table. A table can have only one primary key.
Primary keys may be composite


Alternate Key : All other candidates keys apart  from the primary key are called as alternate keys. For Example Phone Number will become alternate key here.

Composite key : Two or more attributes together form a composite key that can uniquely identify a tuple in a table.

Foreign Key : A Foreign key is a column or a combination of columns whose values match a Primary Key in a different table.

## Normalization in DBMS

Normalization rules divides larger tables into smaller tables(decomposing tables) and link them using relationship
Purpose of Normalization in SQL is to eliminate redundant(repetitive) data and ensure data is tored logically.

Normalization is used also to solve anomaly like

a) Insertion Anomaly 
b) Updation Anomaly
C) Deletion Anomaly


1 NF -> Normal Form
2 NF
3 NF
BCNF -> Boyce-Codd Normal Form
4 NF
5 NF
6 NF

1 NF
A relation in 1 NF contains an atomic value
It states that attribute cannot hold  multiple value
A record must be unique.

2 NF
1. It should be in 1 NF
2. It should have no partial dependency, i.e(non prime attribute(not part of candidate key ) is not dependent on a proper subset of candidate key)

3 NF
1. follow 1 NF and 2 NF
2. In Non Trivial function dependency(i.e, LHS should not have any of the RHS Part a->ae)
3. after 2 is done, if X->Y
4. then X should be super key ( atleast 1 out of 4 and 5)
5. and Y should be a prime attribute

BCNF
1. for every functional dependency X->Y     ,  X must be super key
