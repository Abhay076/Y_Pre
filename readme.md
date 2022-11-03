                                               Yamaha Question

1. ## Print a string in reverse order of words.
### input=> Abhay Yadav
### output=> Yadav Abhay
```java
public static String ReverseWord(String str){
       String result = "";
       int i = str.length()-1;
       int end = str.length();
       while(i>=0){
           if(str.charAt(i)==' '){
            result = result+str.substring(i+1,end)+" ";
            end = i;
            }
            i=i-1;
        }
            result = result+str.substring(i+1,end);
            return result;
}
```
1. ## write a program a string revesre order
  ## input=>abhay
  ## output=>yahba
```java
 public static String Solution( String ans){
    String ans ="";
    char ch;
    for(int i=0;i<ans.length();i++){
        ch=str.charAt(i);
        ans = ch+ans;
    }
    return ans;
 }
```
## write a program for a reverse a number
### input=>123
### output=>321
```java
    public static int Solution(int n){
        int rev=0;
        while(n>0){
            int rem=n%10;
            rev= rev*10+rem;
            n=n/10;
        }
        System.out.println(rev);
    }
```
## write a prgram check number is palindrome or not
### input=>454
### output=> true
```java
  public static void Solution(int n){
    int rev=0;
    int temp=n;
    while(n>0){
        int rem=n%10;
        rev=rev*10+rem;
        n=n/10;
    }
    if(rev==temp){
        System.out.println("palindrome");
    }
    else{
        System.out.println("Not palindrom");
    }
  }
```
## Given a string check palindrom or not.
## input => aba
## output => true
```java
   public static boolean Solution(String str){
      int i = 0;
      int j = str.length()-1;
      while(i<j){
        if(str.charAt(i)!=str.charAt(j)){
            return false;
        }
        i++;
        j--;
      }
      return false;
   } 
```
2. ## Technical Interview. Focus more on DBMS, SQL, and OOPS concepts. They will ask you to write queries such as find 10th highest marks, do join query, etc. 


3. ## Draw an ER diagram of the database in your project.

4. How to implement a map?
5. What is polymorphism in java?
6. Given a string find the occurrences of each character without using inbuilt ds,functions and loops?
7. What if I delete a row containing a foreign key to another table?
8. How to fetch the first 5 elements from a table?
9. SQL Joins?
10. How to take input in JSP based web page?
11. Trigger and it’s backend working.
12. Are java and C++ purely object-oriented? which one is/not and why?
13. What port do MySQL works upon?

14. Pattern
1 2 3 4 5
2 5
3 5
4 5
5
### Can you do it using only one loop?

15. Pattern
1
2 6
3 8 11
4 10 14 18

### Write a code for any of the sorting algorithm. Asked about the complexity of the code written. Optimize the complexity of the code.
## input=> 1 5 2 6 3
## output=> 1 2 3 5 6
```java
public static void main(String[] args)
    {
 
        // Custom input array
        int arr[] = { 4, 3, 2, 1 };
 
        // Outer loop
        for (int i = 0; i < arr.length; i++) {
 
            // Inner nested loop pointing 1 index ahead
            for (int j = i + 1; j < arr.length; j++) {
 
                // Checking elements
                int temp = 0;
                if (arr[j] < arr[i]) {
 
                    // Swapping
                    temp = arr[i];
                    arr[i] = arr[j];
                    arr[j] = temp;
                }
            }
 
            // Printing sorted array elements
            System.out.print(arr[i] + " ");
        }
    }
```
## Technical round in which basic questions on OOPs concepts, data structures were asked?

## print 1-n without loop.?
## input=> 5
## output=> 1 2 3 4 5
```java
  public static void print(int n){
    if(n==0){
        return;
    }
    print(n-1);
    System.out.print(n+" ");
  }
```
## questions like factorial, palindrome etc. Questions from DBMS and SQL?

## What are the differences between server-side and client-side scripting? (Hint: think speed and security Illustrate the differences between call-by-value and call-by-reference. What are the differences between function overloading and function overriding? (Hint: think polymorphism)

