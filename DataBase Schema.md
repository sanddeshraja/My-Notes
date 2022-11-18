  A database schema represents the logical configuration of all or part of relational database

 It can exist in both  as visual representative  as well as integrity constraint 
 These integrity constraint are expressed using DDL, such as SQL

A Database schema can be broadly classified into two categories


- [ ]  Physical Database Schema :  
     - This schema pertains to the actual storage of data and its form of storage like files, indices.. It defines how the data will be stored in the secondary storage.
- [ ]  Logical Database Schema :
     - This schema defines all  the logical constraints that need to be applied on the data stored . It defines tables, views and Integrity Constraints
 - Conceptual  schema : same as logical schema


**TRANSACTION** :  A logical unit of work on a DB.
An action or a series of action that are being performed by a single user or a application program, which reads or updates the contents of a DB.

In a RDBMS stored data in tables related to  one other but But before making the tables. We need to design how to design how to database looks. to be do that we use E R models.
Probably to show to client how to the client that how your DB will look as an architecture of things

Entity : Real object representation

Entity set : A set of  all entities together 

Attributes : Properties or behaviours of the entity

# TYPES OF ATTRIBUTES

- Key Attribute - uniquely indentify an attribute
-  Composite  attribute - muultiple units together entity
- derived  attribute - that can be calculated from another attribute
- multi valued attribute - more than one value 

![[DataBase Schema 2022-10-16 20.53.40.excalidraw]]