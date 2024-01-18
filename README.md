# Process Writeup

## Name: Wilson Huang
## Course: APCSA
## Period: 7
## Concept: Unit 5

### Introduction
In APCSA (Advanced Placement Computer Science A), we are learning about Java. Learning Java is somewhat similar to Javascript; so I am familiar with some of the code. In unit 5 we have been learning on how to write classes. This unit it has been challenging for me to understand because new concepts and vocab were presented to me which was confusing at the beginning. In this write up I will take you through some of the challenges I had when learning in unit 5 and the exam I had at the end

### Challenge 1
One challenge I had when learning about unit 5 is finding the reason why and when do use a void statment. To find the asnwer to this I watched this [youtube vidoe](https://www.youtube.com/watch?v=14Cfx3fpH-w) and I found out that you use a void method when you do not want to return anything in the class. 
#### Void Method
```java
public static void printMessage() {
        System.out.println("This is a void method. It doesn't return anything");
    }
```
#### Non Void Method
```java
public static String printMessage() {
        return "This is a void method. It doesn't return anything";
    }`
```

### Challenge 2
Another challenge I faced in unit 5 is static vs instances. I didn't understand what how and when they are used. To understand this I watched a couple youtube vidoes like [this](https://www.youtube.com/watch?v=-Y67pdWHr9Y). I learned that static methods belong to a class and dont need a specific object to work. On the other hand instance methods that belong to individual objects. 
#### Example
``` java
public static void printMessage() {
        System.out.println("This is a static method.");
    }

    public static void main(String[] args) {
        printMessage();
    }
```

### Challenge 3 
I this challenge I will take you through some of the mistakes I made on the unit 5 exam and the quiz.

### Challenge 3.1
Consider the following methods:
``` Java
public static double doStuff(int a) 
{
  return a / 2;
}
public static double doStuff(double val) 
{
  return val / 10;
}
```
What is output by the following?

System.out.println(doStuff(5) + doStuff(5.0));
  2.00.5 
  2.5 
  22.5 
  2.50.5 
  5 
For this question I chose `2.50.5` because I forgot you can only do that with strings and not primitives. 

#### Challenge 3.2
What is output by the following code?
```Java
public static void stuff(int w) 
{
  w -= 2;
}

public static void main(String[] args) 
{
  int n = 2;
  stuff(n);
  System.out.print(n);
}
```
  2 
  0 
  4 
  1 
  3 

For this question I chose 0 because I thought that you could just do 2-2. But I realised that you can't because the changes in stuff don't affect the orginal number. 

#### Challenge 3.3
Consider the following class declaration.

public class Dog 
{
   private String name;
   private String breed;
   public Dog(String name, String breed) 
   {
     this.name = name;
     this.breed = breed;
   }
   public String getBreed() 
   {
     return this.breed;
   }
   public void setBreed(String breed) 
   {
     this.breed = breed;
   }
   // There may be instance variables, constructors, and methods that are not shown.
}
Assume that the following declaration has been made.

Dog d1 = new Dog("Blackstar", "Black Labrador");

Which of the following statements is the most appropriate for changing the breed of d1 from "Black Labrador" to "Chocolate Labrador"?

```Java 
Dog.setBreed("Chocolate Labrador");
  
d1.breed = "Chocolate Labrador";
  
d1.setBreed("Chocolate Labrador");
  
Dog.breed = "Chocolate Labrador";
  
d1.getBreed("Chocolate Labrador");
```
I answered `d1.getBreed("Chocolate Labrador");`. This is wrong because `getBreed` does not take any parameters but returns the value of breed for a dog object. 

Takeaways
* Watch youtube videos when you don't get the material because there are a lot of resources that can help you online
* Try to understand why you got something wrong on the quiz and exam because it will help you better understand it.


