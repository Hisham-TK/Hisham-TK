# T-Shirts batches
### Description: 

A garment manufacturer produces T-shirts of different sizes and colors grouped by batches.
Implement a system that keeps track of the produced batches.

#### Batch attributes:

Each batch has a group of T-shirts of the same color and size.
Different batches can have different sizes and colors.

#### A batch has:

- Number ( Unique Number greater than zero) 
- Size ( string  [“S” , “M” , “L” , “XL”])
- Color (String [“red” , “blue” , “black” ,”green”])
- Quantity (Number greater than zero represents the number of T-shirts in the batch)
- A batch must have the previously mentioned attributes

### Requirements: 

Given that the views of the system are already implemented (no need for the front-end implementation).

### You are required to:

- Design and implement a database schema for the batch model only. 
- No need to implement a database model for the sizes or the colors. 
- Size can only be one of the following options  [“S” , “M” , “L” , “XL”]
- Color can only be one of the following options  [“red” , “blue” , “black” ,”green”]
- Implement two API endpoints for the basic create and read functionalities for the batch.
- A user can add a batch.
- A user can list all the batches he has produced so far showing each batch’s attributes.


### Bonus tasks (completely optional!)

- Assume that the system got really big and has more than 100 million batch records in the database.
- Discuss an optimized and efficient solution for how it could be implemented if the user wants to know the total number of T-shirts produced from the same color and size which is the summation of quantities of all the batches with the same color and size.


### Example:
#### The database has the following records:

- Batches:  [ {1, “red”, “S” , 50 }  ,{2, “red” , “S” ,100 } , {3 ,”red” ,”M” , 100} ] 

#### If the user asked for the total produced T-shirts of:

- Color “red” and size “S”, the answer should be 150
- Color “red” and size “M”, the answer should be 100
- Color “blue” and size “S”, the answer should be zero
