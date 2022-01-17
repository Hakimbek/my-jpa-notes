# JPA Introduction
The Java Persistence API (JPA) is a specification of Java. It is used to persist data between Java object and relational database. JPA acts as a bridge between object-oriented domain models and relational database systems.

As JPA is just a specification, it doesn't perform any operation by itself. It requires an implementation. So, ORM tools like Hibernate, TopLink and iBatis implements JPA specifications for data persistence.

# JPA Object Relational Mapping
Object Relational Mapping (ORM) is a functionality which is used to develop and maintain a relationship between an object and relational database by mapping an object state to database column. It is capable to handle various database operations easily such as inserting, updating, deleting etc.

## ORM Frameworks
- Hibernate
- TopLink
- ORMLite
- iBATIS
- JPOX

## Mapping Directions
### Unidirectional relationship 
In this relationship, only one entity can refer the properties to another. It contains only one owing side that specifies how an update can be made in the database.

### Bidirectional relationship
This relationship contains an owning side as well as an inverse side. So here every entity has a relationship field or refer the property to other entity.

## Types of Mapping

### One-to-one
This association is represented by **@OneToOne** annotation. Here, instance of each entity is related to a single instance of another entity.

### One-to-many
This association is represented by **@OneToMany** annotation. In this relationship, an instance of one entity can be related to more than one instance of another entity.

### Many-to-one 
This mapping is defined by **@ManyToOne** annotation. In this relationship, multiple instances of an entity can be related to single instance of another entity.

### Many-to-many 
This association is represented by **@ManyToMany** annotation. Here, multiple instances of an entity can be related to multiple instances of another entity. In this mapping, any side can be the owing side.

