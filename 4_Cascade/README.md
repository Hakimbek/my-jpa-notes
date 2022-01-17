# JPA Cascading Operations
In JPA, if any operation is applied on an entity then it will perform on that particular entity only. These operations will not be applicable to the other entities that are related to it.

To establish a dependency between related entities, JPA provides javax.persistence.CascadeType enumerated types that define the cascade operations. These cascading operations can be defined with any type of mapping i.e. One-to-One, One-to-Many, Many-to-One, Many-to-Many.

| Cascade Operations | Description |
| ------------------ | ----------- |
| PERSIST |	In this cascade operation, if the parent entity is persisted then all its related entity will also be persisted. |
| MERGE |	In this cascade operation, if the parent entity is merged then all its related entity will also be merged. |
| DETACH |	In this cascade operation, if the parent entity is detached then all its related entity will also be detached. |
| REFRESH |	In this cascade operation, if the parent entity is refreshed then all its related entity will also be refreshed. |
| REMOVE |	In this cascade operation, if the parent entity is removed then all its related entity will also be removed. |
| ALL |	In this case, all the above cascade operations can be applied to the entities related to parent entity. |
