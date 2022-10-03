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