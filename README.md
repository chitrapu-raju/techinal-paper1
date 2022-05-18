# Data types and Data Structures

## Introduction to Data types :
Java is statically type language where each variable and expression type we must know before hand so we must have an idea on the data types we are gonna use.  
We have two types of data types present in java  
- Primitive Data types 
- Non-Primitive Data types

Primitive data types are the most most basic and only store single values. there are 8 types of primitive data types  
- boolean  
- byte
- short  
- char
- int
- long
- float
- double  

Type casting comes in picture when we try to assign primitive data type to another datatype , there are two types of casting  

### Widening casting :
 - in this case we don't need to do anything , computer implicitly convert smaller type to larger type size.

### Narrowing casting :  
 - in this case we manually convert a larger type to smaller type size.  

 ![example image](./type%20casting.png)

Non-primitive data types are such as Strings,Arrays,classes,interfaces ... etc

## Introduction to Data Structures :
Data structures provides  an efficient way of storing and organising the data.These are widely used in almost every aspect of Computer Science. They play a vital role in improve the performance of a software or program and selecting the appropriate data structure is one of the most important task for a programmer. Once we implement any data structure we can use it anywhere we want.  

We have 2 types of data structures Linear and Non- Linear Data Structures.  

### Overview on Linear Data Structures :  
 
Some of the popular linear data structures are  
 - Array  
 - LinkedList
 - Stack
 - Queue

### 1. Array : 
 Array is the collection of homogenous data type elements and fixed in size, elements are stored at contigous locations one after the other. we can create an  one dimentional array as follows  
  - type var_name [ ] =  new type [size]  
  - type [ ] var_name  - new type [size]  
    - here type defines element data type
    - size determine no of elements in the array
    -  it is like declaring an array and allocating memory to it.
    - length property used to find the length of an array
    -  we can access array individual element by using index.


### 2. Linked List :  
Linked list is collection elements where each element as a seperate node and stored at non-contigous locations , each node consists of reference to the other nodes.  
Types of linked list :  
 - Singly Linked List : each node stores reference of the next node  
    - Ex : 5 -> 6 -> 7 -> NULL  
 - Doubly Linked List : each node store two references , one points to the next node and other points to the previous node.
    - Ex : NULL <-> 5 <-> 6 <-> 7 <-> NULL  
 - Circular Linked List : where all nodes forms a cirle it can be singly circular or doubly circular linked list.
    - Ex : 5 -> 6 -> 7 -> 5