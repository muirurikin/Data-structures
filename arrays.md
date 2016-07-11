## Java Array

Normally, array is a collection of similar type of elements that have contiguous memory location.

**Java array** is an object the contains elements of similar data type. It is a data structure where we store similar elements. We can store only fixed set of elements in a java array.

Array in java is index based, first element of the array is stored at 0 index.

#### Advantage of Java Array

- **Code Optimization:** It makes the code optimized, we can retrieve or sort the data easily.
- **Random access:** We can get any data located at any index position.

* * *

#### Disadvantage of Java Array

- **Size Limit:** We can store only fixed size of elements in the array. It doesn't grow its size at runtime. To solve this problem, collection framework is used in java.

* * *

#### Types of Array in java

There are two types of array.

- Single Dimensional Array
- Multidimensional Array

* * *

#### Single Dimensional Array in java

#### Syntax to Declare an Array in java
```java
1. dataType[] arr; (or)  
2. dataType []arr; (or)  
3. dataType arr[];  
```
#### Instantiation of an Array in java
```java
1. arrayRefVar=new datatype[size];  
```
#### Example of single dimensional java array

Let's see the simple example of java array, where we are going to declare, instantiate, initialize and traverse an array.
```java
1. class Testarray{  
2. public static void main(String args[]){  
3.   
4. int a[]=new int[5];//declaration and instantiation  
5. a[0]=10;//initialization  
6. a[1]=20;  
7. a[2]=70;  
8. a[3]=40;  
9. a[4]=50;  
10.   
11. //printing array  
12. for(int i=0;i&lt;a.length;i++)//length is the property of array  
13. System.out.println(a[i]);  
14.   
15. }} 
```
