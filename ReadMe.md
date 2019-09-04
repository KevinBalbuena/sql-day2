#SQL day 2 (aka sqewl, aka skl)

- Student can add foreign key to new table
- Student can add foreign key to existing table
- Student can use join
- Student can use sub-selects/nested queries
- Student can set null values
- Student can Group by
- Student can update rows
- Student can delete rows
- Student can use distinct
- Student can describe one-to-one relationships
- Student can describe one-to-many relationships
- Student can describe many-to-many relationships

* 1st normal form:

- data in each colum is indivisable

- recommened

- string
- number
- boolean
- null
- float

- not recommened

  - object
  - arrays

* 2nd normal form:

- first normalform
- all non key colums are dependant on the tables primary key

* 3rd normal form

- second form
- contains only colums that are non transitively-dependant on a primary key

transitive: A is greater then B, and B is greater then C this it would
make sense that A if greater then C

A, B, PK if the value if A relies to the PK, anf B relies on the
PK and a A also relies on B then you can
stay A relies on PK through B

```sql
personID, firstName, lastName => non transitively dependant

personID, bodyMassIndex, isObese => transitvely dependant
```

**one to one relationship**

- one colum in a table is associated with one and only one column
  from another table

<img width='500px' src='https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/CPT-Databases-OnetoOne.svg/500px-CPT-Databases-OnetoOne.svg.png'>

**one to many relationships**

- on column is a table can be associated with on or more colums in another table

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d7/CPT-Databases-OnetoMany2.svg/500px-CPT-Databases-OnetoMany2.svg.png">

**many to many relationships**

- multiple columns is a table can be associated with mutiple colums from another table

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/CPT-Databases-ManytoMany.svg/500px-CPT-Databases-ManytoMany.svg.png">

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/0/02/Databases-ManyToManyWJunction.jpg">
