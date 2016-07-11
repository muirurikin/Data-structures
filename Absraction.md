#Abstraction

## Abstract class in Java

A class that is declared with abstract keyword, is known as abstract class in java. It can have abstract and non-abstract methods (method with body).

Before learning java abstract class, let's understand the abstraction in java first.

* * *

#### Abstraction in Java

**Abstraction** is a process of hiding the implementation details and showing only functionality to the user.

Another way, it shows only important things to the user and hides the internal details for example sending sms, you just type the text and send the message. You don't know the internal processing about the message delivery.

Abstraction lets you focus on what the object does instead of how it does it.

#### Ways to achieve Abstaction

There are two ways to achieve abstraction in java

1. Abstract class (0 to 100%)
2. Interface (100%)

* * *

#### Abstract class in Java

A class that is declared as abstract is known as **abstract class**. It needs to be extended and its method implemented. It cannot be instantiated.

#### Example abstract class
```java
1. abstract class A{}  

* * *
```
#### abstract method

 A method that is declared as abstract and does not have implementation is known as abstract method.

#### Example abstract method
```java
1. abstract void printStatus();//no body and abstract  

* * *
```
#### Example of abstract class that has abstract method

In this example, Bike the abstract class that contains only one abstract method run. It implementation is provided by the Honda class.
```java
1. abstract class Bike{  
2.   abstract void run();  
3. }  
4.   
5. class Honda4 extends Bike{  
6. void run(){System.out.println("running safely..");}  
7.   
8. public static void main(String args[]){  
9.  Bike obj = new Honda4();  
10.  obj.run();  
11. }  
12. }  
```
#### Understanding the real scenario of abstract class

In this example, Shape is the abstract class, its implementation is provided by the Rectangle and Circle classes. Mostly, we don't know about the implementation class (i.e. hidden to the end user) and object of the implementation class is provided by the **factory method**.

A **factory method** is the method that returns the instance of the class. We will learn about the factory method later.

In this example, if you create the instance of Rectangle class, draw() method of Rectangle class will be invoked.

```java
1. abstract class Shape{  
2. abstract void draw();  
3. }  
4. //In real scenario, implementation is provided by others i.e. unknown by end user  
5. class Rectangle extends Shape{  
6. void draw(){System.out.println("drawing rectangle");}  
7. }  
8.   
9. class Circle1 extends Shape{  
10. void draw(){System.out.println("drawing circle");}  
11. }  
12.   
13. //In real scenario, method is called by programmer or user  
14. class TestAbstraction1{  
15. public static void main(String args[]){  
16. Shape s=new Circle1();//In real scenario, object is provided through method e.g. getShape() method  
17. s.draw();  
18. }  
19. }  
```
