# Read: Class 4 : Data Modeling

- - -

## Review, Research, and Discussion

* **name 3 advantages to Test Driven Development**

Better program design and higher code quality   
Detailed project documentation   
TDD reduces the time required for project development   
Code flexibility and easier maintenance   
With TDD you will get a reliable solution   
Save project costs in the long run   


* **In what case would you need to use beforeEach() or afterEach() in a test suite?**

**beforeEach** Runs a function before each of the tests in this file runs. If the function returns a promise or is a generator, Jest waits for that promise to resolve before running the test.This is often useful if you want to reset some global state that will be used by many tests.    
 
**afterEach** Runs a function after each one of the tests in this file completes. If the function returns a promise or is a generator, Jest waits for that promise to resolve before continuing.This is often useful if you want to clean up some temporary state that is created by each test.


* **What is one downside of Test Driven Development**
The test suite itself has to be maintained; tests may not be completely deterministic (i.e. reliant on external dependencies).
The tests may be hard to write, esp. beyond the unit testing level.

* **What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

In simple words class is a blueprint for creating an object and constructor is special kind of a method that creates objects.


* **Why REST?**

REST APIs is that they provide a great deal of flexibility. Data is not tied to resources or methods, so REST can handle multiple types of calls, return different data formats and even change structurally with the correct implementation of hypermedia.

- - -

#### Document the following Vocabulary Terms

* **functional programming** In computer science, functional programming is a programming paradigm where programs are constructed by applying and composing functions

* **object-oriented programming (OOP)** Object-oriented programming is a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields, and code, in the form of procedures. A feature of objects is that an object's own procedures can access and often modify the data fields of itself    

* **class** In object-oriented programming, a class is an extensible program-code-template for creating objects, providing initial values for state (member variables) and implementations of behavior (member functions or methods)

* **super** super() will calls the constructor of its parent class. This is required when you need to access some variables from the parent class. In React, when you call super with props. React will make props available across the component through this.props .

* **this** keyword that represents the current instance of the class in which it appears. It is used to access class variables and methods

* **Test Driven Development (TDD)** “Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).

* **Jest**  an open source project maintained by Facebook, and it's especially well suited for React code testing, although not limited to that: it can test any JavaScript code

* **Continuous Integration (CI)** Continuous integration (CI) is a software engineering practice where members of a team integrate their work with increasing frequency. ... Continuous delivery (CD) is to packaging and deployment what CI is to build and test.

* **REST** Representational state transfer is a software architectural style that was created to guide the design and development of the architecture for the World Wide Web. REST defines a set of constraints for how the architecture of an Internet-scale distributed hypermedia system, such as the Web, should behave

* **Data Model** A data model (or datamodel) is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. ... So the "data model" of a banking application may be defined using the entity-relationship "data model".

- - - 

## Article : sql vs nosql 

| SQL                                 | NoSQL                                           |
| --------------                      |----------------------------------------         |
| Relational Databases (RDBMS)        | distributed database.                           |
| table based databases               | document based                                  |
| predefined schema                   | dynamic schema                                  |
| vertically scalable                 | horizontally scalable                           |
| uses SQL                            | queries are focused on collection of documents. |
| either open-source or close-sourced | graph databases, key-value store databases      |
|Excellent support are available      | you still have to rely on community support     |
### SQL Database Examples

* MySQL Community Edition
* MS-SQL Server Express Edition 
* Oracle Express Edition

### NoSQL Database Examples

* MongoDB
* CouchDB
* Redis

--- 

## Article : nosql modeling techniques

**NoSQL** databases are often compared by various non-functional criteria, such as scalability, performance, and consistency.    

**SQL** and relational model in general were designed long time ago to interact with the end user. This user-oriented nature had vast implications:
- The end user is often interested in aggregated reporting information, not in separate data items, and SQL pays a lot of attention to this aspect.
- No one can expect human users to explicitly control concurrency, integrity, consistency, or data type validity. That’s why SQL pays a lot of attention to transactional guaranties, schemas, and referential integrity

And this was where a new evolution of data models began:

- Key-Value storage is a very simplistic, but very powerful model. Many techniques that are described below are perfectly applicable to this model.

- Ordered Key-Value model is very powerful, but it does not provide any framework for value modeling.
- Document databases advance the BigTable model offering two significant improvements. 
- Graph data models can be considered as a side branch of evolution that origins from the Ordered Key-Value models. Graph databases allow one model business entities very transparently (this depends on that), but hierarchical modeling techniques make other data models very competitive in this area too. 

### Conceptual Techniques

* Denormalization 

* Aggregates

* Application Side Joins

* Atomic Aggregates

* Enumerable Keys

* Dimensionality Reduction

* Index Table

* Composite Key Index

* Aggregation with Composite Keys

* Inverted Search – Direct Aggregation

* Tree Aggregation

* Adjacency Lists

* Materialized Paths

* Nested Sets

* Batch Graph Processing

- - - 