## swap to number without temp variable
```java
public static void main(String a[])
    {
        int x = 10;
        int y = 5;
        x = x + y;
        y = x - y;
        x = x - y;
        System.out.println("After swapping:"
                           + " x = " + x + ", y = " + y);
    }
```
## if you have 1-100 number to find the 2nd largest. what sorting will u use?
## input=> 1 2 3 4
## output=> 3
```java
 public static void second(int arr[]){
       int largest=Integer.MIN_VALUE;
       int secondLargest = Integer.MIN_VALUE;
       for(int i=0;i<arr.length;i++){
           if(arr[i]>largest){
               secondLargest=largest;
               largest=arr[i];
           }
           else if (arr[i] > secondLargest && arr[i] != largest){
                secondLargest = arr[i];
           }
       }
       System.out.println(secondLargest);
   }
```
## OOPs
### Access Modifier
1. ## Private
  ```The access level of a private modifier is only within the class. It
cannot be accessed from outside the class.```
2. ## Default. 
   The access level of a default modifier is only within the package. It
cannot be accessed from outside the package. If you do not specify any
access level, it will be the default.
3. ## Protected.
The access level of a protected modifier is within the package and
outside the package through child class. If you do not make the child class, it
cannot be accessed from outside the package.
4. ## public.
  The access level of a public modifier is everywhere. It can be accessed
from within the class, outside the class, within the package and outside the
package.
## Final Keyword
If you make any variable final, you cannot change the value of the final variable (It
will be constant).
```java 
 class Pen{
 final int price = 15;
}
public class MCQs {
 public static void main(String[] args) {
 Pen p = new Pen();
 p.price = 20;
 System.out.println(p.price);
 }
} 
```
There is a final variable price, we are going to change the value of this variable, but
it can't be changed because the final variable once assigned a value can never be
changed. Therefore this will give a compile time error.

## Overloading in Java
If a class
has multiple methods having same name but different in parameters, it is known as Method Overloading.

```java
class Adder{  
static int add(int a,int b){return a+b;}  
static int add(int a,int b,int c){return a+b+c;}  
}  
class TestOverloading1{  
public static void main(String[] args){  
System.out.println(Adder.add(11,11));  
System.out.println(Adder.add(11,11,11));  
}}
```
## Method Overriding in Java
If subclass (child class) has the same method as declared in the parent class, it is known as method overriding in Java.
```java
class Vehicle{  
  //defining a method  
  void run(){System.out.println("Vehicle is running");}  
}  
//Creating a child class  
class Bike2 extends Vehicle{  
  //defining the same method as in the parent class  
  void run(){System.out.println("Bike is running safely");}  
  
  public static void main(String args[]){  
  Bike2 obj = new Bike2();//creating object  
  obj.run();//calling method
  }  
}  
```
## vartual function in java
A virtual function is not any special function, but it is a member function that facilitates the method overriding mechanism.
## how is error handling done in java
The try-catch is the simplest method of handling exceptions. Put the code you want to run in the try block, and any Java exceptions that the code throws are caught by one or more catch blocks.
## What are sockets?
 A socket is a combination of port and IP address. An incoming packet has a port number which is used to identify the process that needs to consume the packet.
## what are port?
Port are the terms used in Transport Layer. 
The same port number can be used in different computer running on same software.
## what are the kernal in os?
Kernel is central component of an operating system that manages operations of computer and hardware. It basically manages operations of memory and CPU time.
1. Monolithic Kernel 
2. Micro Kernel
3. Hybrid Kernel – 
4.  Exo Kernel – 
## ACID Property in dbms
1. Atomicity
2. Consistency
3. Isolation
3. Durability
## primary key
1. Define each row/reacords uniquely in database.
1. Can not have null values.
1. one table can have one primary key.
1. Conatins unique value.
## unique value
A Table can have multiple unique keys.
it can have one Null value.

## forgien key
Used to link two tables together.
## Like
Like used to search for a specfic pattern in a column
## rename Query in sql
``` reaname table oldName to newName
and with multile table change we can add ,
```
## truncate Query in sql
empty entire table
we can uased when we want delete all data but structure is not delete its same
```truncate tableName```

## drop Query in SQL
we can used drop query in sql when we want to delete or destory table or database.
``` drop table tableName```
  or
``` drop database databaseName```

## ALTER IN SQL
alter means when we used to we are want exsiting table are modified
``` alter table Std add(address varchar(100));```
## how to insert data
``` insert into std values(101,"Neha",20,"xyz");```
## max in sql
``` select max(age) from tableName```