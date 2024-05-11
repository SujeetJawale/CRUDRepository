### Overview

This project is a demonstration of using Spring Data JPA for effective data management in Java applications. Spring Data JPA simplifies the implementation of data access layers by reducing the amount of boilerplate code required. In this project, I have specifically explored the capabilities of the CrudRepository interface, which provides sophisticated CRUD (Create, Read, Update, Delete) functionality out-of-the-box.

### Features

The key feature of this project is the utilization of the CrudRepository interface from Spring Data JPA. Here is an overview of the methods explored and their purposes:

##### save(S entity): 
Saves a given entity. Use this method when you want to create a new entry or update an existing entry in the database.
##### findById(ID id): 
Retrieves an entity by its id. This is particularly useful for fetching details of a specific entry.
##### existsById(ID id): 
Checks whether an entity with the given id exists in the database.
##### findAll(): 
Returns all instances of the type.
##### findAllById(Iterable<ID> ids): 
Returns all instances identified by the given ids.
##### count(): 
Returns the number of entities available.
##### deleteById(ID id): 
Deletes the entity with the specified id.
##### delete(S entity): 
Deletes a given entity.
##### deleteAll(Iterable<? extends S> entities):
Deletes all the entities identified by the given iterable.
##### deleteAll(): 
Deletes all entities managed by the repository.
##### saveAll(Iterable <> entities): 
Saves all given entities, which is particularly useful for batching multiple saves in a single operation.

Further will explore the other interface which is JpaRepository a combination of CrudRepository and PagingAndSortingRepositiory.
