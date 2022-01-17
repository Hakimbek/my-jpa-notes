# JPA Entity Introduction
In general, entity is a group of states associated together in a single unit. On adding behaviour, an entity behaves as an object and becomes a major constituent of object-oriented paradigm. So, an entity is an application-defined object in Java Persistence Library.

## Entity Properties

### Persistability 
An object is called persistent if it is stored in the database and can be accessed anytime.

### Persistent Identity 
In Java, each entity is unique and represents as an object identity. Similarly, when the object identity is stored in a database then it is represented as persistence identity. This object identity is equivalent to primary key in database.

### Transactionality 
Entity can perform various operations such as create, delete, update. Each operation makes some changes in the database. It ensures that whatever changes made in the database either be succeed or failed atomically.

### Granuality 
Entities should not be primitives, primitive wrappers or built-in objects with single dimensional state.

## Entity Metadata
Each entity is associated with some metadata that represents the information of it. Instead of database, this metadata is exist either inside or outside the class. This metadata can be in following forms: -

### Annotation 
In Java, annotations are the form of tags that represents metadata. This metadata persist inside the class.

### XML
In this form, metadata persist outside the class in XML file.

# JPA Creating an Entity
A Java class can be easily transformed into an entity. For transformation the basic requirements are:

- No-argument Constructor
- Annotation

Here, we will learn how to transform a regular Java class into an entity class with the help of an example:

### Simple Student class

```java
public class Student {  
    private int id;  
    private String name;  
    private long fees;  
    
    // constructors
    // getters and setters
```

Above class is a regular java class having three attributes id, name and fees. To transform this class into an entity add **@Entity** and **@Id** annotation in it.

### @Entity
This is a marker annotation which indicates that this class is an entity. This annotation must be placed on the class name.

### @Id 
This annotation is placed on a specific field that holds the persistent identifying properties. This field is treated as a primary key in database.

```java
@Entity
public class Student {  
    @Id
    @GeneratedValue(strategy=GenerationType.AUTO) 
    private int id;  
    private String name;  
    private long fees;  
    
    // constructors
    // getters and setters
```
