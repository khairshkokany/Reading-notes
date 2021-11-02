# Saving data with Room

![images](https://miro.medium.com/max/659/1*SssXYHFuffP4DlamiClmZA.png)
## Room provides the following benefits:
- Compile-time verification of SQL queries.
- Convenience annotations that minimize repetitive and error-prone boilerplate code.
- Streamlined database migration paths.

## There are three major components in Room:
- The database class that holds the database and serves as the main access point for the underlying connection to your app's persisted data.
- Data entities that represent tables in your app's database.
- Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.

### The database class provides your app with instances of the DAOs associated with that database. In turn, the app can use the DAOs to retrieve data from the database as instances of the associated data entity objects.

### AppDatabase defines the database configuration and serves as the app's main access point to the persisted data.
## The database class must satisfy the following conditions:

- The class must be annotated with a @Database annotation that includes an entities array that lists all of the data entities associated with the database.
- The class must be an abstract class that extends RoomDatabase.
- For each DAO class that is associated with the database, the database class must define an abstract method that has zero arguments and returns an instance of the DAO class.

## Primary components
There are three major components in Room:

1. Database Class 
2. Data Entities
3. Data Access Object

The image bellow illistrate the relation between room components:

![image](https://miro.medium.com/max/2000/1*33hzCoxAoUehHrHeBJi-VA.png)

# Defining data using Room entities

- Each entity corresponds to a table in the associated Room database, and each instance of an entity represents a row of data in the corresponding table.

- you can use Room entities to define your database schema.

- A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

- Room uses the field names as column names in the database by default. If you want a column to have a different name, add the @ColumnInfo annotation to the field and set the name property. 

- Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.

- you can use the @Embedded annotation to represent an object that you'd like to decompose into its subfields within a table. 