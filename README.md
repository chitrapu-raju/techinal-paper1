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

Code Example :  


    public static void main(String[] args) {
        int[] intArray = { 1,2,3,4,5}; //declaring array with integers by using array literals
        for(int i=0;i<intArray.length;i++){
            System.out.println("Element at index "+i+" : "+intArray[i]);
        }
        String [] stringArray = {"Ajay","Ram","Sam","Vinay"}; //declaring array with strings by using array literals
        for(int i=0;i<stringArray.length;i++){
            System.out.println("Element at index "+i+" : "+stringArray[i]);
        } 
      };


### 2. Linked List :  
Linked list is collection elements where each element as a seperate node and stored at non-contigous locations , each node consists of reference to the other nodes.  
Types of linked list :  
 - Singly Linked List : each node stores reference of the next node  
    - Ex : 5 -> 6 -> 7 -> NULL  
 - Doubly Linked List : each node store two references , one points to the next node and other points to the previous node.
    - Ex : NULL <-> 5 <-> 6 <-> 7 <-> NULL  
 - Circular Linked List : where all nodes forms a cirle it can be singly circular or doubly circular linked list.
    - Ex : 5 -> 6 -> 7 -> 5  

Code Example : 


    public static void main(String[] args)
    {
  
        LinkedList<Integer> llist = new LinkedList<Integer>();
  
        // Appending new elements at the end
        for (int i = 1; i <= 5; i++)
            llist.add(i);
  
        System.out.println(llist);
  
        llist.remove(3);
        // after deletion
        System.out.println(llist);
  
        // Printing elements one by one
        for (int i = 0; i < llist.size(); i++)
            System.out.print(llist.get(i) + " ");
    }

### 3. Stack : 
A Stack is a collection of elements that store entities as last in first out (LIFO) manner, with two basic principles which add elements and remove elements.
- Ex : Stacks are used maintaining function calls    

Code Example :  
  

    public static void main(String args[])
    {
        Stack<String> stack = new Stack<String>();
        stack.push("Ram");
        stack.push("Sam");
        stack.push("Vinay");
        stack.push("Prem");
 
        Iterator<String> itr = stack.iterator();
  
        // Printing the stack
        while (itr.hasNext()) {
            System.out.print(itr.next() + " ");
        }
  
        System.out.println();
  
        stack.pop();
  
        // Iterator for the stack
        itr = stack.iterator();
  
        // Printing the stack
        while (itr.hasNext()) {
            System.out.print(itr.next() + " ");
        }
    }

### 4.Queue : 
A Queue is a collection of elements that store entities as first in first out (FIFO) manner, with two basic principles
- enqueue : the elements added from the rear side
- dequeue : elements removed from the front side.  

Code Example :  

    public static void main(String args[])  

    {
        PriorityQueue<Integer> prQ = new PriorityQueue<Integer>();
  
        // Adding items to the priorityQueue using add()
        prQ.add(6);
        prQ.add(5);
        prQ.add(15);
  
        // Printing the top element of PriorityQueue
        System.out.println(prQ.peek());
  
        // Printing the top element and removing it
        System.out.println(prQ.poll());
  
        // Printing the top element again
        System.out.println(prQ.peek());
    }   


### Short Note On Non-Linear Data Structures :  

Unlike linear Data Structures in non-linear data structures data elements are not arranged in contigous manner,as the arrangement in nonsequential, so we cannot access and traverse in a single run.In the case of linear data structures element is connected to two elements , where as in non-linear data structure the element can be connected to more than  two elements. There are two types of non-linear data structure   
 - Tree  
  - Graphs

Reference Links : 

[Overview of Data Structures from Geek For Geeks](https://www.geeksforgeeks.org/overview-of-data-structures-set-1-linear-data-structures/)  

[Study Data Structures from Javatpoint-1](https://www.javatpoint.com/data-structure-tutorial)

[Study Data Structures from Javatpoint-2](https://www.javatpoint.com/linear-vs-non-linear-data-structure)

[Graphs and its representation](https://www.geeksforgeeks.org/graph-and-its-representations/?ref=lbp)  

[Introduction to Tree Data Structure](https://www.geeksforgeeks.org/introduction-to-tree-data-structure/) 