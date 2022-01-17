# JPA One-To-One Mapping
The One-To-One mapping represents a single-valued association where an instance of one entity is associated with an instance of another entity. In this type of association one instance of source entity can be mapped atmost one instance of target entity.

### @OneToOne Example
In this example, we will create a One-To-One relationship between a Student and Library in such a way that one student can be issued only one type of book.

# JPA One-To-Many Mapping
The One-To-Many mapping comes into the category of collection-valued association where an entity is associated with a collection of other entities. Hence, in this type of association the instance of one entity can be mapped with any number of instances of another entity.

### @OneToMany Example
In this example, we will create a One-To-Many relationship between a Student and Library in such a way that one student can be issued more than one type of book.

# JPA Many-To-One Mapping
The Many-To-One mapping represents a single-valued association where a collection of entities can be associated with the similar entity. Hence, in relational database any more than one row of an entity can refer to the similar rows of another entity.

### @ManyToOne Example
In this example, we will create a Many-To-One relationship between a Student and Library in such a way that more than one student can issued the same book.

# JPA Many-To-Many Mapping
The Many-To-Many mapping represents a collection-valued association where any number of entities can be associated with a collection of other entities. In relational database any number of rows of one entity can be referred to any number of rows of another entity.

### @ManyToMany Example
In this example, we will create a Many-To-Many relationship between a Student and Library in such a way that any number of students can be issued any type of books.
