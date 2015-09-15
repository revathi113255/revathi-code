Day1
javac -d myPack myPack/ser/*.java
javac -d . myPack/ser/*.java
------------------------------

class Testarray
{  
public static void main(String args[]){  
  
int a[]=new int[5];//declaration and instantiation  
a[0]=10;//initialization  
a[1]=20;  
a[2]=70;  
a[3]=40;  
a[4]=50;  
  
//printing array  
for(int i=0;i<a.length;i++)//length is the property of array  
System.out.println(a[i]);  
  
}}  




class Testarray1{  
public static void main(String args[]){  
  
int a[]={33,3,4,5};//declaration, instantiation and initialization  
  
//printing array  
for(int i=0;i<a.length;i++)//length is the property of array  
System.out.println(a[i]);  
  
}}  



class Testarray2{  
static void min(int arr[]){  
int min=arr[0];  
for(int i=1;i<arr.length;i++)  
 if(min>arr[i])  
  min=arr[i];  
 System.out.println(min);  
}  
 public static void main(String args[]){  
 int a[]={33,3,4,5};  
min(a);//passing array to method  
  
}}  




class Testarray3{  
public static void main(String args[]){  
  
//declaring and initializing 2D array  
int arr[][]={{1,2,3},{2,4,5},{4,4,5}};  
  
//printing 2D array  
for(int i=0;i<3;i++){  
 for(int j=0;j<3;j++){  
   System.out.print(arr[i][j]+" ");  
 }  
 System.out.println();  
}  
  
}}  




class TestArrayCopyDemo {  
    public static void main(String[] args) {  
        char[] copyFrom = { 'd', 'e', 'c', 'a', 'f', 'f', 'e',  
                'i', 'n', 'a', 't', 'e', 'd' };  
        char[] copyTo = new char[7];  
  
        System.arraycopy(copyFrom, 2, copyTo, 0, 7);  
        System.out.println(new String(copyTo));  
    }  
}  





class Testarray5{  
public static void main(String args[]){  
//creating two matrices  
int a[][]={{1,3,4},{3,4,5}};  
int b[][]={{1,3,4},{3,4,5}};  
  
//creating another matrix to store the sum of two matrices  
int c[][]=new int[2][3];  
  
//adding and printing addition of 2 matrices  
for(int i=0;i<2;i++){  
for(int j=0;j<3;j++){  
c[i][j]=a[i][j]+b[i][j];  
System.out.print(c[i][j]+" ");  
}  
System.out.println();//new line  
}  
  
}}  


public class IfStatementDemo {

	public static void main(String[] args) {
		int a = 10, b = 20;
		if (a > b)
			System.out.println("a > b");
		if (a < b)
			System.out.println("b > a");
	}
}




public class SwitchCaseStatementDemo {

	public static void main(String[] args) {
		int a = 10, b = 20, c = 30;
		int status = -1;
		if (a > b && a > c) {
			status = 1;
		} else if (b > c) {
			status = 2;
		} else {
			status = 3;
		}
		switch (status) {
		case 1:
			System.out.println("a is the greatest");
			break;
		case 2:
			System.out.println("b is the greatest");
			break;
		case 3:
			System.out.println("c is the greatest");
			break;
		default:
			System.out.println("Cannot be determined");
		}
	}
}






Consider the following code snippet.

if (aNumber >= 0)
    if (aNumber == 0)
        System.out.println("first string");
else System.out.println("second string");
System.out.println("third string");


What output do you think the code will produce if aNumber is 3?



public class ForLoop
{ 
public static void main(String args[])
 { 

 for(int i=1; i<=10; i++)
 { 
System.out.print(i+" "); 
} 
System.out.println();

 for(int i=10; i>=1; i--) 
{ 
System.out.print(i+" ");
 }
 } 
}






public class Keyword
{
 public static void main(String args[])
{ for(int i=1; i<=10; i++)
 { if(i == 5)
{ System.out.println("Loop stopped at 5th iteration"); break; 
}
 }
 }
}




public class Keyword
{
 public static void main(String args[])
{ 
for(int i=1; i<=10; i++)
 {
if(i % 2 == 0) 
{ System.out.printf("\nLoop is at %dth iteration..",i);
 continue; 
} 
else if(i == 5) 
{ System.out.printf("\nLoop stoped at %dth iteration",i); break; } } } } 

 class Keyword
{
 public static void main(String args[])
{
 String s = "Saturday";
int whichSat = 2;
boolean isHoliday = false;
 
if (s == "Saturday")
{
    if (whichSat == 2)
    {
        if (isHoliday == false)
        {
            System.out.println("It is meeting today.");
        }
    }
}
else
{
    System.out.println("No meeting today.");
}
 }
}




class Palindrome{
	public static void main(String args[]){
		int num = Integer.parseInt(args[0]);
		int n = num; //used at last time check
		int reverse=0,remainder;
		while(num > 0){
			remainder = num % 10;
			reverse = reverse * 10 + remainder;
			num = num / 10;
		}
		if(reverse == n)
			System.out.println(n+" is a Palindrome Number");
		else
			System.out.println(n+" is not a Palindrome Number");
	}
}

class PrimeNo{
	public static void main(String args[]){
		int num = Integer.parseInt(args[0]);
		int flag=0;
		for(int i=2;i<num;i++){
			if(num%i==0)
			{
				System.out.println(num+" is not a Prime Number");
				flag = 1;
				break;
			}
		}
		if(flag==0)
			System.out.println(num+" is a Prime Number");
	}
}


public class SumOfDigits {
      public static void main(String[] args) {
            int n=Integer.parseInt(args[0]);
            if (n <= 0)
                  System.out.println("Integer you've entered is nonpositive.");
            else {
                  int sum = 0;
                                   while (n != 0) {
                       
                        sum += n % 10;
                       n /= 10;
                  }
                  System.out.println("Sum of digits: " + sum);
            }
      }
}

public class NumberFactorial {
 
        public static void main(String[] args) {
               
                int number = 5;
               
                            
                int factorial = number;
               
                for(int i =(number - 1); i > 1; i--)
                {
                        factorial = factorial * i;
                }
       
                System.out.println("Factorial of a number is " + factorial);
        }
}
class Student
{
int marks;
String name;
public int getMarks() {
		return marks;
	}
	public void setMarks(int marks) {
		this.marks = marks;
	}
public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}
public static void main(String[] args) {

    Student[] studentArray = new Student[7];
for(int i=0;i<4;i++)
{
    studentArray[i] = new Student();
}

    studentArray[0].setMarks(100);
 studentArray[1].setMarks(100);
studentArray[2].setMarks(100);
 studentArray[3].setMarks(100);
studentArray[0].setName("a");
 studentArray[1].setName("a");
studentArray[2].setName("a");
 studentArray[3].setName("a");

for(int i=0;i<4;i++)
{
    System.out.println(studentArray[0].getMarks());
}
       
}
}

import java.io.*;
class aaaaa
{
    public static void main(String[] args) throws 

IOException
    {
        BufferedReader br = new BufferedReader(new 

InputStreamReader(System.in));
        System.out.print("\nEnter the number of rows : ");
        int r = Integer.parseInt(br.readLine());
        for(int i=0;i<r;i++)
        {
            for(int k=r;k>i;k--)
            {
                System.out.print(" ");
            }
            int number = 1;
            for(int j=0;j<=i;j++)
            {
 
                 System.out.print(number+" ");
                 number = number * (i - j) / (j + 1);
                  
            }
            System.out.println();
        }
 
    }
}


Day2
------------------------------------------
CONSTRUCTOR
------------
class Bike1{  
Bike1()
{
System.out.println("Bike is created");
}  
public static void main(String args[])
{  
Bike1 b=new Bike1();  
}  
}  



class Student3{  
int id;  
String name;  
  
void display(){System.out.println(id+" "+name);}  
  
public static void main(String args[]){  
Student3 s1=new Student3();  
Student3 s2=new Student3();  
s1.display();  
s2.display();  
}  
}  



class Student4{  
    int id;  
    String name;  
      
    Student4(int i,String n){  
    id = i;  
    name = n;  
    }  
    void display(){System.out.println(id+" "+name);}  
   
    public static void main(String args[]){  
    Student4 s1 = new Student4(111,"Karan");  
    Student4 s2 = new Student4(222,"Aryan");  
    s1.display();  
    s2.display();  
   }  
}  



class Student5{  
    int id;  
    String name;  
    int age;  
    Student5(int i,String n){  
    id = i;  
    name = n;  
    }  
    Student5(int i,String n,int a){  
    id = i;  
    name = n;  
    age=a;  
    }  
    void display(){System.out.println(id+" "+name+" "+age);}  
   
    public static void main(String args[]){  
    Student5 s1 = new Student5(111,"Karan");  
    Student5 s2 = new Student5(222,"Aryan",25);  
    s1.display();  
    s2.display();  
   }  
}  

THIS
-------
class Student10{  
    int id;  
    String name;  
      
    Student10(int id,String name){  
    this.id = id;  
    this.name = name;  
    }  
    void display(){System.out.println(id+" "+name);}  
  
    public static void main(String args[]){  
    Student10 s1 = new Student10(111,"Karan");  
    Student10 s2 = new Student10(321,"Aryan");  
    s1.display();  
    s2.display();  
    }  
}  




class Student11{  
    int id;  
    String name;  
      
    Student11(int id,String name){  
    this.id = id;  
    this.name = name;  
    }  
    void display(){System.out.println(id+" "+name);}  
    public static void main(String args[]){  
    Student11 s1 = new Student11(111,"Karan");  
    Student11 s2 = new Student11(222,"Aryan");  
    s1.display();  
    s2.display();  
}  
}  



class Student12{  
    int id;  
    String name;  
      
    Student12(int i,String n){  
    id = i;  
    name = n;  
    }  
    void display(){System.out.println(id+" "+name);}  
    public static void main(String args[]){  
    Student12 e1 = new Student12(111,"karan");  
    Student12 e2 = new Student12(222,"Aryan");  
    e1.display();  
    e2.display();  
}  
}  



class Student13{  
    int id;  
    String name;  
    Student13(){System.out.println("default constructor is invoked");}  
      
    Student13(int id,String name){  
    this ();  
    this.id = id;  
    this.name = name;  
    }  
    void display(){System.out.println(id+" "+name);}  
      
    public static void main(String args[]){  
    Student13 e1 = new Student13(111,"karan");  
    Student13 e2 = new Student13(222,"Aryan");  
    e1.display();  
    e2.display();  
   }  
}  


STATIC
---------

The static can be:

variable (also known as class variable)
method (also known as class method)
block
nested class



class Student8{  
   int rollno;  
   String name;  
   static String college ="ITS";  
     
   Student8(int r,String n){  
   rollno = r;  
   name = n;  
   }  
 void display (){System.out.println(rollno+" "+name+" "+college);}  
  
 public static void main(String args[]){  
 Student8 s1 = new Student8(111,"Karan");  
 Student8 s2 = new Student8(222,"Aryan");  
   
 s1.display();  
 s2.display();  
 }  
}  




class Counter{  
int count=0;  
  
Counter(){  
count++;  
System.out.println(count);  
}  
  
public static void main(String args[]){  
  
Counter c1=new Counter();  
Counter c2=new Counter();  
Counter c3=new Counter();  
  
 }  
} 


class Counter2{  
static int count=0; 
  
Counter2(){  
count++;  
System.out.println(count);  
}  
  
public static void main(String args[]){  
  
Counter2 c1=new Counter2();  
Counter2 c2=new Counter2();  
Counter2 c3=new Counter2();  
  
 }  
}  


class A{  
 int a=40; 
   
 public static void main(String args[]){  
  System.out.println(a);  
 }  
}     



class A2{  
  static
{
System.out.println("static block is invoked");
}  
  public static void main(String args[]){  
   System.out.println("Hello main");  
  }  
}  



class A2{ 
A2()
{
System.out.println("constructor");
}
  static{System.out.println("static block is invoked1");}  
static
{
System.out.println("static block is invoked2");
}
static void m1()
{
System.out.println("static method");
}  
static
{
System.out.println("static block is invoked3");
}  
  public static void main(String args[]){  
   System.out.println("Hello main");  
  }  
} 

class A5
{  
  private A5()
{
System.out.println("Constructor invoked");
}

static A5 generate(){
return (new A5());
}

static
{
System.out.println("static block is invoked");
} 
}
class A2
{
  public static void main(String args[])

{  
A5 v=A5.generate();
   System.out.println("Hello main");  
  } 
  
}  


INHERITENCE
---------------
class Employee{  
 float salary=40000;  
}  
class Programmer extends Employee{  
 int bonus=10000;  
 public static void main(String args[]){  
   Programmer p=new Programmer();  
   System.out.println("Programmer salary is:"+p.salary);  
   System.out.println("Bonus of Programmer is:"+p.bonus);  
}  
}  

class X 
 {
X( )
{  System.out.println(“Inside X’s Constructor”); 
 }  }
class Y  extends X 
{Y( )
 { System.out.println(“Inside Y’s Constructor”); 
 } 
 }
class Z extends Y
 {
Z()
{ 
System.out.println(“Inside Z’s Constructor”);
  } 
 }
class OrderOfConstructorCallDemo
{
public static void main(String args[])
{
Z z = new Z(); 
 } 
}  



class A1 
{A1()
{ System.out.println("A1 no arg constructor");
 }A1(int a)
{System.out.println("A1 constructor "+ a);
 }}
class B1 extends A1
{B1()
{  System.out.println("B1 no arg constructor");}
B1(int b)
{  
super(1000);
System.out.println("B1 constructor "+ b); 
} }
class C1 extends B1
{C1()
 {System.out.println("C1 no arg constructor");}
C1(int c)
{ 
super(100);
System.out.println("C1 constructor "+ c);
 }}
class TestingInheritance
{
public static void main(String args[])
{C1 ca = new C1();
}




class A1 

{
A1()
{ System.out.println("A1 no arg constructor");
 }
A1(int a)
{
System.out.println("A1 constructor "+ a);
 }
}
class B1 extends A1
{
B1()
{  System.out.println("B1 no arg constructor");
 }
B1(int b)
{  
//super(1000);
System.out.println("B1 constructor "+ b); 
}
 }
class C1 extends B1
{
C1()
 {
System.out.println("C1 no arg constructor");
 }
C1(int c)
{ 
super(100);
System.out.println("C1 constructor "+ c);
 }
}
class TestingInheritance
{
public static void main(String args[])
{
C1 ca = new C1(10);
}
}

Class X
{   public void methodX()
   {
     System.out.println("Class X method");}}
Class Y extends X
{
public void methodY()
{
System.out.println("class Y method");
}}
Class Z extends Y
{
   public void methodZ()
   {
     System.out.println("class Z method");
   }
   public static void main(String args[])
   {
     Z obj = new Z();
     obj.methodX(); 
     obj.methodY();
     obj.methodZ(); 
  }
}

public class StaticTest
{
        public static StaticTest()
     {
         System.out.println("Static Constructor of the class");
     }
     public static void main(String args[])
     {
        
         StaticTest obj = new StaticTest();
     }
}
SUPER
-------
The super keyword in java is a reference variable that is used to refer immediate parent class object.


class Vehicle{  
  int speed=50;  
}  
class Bike3 extends Vehicle{  
  int speed=100;  
  void display(){  
   System.out.println(speed); 
  }  
  public static void main(String args[]){  
   Bike3 b=new Bike3();  
   b.display();  
}  
}  





class Vehicle{  
  int speed=50;  
}  
  
class Bike4 extends Vehicle{  
  int speed=100;  
      
  void display(){  
   System.out.println(super.speed);
  }  
  public static void main(String args[]){  
   Bike4 b=new Bike4();  
   b.display();  
     
}  
}



class A
{
int a,b;
A(int m, int n)
{a = m;b = n;}
void display()
{System.out.println("a and b are :" + a +" " +     b);}}
class B extends A
{
int c;
B(int m, int n, int o)
{super(m,n);c = o;
}
void display() 
{super.display();
System.out.println("c :" + c);
}
}
class OverrideDemo
{public static void main(String args[])
{B subOb = new B(4,5,6);subOb.display(); }
}

aggregation
------------------
class Operation{  
 int square(int n){  
  return n*n;  
 }  }  
class Circle{  
 Operation op; 
 double pi=3.14;  
  double area(int radius){  
   op=new Operation();  
   int rsquare=op.square(radius);//code reusability (i.e. delegates the method call).  
   return pi*rsquare;  
 }
   
 public static void main(String args[]){  
   Circle c=new Circle();  
   double result=c.area(5);  
   System.out.println(result);  
 }  
}  

final
---------------------

class Bike{  
  final void run(){System.out.println("running");}  
}  
     
class Honda extends Bike{  
   void run(){System.out.println("running safely with 100kmph");}  
     
   public static void main(String args[]){  
   Honda honda= new Honda();  
   honda.run();  
   }  
}  


class Bike9{  
 final int speedlimit=90;//final variable  
 void run(){  
  speedlimit=400;  
 }  
 public static void main(String args[]){  
 Bike9 obj=new  Bike9();  
 obj.run();  
 }  
}



final class Bike{}  
  
class Honda extends Bike{  
  void run(){System.out.println("running safely with 100kmph");}  
    
  public static void main(String args[]){  
  Honda honda= new Honda();  
  honda.run();  
  }  
}  


class Bike{  
  final void run(){System.out.println("running...");}  
}  
class Honda2 extends Bike{  
   public static void main(String args[]){  
    new Honda2().run();  
   }  
}  

Instanceof
----------------
class Simple1{  
 public static void main(String args[]){  
 Simple1 s=new Simple1();  
 System.out.println(s instanceof Simple); 
 }  
}  

class Animal{}  
class Dog1 extends Animal{ 
  
 public static void main(String args[]){  
 Dog1 d=new Dog1();  
 System.out.println(d instanceof Animal);  
 }  
}  


class Parent{}

class Child1 extends Parent{}

class Child2 extends Parent{}

class Test
{
  public static void main(String[] args)
  {
      Parent p =new Parent();
      Child1 c1 = new Child1();
      Child2 c2 = new Child2();
      
      System.out.println(c1 instanceof Parent);			
      System.out.println(c2 instanceof Parent);			
      System.out.println(p instanceof Child1);			
      System.out.println(p instanceof Child2);			
      }
}

class Animal{
}

class Mammal extends Animal{
}

class Reptile extends Animal{
}

public class Dog extends Mammal{

   public static void main(String args[]){

      Animal a = new Animal();
      Mammal m = new Mammal();
      Dog d = new Dog();

      System.out.println(m instanceof Animal);
      System.out.println(d instanceof Mammal);
      System.out.println(d instanceof Animal);
   }
}
package to another package

D:\>javac -d . pack/A.java

D:\>javac -d . mypack/B.java

D:\>java mypack.B
javac *.java -d d:
Hello
 polymorphism
----------------
METHOD OVERLOADING
---------------------
There are two ways to overload the method in java
By changing number of arguments
By changing the data type



class Calculation{  
  void sum(int a,int b){System.out.println(a+b);}  
  void sum(int a,int b,int c){System.out.println(a+b+c);}  
  
  public static void main(String args[]){  
  Calculation obj=new Calculation();  
  obj.sum(10,10,10);  
  obj.sum(20,20);  
  
  }  
}  



class Calculation2{  
  void sum(int a,int b){System.out.println(a+b);}  
  void sum(double a,double b){System.out.println(a+b);}  
  
  public static void main(String args[]){  
  Calculation2 obj=new Calculation2();  
  obj.sum(10.5,10.5);  
  obj.sum(20,20);  
  
  }  
}  

RUNTIME POLYMORPHISM
--------------------------
Polymorphism in java is a concept by which we can perform 
a single action by different ways. Polymorphism is derived from 2 greek words: 
poly and morphs. The word "poly" means many and "morphs" 
means forms. So polymorphism means many forms.

There are two types of polymorphism in java: 
compile time polymorphism and runtime polymorphism.
 We can perform polymorphism in java by method overloading 
and method overriding.

Runtime polymorphism or Dynamic Method Dispatch is a 
process in which a call to an overridden method is 
resolved at runtime rather than compile-time.

Rules for Java Method Overriding
*************************************
method must have same name as in the parent class
method must have same parameter as in the parent class.
must be IS-A relationship (inheritance).


class ABC{
   public void disp()
   {
      System.out.println("disp() method of parent class");
   }
   public void abc()
   {
      System.out.println("abc() method of parent class");
   }	   
}
class Test extends ABC{
   public void disp(){
      System.out.println("disp() method of Child class");
   }
   public void xyz(){
      System.out.println("xyz() method of Child class");
   }
   public static void main( String args[]) {
      //Parent class reference to child class object
      ABC obj = new Test();
      obj.disp();
      obj.abc();
   }
}

public class X
{
    public void methodA() //Base class method
    {
        System.out.println ("hello, I'm methodA of class X");
    }
}

public class Y extends X
{
    public void methodA() //Derived Class method
    {
        System.out.println ("hello, I'm methodA of class Y");
    }
}
public class Z
{
   public static void main (String args []) {
       X obj1 = new X(); // Reference and object X
       X obj2 = new Y(); // X reference but Y object
       obj1.methodA();
       obj2.methodA();
   }
}

class Human{
   public void eat()
   {
      System.out.println("Human is eating");
   }
}
class Boy extends Human{
   public void eat(){
      System.out.println("Boy is eating");
   }
   public static void main( String args[]) {
      Boy obj = new Boy();
      obj.eat();
   }
}

class ABC{
   public void disp()
   {
      System.out.println("disp() method of parent class");
   }
   public void abc()
   {
      System.out.println("abc() method of parent class");
   }	   
}
class Test extends ABC{
   public void disp(){
      System.out.println("disp() method of Child class");
   }
   public void xyz(){
      System.out.println("xyz() method of Child class");
   }
   public static void main( String args[]) {
      //Parent class reference to child class object
      ABC obj = new Test();
      obj.disp();
      obj.abc();
   }
}
Output:

disp() method of Child class
abc() method of parent class



class MyBaseClass{
   public void disp()
   {
       System.out.println("Parent class method");
   }
}
class MyChildClass extends MyBaseClass{
   protected void disp(){
      System.out.println("Child class method");
   }
   public static void main( String args[]) {
      MyChildClass obj = new MyChildClass();
      obj.disp();
   }
}

garbage collection
---------------------


object unreference

There are many ways:

By nulling the reference
By assigning a reference to another

Advantages of Garbage Collection

Programmer doesn't need to worry about dereferencing an object.
It is done automatically by JVM.
Increases memory efficiency and decreases the chances for memory leak.
finalize() method

Sometime an object will need to perform some specific task before it is destroyed such as closing an open connection or releasing any resources held. To handle such situation finalize() method is used. finalize() method is called by garbage collection thread before collecting object. Its the last chance for any object to perform cleanup utility.


public class TestGarbage1{  
 public void finalize(){System.out.println("object is garbage collected");}  
 public static void main(String args[]){  
  TestGarbage1 s1=new TestGarbage1();  
  TestGarbage1 s2=new TestGarbage1();  
  s1=null;  
  s2=null;  
  System.gc();  
 }  
}  

public class MemoryTest{  
 public static void main(String args[])throws Exception{  
  Runtime r=Runtime.getRuntime();  
  System.out.println("Total Memory: "+r.totalMemory());  
  System.out.println("Free Memory: "+r.freeMemory());  
    
  for(int i=0;i<10000;i++){  
   new MemoryTest();  
  }  
  System.out.println("After creating 10000 instance, Free Memory: "+r.freeMemory());  
  System.gc();  
  System.out.println("After gc(), Free Memory: "+r.freeMemory());  
 }  
}  

public class Test
{
    
    public static void main(String[] args)
    {
        Test t = new Test();
        t=null;
        System.gc();
    }
    public void finalize()
    {
        System.out.println("Garbage Collected");
    }
}


public class RuntimeDemo {

   public static void main(String[] args) {
   try {

 
   System.out.println("Executing notepad.exe");

   
   Process process = Runtime.getRuntime().exec("notepad.exe");


   System.out.println("Notepad should now open.");

   } catch (Exception ex) {
   ex.printStackTrace();
   }

   }
}

class GarbageCollectionTest1{
  
public static void main(String [] args){
 
String str=new String("uestions");
// String object referenced by variable str and is not eligible for GC yet.
 
str=null;
//String object referenced by variable str is eligible for GC
}
}



class GarbageCollectionTest1{
  
public static void main(String [] args){
 
String str=new String("uestions");

String str1=new String("uestions");

str1=str;

}
}
http://bipinisahoo.blogspot.in/2012/04/explicitly-makes-objects-eligible-for.html

INSTANCEOF
------------
class Sample
{public static void main(String args[])
{Sample s=new Sample();
System.out.println(s instanceof Sample);
}
}

STRING
----------
charAt()
************

charAt() function returns the character located at the specified index.

String str = "studytonight";
System.out.println(str.charAt(2));


equalsIgnoreCase()
************

equalsIgnoreCase() determines the equality of two Strings, ignoring thier case (upper or lower case doesn't matters with this fuction ).

String str = "java";
System.out.println(str.equalsIgnoreCase("JAVA"));


length()
************

length() function returns the number of characters in a String.

String str = "Count me";
System.out.println(str.length());


replace()
************

replace() method replaces occurances of character with a specified new character.

String str = "Change me";
System.out.println(str.replace('m','M'));


substring()
************

substring() method returns a part of the string. substring() method has two forms,

public String substring(int begin);

public String substring(int begin, int end); 
The first argument represents the starting point of the subtring. If the substring() method is called with only one argument, the subtring returned, will contain characters from specified starting point to the end of original string.

But, if the call to substring() method has two arguments, the second argument specify the end point of substring.

String str = "0123456789";
System.out.println(str.substring(4));


System.out.println(str.substring(4,7));


toLowerCase()
************

toLowerCase() method returns string with all uppercase characters converted to lowercase.

String str = "ABCDEF";
System.out.println(str.toLowerCase());


toString()
************

toString() method returns the string representation of the object used to invoke this method. toString() is used to represent any Java Object into a meaningful string representation. It is declared in the Object class, hence can be overrided by any java class. (Object class is super class of all java classes.)

public class Car {
 public static void main(String args[])
 {
  Car c=new Car();  
  System.out.println(c);
 }
 public String toString()
 {
  return "This is my car object";
 }
}
Output : This is my car object

Whenever we will try to print any object of class Car, its toString() function will be called. toString() can also be used with normal string objects.


toUpperCase()
************

This method returns string with all lowercase character changed to uppercase.

String str = "abcdef";
System.out.println(str.toUpperCase());


trim()
************

This method returns a string from which any leading and trailing whitespaces has been removed.

String str = "   hello  ";
System.out.println(str.trim());


public class StringDemo {

   public static void main(String args[]) {
      String palindrome = "Dot saw I was Tod";
      int len = palindrome.length();
      System.out.println( "String Length is : " + len );
   }
}

public class StringDemo {

   public static void main(String args[]) {
      String string1 = "saw I was ";
      System.out.println("Dot " + string1 + "Tod");
   }
}

Java String startsWith() and endsWith() method

String s="Sachin";  
 System.out.println(s.startsWith("Sa"));  
 System.out.println(s.endsWith("n"));  

STRINGBUFFER
----------------
class A{  
public static void main(String args[]){  
StringBuffer sb=new StringBuffer("Hello ");  
sb.append("Java"); 
System.out.println(sb); 
}  
}  

class A{  
public static void main(String args[]){  
StringBuffer sb=new StringBuffer("Hello ");  
sb.insert(1,"Java");  
System.out.println(sb);  
}  
}  


class A{  
public static void main(String args[]){  
StringBuffer sb=new StringBuffer("Hello");  
sb.replace(1,3,"Java");  
System.out.println(sb);//prints HJavalo  
}  
}  

class A{  
public static void main(String args[]){  
StringBuffer sb=new StringBuffer("Hello");  
sb.delete(1,3);  
System.out.println(sb); 
}  
}  


class A{  
public static void main(String args[]){  
StringBuffer sb=new StringBuffer();  
System.out.println(sb.capacity());//default 16  
sb.append("Hello");  
System.out.println(sb.capacity());//now 16  
sb.append("java is my favourite language");  
System.out.println(sb.capacity());//now (16*2)+2=34 i.e (oldcapacity*2)+2  
}  
}  


http://beginnersbook.com/2013/04/oops-concepts/

Exception handling
---------------------------
Scenario where ArithmeticException occurs

If we divide any number by zero, there occurs an ArithmeticException.

int a=50/0;//ArithmeticException  
2) Scenario where NullPointerException occurs

If we have null value in any variable, performing any operation by the variable occurs an NullPointerException.

String s=null;  
System.out.println(s.length());//NullPointerException  
3) Scenario where NumberFormatException occurs

The wrong formatting of any value, may occur NumberFormatException. Suppose I have a string variable that have characters, converting this variable into digit will occur NumberFormatException.

String s="abc";  
int i=Integer.parseInt(s);//NumberFormatException  
4) Scenario where ArrayIndexOutOfBoundsException occurs

If you are inserting any value in the wrong index, it would result ArrayIndexOutOfBoundsException as shown below:

int a[]=new int[5];  
a[10]=50; //ArrayIndexOutOfBoundsException  
Java Exception Handling Keywords

There are 5 keywords used in java exception handling.




try
catch
finally
throw
throws

public class Testtrycatch1{  
  public static void main(String args[]){  
      int data=50/0;  
      System.out.println("rest of the code...");  
}  
}  


public class Testtrycatch2{  
  public static void main(String args[]){  
   try{  
      int data=50/0;  
   }catch(ArithmeticException e){System.out.println(e);}  
   System.out.println("rest of the code...");  
}  
}  



public class TestMultipleCatchBlock{  
  public static void main(String args[]){  
   try{  
    int a[]=new int[5];  
    a[5]=30/0;  
   }  
   catch(ArithmeticException e)
{System.out.println("task1 is completed");
}  
   catch(ArrayIndexOutOfBoundsException e)
{System.out.println("task 2 completed");
}  
   catch(Exception e)
{
System.out.println("common task completed");
}  
  
   System.out.println("rest of the code...");  
 }  
}  




class TestMultipleCatchBlock1{  
  public static void main(String args[]){  
   try{  
    int a[]=new int[5];  
    a[5]=30/0;  
   }  
   catch(Exception e){System.out.println("common task completed");}  
   catch(ArithmeticException e){System.out.println("task1 is completed");}  
   catch(ArrayIndexOutOfBoundsException e){System.out.println("task 2 completed");}  
   System.out.println("rest of the code...");  
 }  
}  



class Excep6{  
 public static void main(String args[]){  
  try{  
    try{  
     System.out.println("going to divide");  
     int b =39/0;  
    }catch(ArithmeticException e){System.out.println(e);}  
   
    try{  
    int a[]=new int[5];  
    a[5]=4;  
    }catch(ArrayIndexOutOfBoundsException e){System.out.println(e);}  
     
    System.out.println("other statement);  
  }catch(Exception e){System.out.println("handeled");}  
  
  System.out.println("normal flow..");  
 }  
}  



class TestFinallyBlock{  
  public static void main(String args[]){  
  try{  
   int data=25/5;  
   System.out.println(data);  
  }  
  catch(NullPointerException e){System.out.println(e);}  
  finally{System.out.println("finally block is always executed");}  
  System.out.println("rest of the code...");  
  }  
}  




class TestFinallyBlock1{  
  public static void main(String args[]){  
  try{  
   int data=25/0;  
   System.out.println(data);  
  }  
  catch(NullPointerException e){System.out.println(e);}  
  finally{System.out.println("finally block is always executed");}  
  System.out.println("rest of the code...");  
  }  
}  




public class TestFinallyBlock2{  
  public static void main(String args[]){  
  try{  
   int data=25/0;  
   System.out.println(data);  
  }  
  catch(ArithmeticException e){System.out.println(e);}  
  finally{System.out.println("finally block is always executed");}  
  System.out.println("rest of the code...");  
  }  
}  



public class TestThrow1{  
   static void validate(int age){  
     if(age<18)  
      throw new ArithmeticException("not valid");  
     else  
      System.out.println("welcome to vote");  
   }  
   public static void main(String args[]){  
      validate(13);  
      System.out.println("rest of the code...");  
  }  
}  

Method overridding with exception
--------------------------------

Rule: If the superclass method does not declare an
 exception,subclass overridden method cannot declare
 the checked 
exception.

import java.io.*;  
class Parent{  
  void msg(){System.out.println("parent");}  
}  
  
class TestExceptionChild extends Parent{  
  void msg()throws IOException{  
    System.out.println("TestExceptionChild");  
  }  
  public static void main(String args[]){  
   Parent p=new TestExceptionChild();  
   p.msg();  
  }  
}  

import java.io.*;  
class Parent{  
  void msg(){System.out.println("parent");}  
}  
  
class TestExceptionChild1 extends Parent{  
  void msg()throws ArithmeticException{  
    System.out.println("child");  
  }  
  public static void main(String args[]){  
   Parent p=new TestExceptionChild1();  
   p.msg();  
  }  
} 

 Rule: If the superclass method does not declare an exception, subclass 
overridden method cannot declare the checked exception 
but can declare unchecked exception.


Rule: If the superclass method declares an exception,
 subclass overridden method can declare same, 
subclass exception or no exception but cannot 
declare parent exception.

import java.io.*;  
class Parent{  
  void msg()throws ArithmeticException{System.out.println("parent");}  
}  
  
class TestExceptionChild2 extends Parent{  
  void msg()throws Exception{System.out.println("child");}  
  
  public static void main(String args[]){  
   Parent p=new TestExceptionChild2();  
   try{  
   p.msg();  
   }catch(Exception e){}  
  }  
}  

import java.io.*;  
class Parent{  
  void msg()throws Exception{System.out.println("parent");}  
}  
  
class TestExceptionChild3 extends Parent{  
  void msg()throws Exception{System.out.println("child");}  
  
  public static void main(String args[]){  
   Parent p=new TestExceptionChild3();  
   try{  
   p.msg();  
   }catch(Exception e){}  
  }  
}  





import java.io.*;  
class Parent{  
  void msg()throws Exception{System.out.println("parent");}  
}  
  
class TestExceptionChild5 extends Parent{  
  void msg(){System.out.println("child");}  
  
  public static void main(String args[]){  
   Parent p=new TestExceptionChild5();  
   try{  
   p.msg();  
   }catch(Exception e){}  
  }  
}  

Interface
---------------------------
http://beginnersbook.com/2013/05/java-interface/
http://www.journaldev.com/2752/java-8-interface-changes-static-methods-default-methods-functional-interfaces
https://blog.idrsolutions.com/2015/01/java-8-default-methods-explained-5-minutes/
http://www.programcreek.com/2014/12/default-methods-in-java-8-and-multiple-inheritance/

interface printable{  
void print();  
}  
  
class A6 implements printable{  
public void print(){System.out.println("Hello");}  
  
public static void main(String args[]){  
A6 obj = new A6();  
obj.print();  
 }  
}  



interface Printable{  
void print();  
}  
  
interface Showable{  
void show();  
}  
  
class A7 implements Printable,Showable{  
  
public void print(){System.out.println("Hello");}  
public void show(){System.out.println("Welcome");}  
  
public static void main(String args[]){  
A7 obj = new A7();  
obj.print();  
obj.show();  
 }  
} 



interface Printable{  
void print();  
}  
interface Showable{  
void print();  
}  
  
class TestTnterface1 implements Printable,Showable{  
public void print(){System.out.println("Hello");}  
public static void main(String args[]){  
TestTnterface1 obj = new TestTnterface1();  
obj.print();  
 }  
}  



interface Printable{  
void print();  
}  
interface Showable extends Printable{  
void show();  
}  
class Testinterface2 implements Showable{  
  
public void print(){System.out.println("Hello");}  
public void show(){System.out.println("Welcome");}  
  
public static void main(String args[]){  
Testinterface2 obj = new Testinterface2();  
obj.print();  
obj.show();  
 }  
}

shortcut for eclipse
---------------------
http://www.shortcutworld.com/en/win/Eclipse.html#link_9
dividing two digits
------------------------

package com.javatpoint;
import java.lang.annotation.*;  
import java.lang.reflect.*;  
    
class TestCustomAnnotation1{  
public static void main(String args[])throws Exception{  
  
	int four = 1234;  
	int first = four / 100;   
	int second = four % 100; 
	System.out.println(second);
	System.out.println(first);
}} 
 
http://www.javabeat.net/spring-dependson-attribute/
http://www.concretepage.com/spring/example_depends_on_spring
http://findnerd.com/list/view/depends-on-attributes-in-spring/1872/
http://www.tutorialspoint.com/spring/aspectj_based_aop_appoach.htm   



class Student18 implements Cloneable{  
int rollno;  
String name;  
  
Student18(int rollno,String name){  
this.rollno=rollno;  
this.name=name;  
}  
  
 
  
public static void main(String args[]) throws CloneNotSupportedException{  
 
Student18 s1=new Student18(101,"amit");  
  
Student18 s2=(Student18)s1.clone();  
  
System.out.println(s1.rollno+" "+s1.name);  
System.out.println(s2.rollno+" "+s2.name);  
  

}  
}
Collection
-------------------
Collection Subtypes: The following interfaces (collection types) extends the Collection interface:

  1.  List

  2.  Set 

  3. SortedSet

  4. NavigableSet

  5. Queue

  6. Deque  

Example :

import java.util.*;
import java.util.Collection;

public class collectioninterface {

public static void main(String[] args) {
Collection collection = new ArrayList();
collection.add("Dev");
collection.add("Manuals");
System.out.print(" Elements Of the Array List are ");
System.out.print(collection + ".");
}
}

import java.util.Arrays;
import java.util.List;

public class ArrayDemo1 {
   public static void main (String args[]) {   
   String a[] = new String[]{"abc","klm","xyz","pqr"};
      List list1 = Arrays.asList(a);
   System.out.println("The list is:" + list1);
   }
}
import java.util.ArrayList;
import java.util.List;

public class MyArrayList {

    public static void main(String[] args) {

     
        List<String> var = new ArrayList<>();

       
        var.add("Lars");
        var.add("Tom");

      
        var.forEach(System.out.println);
    }
} 
SET
-----------------
import java.util.*;

public class SetDemo {
	public static void main(String[] args) {

		Set st = new TreeSet();

		st.add("Gyan");
		st.add("Rohit");
		st.add("Anand");
		st.add("Arunesh");

		Iterator itr = st.iterator();

		while (itr.hasNext()) {
			String str = (String) itr.next();

			System.out.println("Name :" + str);
		}
	}

}

import java.util.*;

public class HashSetDemo {
        public static void main(String args[]) {

                HashSet HSet = new HashSet();

                HSet.add("C");
                HSet.add("A");
                HSet.add("B");
                HSet.add("E");
                HSet.add("F");
                HSet.add("D");
                System.out.println("The HashSet elements are: " + HSet);
        }
}


import java.util.*;

public class TreeSetDemo {
        public static void main(String args[]) {
               TreeSet oTreeSet = new TreeSet();
              
                oTreeSet.add("C");
                oTreeSet.add("A");
                oTreeSet.add("B");
                oTreeSet.add("E");
                oTreeSet.add("F");
                oTreeSet.add("D");
                System.out.println(oTreeSet);
        }
}


package ser;

import java.util.*;
import java.util.*;

public class aaa {
        public static void main(String args[]) {
               TreeSet oTreeSet = new TreeSet();
              
                oTreeSet.add("C");
                oTreeSet.add("A");
                oTreeSet.add("B");
                oTreeSet.add("E");
                oTreeSet.add("F");
                oTreeSet.add("D");
                System.out.println(oTreeSet);
                System.out.println(oTreeSet.descendingSet());
                
        }
}

import java.util.*;

public class LinkedHashSetDemo {
	public static void main(String args[]) {

		LinkedHashSet LHSet = new LinkedHashSet();
		LHSet.add("C");
		LHSet.add("A");
		LHSet.add("B");
		LHSet.add("E");
		LHSet.add("F");
		LHSet.add("D");
		System.out.println("The LinkedHashSet elements are: " + LHSet);
	}
}

package ser;

import java.util.NavigableMap;
import java.util.TreeMap;

public class aaa {

  public static void main(String[] args) {
		
	NavigableMap<String,Integer> navigableMap=new TreeMap<String, Integer>();
		
	navigableMap.put("X", 500);
	navigableMap.put("B", 600);
	navigableMap.put("A", 700);
	navigableMap.put("T", 800);
	navigableMap.put("Y", 900);
	navigableMap.put("Z", 200);
		
	System.out.printf("Descending Set  : %s%n",navigableMap.descendingKeySet());
	
	System.out.printf("Reverse Map : %s%n",navigableMap.descendingMap());
			
  }
	
}
public class ArrayListDemo {
        public static void main(String[] args) {

                ArrayList ALST = new ArrayList();

                ALST.add("One");
                ALST.add("Three");
                ALST.add("Two");
                ALST.add("Four");

                System.out.println("The ArrayList Elements are : " + ALST);

        }

}
import java.util.*;
class Test_Iterator
{
 public static void main(String[] args)
 {
  ArrayList< String> ar = new ArrayList< String>();
  ar.add("ab");
  ar.add("bc");
  ar.add("cd");
  ar.add("de");

 Iterator it = ar.iterator();    
  while(it.hasNext())
  {  
   System.out.print(it.next()+" ");
  }
 }
}


class Test_Iterator
{
 public static void main(String[] args)
 {
  ArrayList< String> ar = new ArrayList< String>();
  ar.add("ab");
  ar.add("bc");
  ar.add("cd");
  ar.add("de");

  ListIterator litr = ar.listIterator();
  while(litr.hasNext())                 //In forward direction
  {
   System.out.print(litr.next()+" ");
  }

  while(litr.hasPrevious())             //In backward direction
  {
   System.out.print(litr.next()+" ");
  }
 }
}

import java.util.*;
class ForEachDemo
{
 public static void main(String[] args)
 {
  LinkedList< String> ls = new LinkedList< String>();
  ls.add("a");
  ls.add("b");
  ls.add("c");
  ls.add("d");
  
  for(String str : ls)
  {
   System.out.print(str+" ");
  }
 }
}
public class LinkedListDemo {
        public static void main(String[] args) {

                LinkedList LKLST = new LinkedList();
                LKLST.add("Gyan");
                LKLST.add("Singh");
                LKLST.add("Arunesh");
                LKLST.add("Kumar");
                System.out.println("The LinkedList Elements are : " + LKLST);

        }
}
Map
---------------
package ser;
import java.util.*;
import java.util.*;

public class aaa {
        public static void main(String args[]) {
                HashMap hm = new HashMap();
                hm.put(1, "Gyan");
                hm.put(2, "Ankit");
                hm.put(3, "Arun");
                hm.put(4, "Anand");
                hm.put(5, "Ram");
                System.out.println(hm);
                System.out.println(hm.entrySet());
                System.out.println(hm.keySet());
                System.out.println(hm.values());
                
                
}

}
package ser;

import java.util.*;


public class aaa {
        public static void main(String args[]) {
                HashMap hm = new HashMap();
                hm.put(1, 1);
                hm.put(2, "Ankit");
                hm.put(3, "Arun");
                hm.put(4, "Anand");
                hm.put(5, "Ram");
                System.out.println(hm);
               int a= (Integer)hm.get(1);
                
        }              
                
}

package ser;
import java.util.*;
import java.util.*;

public class aaa {
        public static void main(String args[]) {
                HashMap hm = new HashMap();
                hm.put(1, "Gyan");
                hm.put(2, "Ankit");
                hm.put(3, "Arun");
                hm.put(4, "Anand");
                hm.put(5, "Ram");
                hm.put(6, "Ram");
                System.out.println(hm);
                System.out.println(hm.entrySet());
                System.out.println(hm.keySet());
                System.out.println(hm.values());
                
                
}

}

import java.util.*;

public class HashMapDemo {
        public static void main(String args[]) {
                HashMap hm = new HashMap();
                hm.put(1, "Gyan");
                hm.put(2, "Ankit");
                hm.put(3, "Arun");
                hm.put(4, "Anand");
                hm.put(5, "Ram");

                Set set = hm.entrySet();
                Iterator i = set.iterator();
                while (i.hasNext()) {
                        Map.Entry me = (Map.Entry) i.next();
                        System.out.print(me.getKey() + ": ");
                        System.out.println(me.getValue());
                }
                System.out.println();

        }
}

package ser;
import java.util.*;
public class aaa {
	public static void main(String args[]) {
		 TreeMap Tmap = new TreeMap();
         Tmap.put("Gyan", "Singh");
         Tmap.put("Ankit", "Kumar");
         Tmap.put("Arunesh", "Kumar");
         Tmap.put("Anand", "Nagar");
         Tmap.put("Ram", "Prakash");
         Set  set = Tmap.keySet();
         Iterator i = set.iterator();
         while (i.hasNext()) {
        	 System.out.println(i.next());
         }
         Collection set1 = Tmap.values();
         Iterator ii = set.iterator();
         while (ii.hasNext()) {
        	 System.out.println(ii.next());
         } 
	}
}
http://java67.blogspot.in/2015/01/how-to-sort-hashmap-in-java-based-on.html
http://www.dotnetperls.com/hashmap
import java.util.*;

public class CollectionsDemo {
   public static void main(String[] args) {
   // create map
   Map<String,String> map = new HashMap<String,String>();
      
   // populate the map
   map.put("1","TP"); 
   map.put("2","IS");
   map.put("3","BEST");
      
   // create a synchronized map
   Map<String,String> synmap = Collections.synchronizedMap(map);
     
   System.out.println("Synchronized map is :"+synmap);
   }
}
import java.util.*;

public class TreeMapDemo {
        public static void main(String args[]) {
                TreeMap Tmap = new TreeMap();
                Tmap.put("Gyan", "Singh");
                Tmap.put("Ankit", "Kumar");
                Tmap.put("Arunesh", "Kumar");
                Tmap.put("Anand", "Nagar");
                Tmap.put("Ram", "Prakash");
                Set <Map.Entry<String, String>> set = Tmap.entrySet();
                System.out.println("The Entries of the TreeMap are : ");
                for (Map.Entry<String, String> TM : set) {
                        System.out.print(TM.getKey() + " : ");
                        System.out.println(TM.getValue());
                }
        }
}


import java.util.*;

public class LinkedHashMapDemo {
        public static void main(String args[]) {
                LinkedHashMap Lhm = new LinkedHashMap();
                Lhm.put(1, "Gyan");
                Lhm.put(6, "Ankit");
                Lhm.put(5, "Arun");
                Lhm.put(4, "Anand");
                Lhm.put(3, "Ram");
                System.out.println("The Entries of LinkedHashMap are : " + Lhm);

        }
}

import java.util.*;

public class SortedSetDemo {
	public static void main(String args[]) {
		SortedSet Sset = new TreeSet();
		Sset.add("Gyan");
		Sset.add("Ankit");
		Sset.add("Arun");
		Sset.add("Anand");
		Sset.add("Ram");
		System.out.println("The SortedSet entries is as follows : " + Sset);
	}
}


import java.util.*;  
class TestCollection16{  
 public static void main(String args[]){  
   
  Hashtable<Integer,String> hm=new Hashtable<Integer,String>();  
  
  hm.put(100,"Amit");  
  hm.put(102,"Ravi");  
  hm.put(101,"Vijay");  
  hm.put(103,"Rahul"); 
 hm.put(null,"Rahul");  
  
  for(Map.Entry m:hm.entrySet()){  
   System.out.println(m.getKey()+" "+m.getValue());  
  }  
 }  
}  


import java.io.FileWriter;
import java.util.*;
  
public class aaa {  
public static void main(String[] args)throws Exception{  
  
Properties p=new Properties();  
p.setProperty("name","wipro");  
p.setProperty("email","jjj@wipro.com");  
  p.store(new FileWriter("e:\\info.properties"),"wipro Properties Example");  
  
}  
}  
package ser;


import java.util.*;


public class aaa {

  public static void main(String[] args) {

	List<String> list = new ArrayList<String>();
	list.add("a");
	list.add("b");
	list.add("c");
	list.add("d");
	list.add("b");
	list.add("c");
	list.add("a");
	list.add("a");
	list.add("a");

	System.out.println("\nExample 1 - Count 'a' with frequency");
	System.out.println("a : " + Collections.frequency(list, "a"));
  }
}

import java.util.*;

public class Test 
{
    
   public static void main(String[] args) 
   {
     Properties pr = new Properties();
     pr.put("Java", "James Ghosling");
     pr.put("C++", "Bjarne Stroustrup");
     pr.put("C", "Dennis Ritchie");
     pr.put("C#", "Microsoft Inc.");
     Set<?> creator = pr.keySet();
     
     for(Object ob: creator)
     {
         System.out.println(ob+" was created by "+ pr.getProperty((String)ob) );
     }
     
   }
    
}
 
package ser;

import java.util.ArrayList;
import java.util.Collections;
import java.util.HashMap;
import java.util.HashSet;
import java.util.List;
import java.util.Map;
import java.util.Set;
import java.util.TreeMap;

public class data {

  public static void main(String[] args) {

	List<String> list = new ArrayList<String>();
	list.add("a");
	list.add("b");
	list.add("c");
	list.add("d");
	list.add("b");
	list.add("c");
	list.add("a");
	list.add("a");
	list.add("a");

	System.out.println("\nExample 1 - Count 'a' with frequency");
	System.out.println("a : " + Collections.frequency(list, "a"));

	System.out.println("\nExample 2 - Count all with frequency");
	Set<String> uniqueSet = new HashSet<String>(list);
	for (String temp : uniqueSet) {
		System.out.println(temp + ": " + Collections.frequency(list, temp));
	}

	System.out.println("\nExample 3 - Count all with Map");
	Map<String, Integer> map = new HashMap<String, Integer>();

	for (String temp : list) {
		Integer count = map.get(temp);
		map.put(temp, (count == null) ? 1 : count + 1);
	}
	printMap(map);
				
	System.out.println("\nSorted Map");
	Map<String, Integer> treeMap = new TreeMap<String, Integer>(map);
	printMap(treeMap);
		
  }
	
  public static void printMap(Map<String, Integer> map){

	for (Map.Entry<String, Integer> entry : map.entrySet()) {
		System.out.println("Key : " + entry.getKey() + " Value : "
			+ entry.getValue());
	}
		
  }

}
import java.util.*;      
class TestVector1{      
 public static void main(String args[]){      
  Vector<String> v=new Vector<String>();//creating vector  
  v.add("umesh");//method of Collection  
  v.addElement("irfan");//method of Vector  
  v.addElement("kumar");  
  //traversing elements using Enumeration  
  Enumeration e=v.elements();  
  while(e.hasMoreElements()){  
   System.out.println(e.nextElement());  
  }  
 }      
}

System.out.println("Getting elements of Vector");
    System.out.println(v.get(0));
    System.out.println(v.get(1));
    System.out.println(v.get(2));

         
package ser;
import java.util.*;
class aaa
{
 public static void main(String[] args)
 {
	 LinkedList<Number> number = new LinkedList<Number>();
		   //List A2=new ArrayList();
		   number.add(11);
		   number.add(11.22);
		  
		   System.out.println("Unsorted List: "+number);
		  
}}


package ser;
import java.util.*;
class Student{  
	  int rollno;  
	  String name;  
	  int age;  
	  Student(int rollno,String name,int age){  
	   this.rollno=rollno;  
	   this.name=name;  
	   this.age=age;  
	  }  
	}  
 class aaa{  
	 public static void main(String args[]){  
	  //Creating user-defined class objects  
	  Student s1=new Student(101,"Sonoo",23);  
	  Student s2=new Student(102,"Ravi",21);  
	  Student s3=new Student(103,"Hanumat",25);  
	      
	  ArrayList<Student> al=new ArrayList<Student>();//creating arraylist  
	  al.add(s1);//adding Student class object  
	  al.add(s2);  
	  al.add(s3);  
	    
	  Iterator itr=al.iterator();  
	  //traversing elements of ArrayList object  
	  while(itr.hasNext()){  
	    Student st=(Student)itr.next();  
	    System.out.println(st.rollno+" "+st.name+" "+st.age);  
	  }  
	 }  
	} 
import java.util.Vector;
import java.util.Enumeration;

public class EnumerationTester {

   public static void main(String args[]) {
      Enumeration days;
      Vector dayNames = new Vector();
      dayNames.add("Sunday");
      dayNames.add("Monday");
      dayNames.add("Tuesday");
      dayNames.add("Wednesday");
      dayNames.add("Thursday");
      dayNames.add("Friday");
      dayNames.add("Saturday");
      days = dayNames.elements();
      while (days.hasMoreElements()){
         System.out.println(days.nextElement()); 
      }
   }
} 
package ser;

import java.util.*;


public class aaa {
        public static void main(String args[]) {
        	Hashtable<String,Double> balance = new Hashtable<String,Double>();
        	Enumeration names;
        	String str;
        	double bal;
        	balance.put("Arun", new Double(3434.34));
        	balance.put("Radha", new Double(123.22));
        	balance.put("Ram", new Double(99.22));
               
                
        }              
                
}


package ser;

public class aaa {
 
        public static void main(String[] args) {
               
                               int intArray[] = new int[]{5,90,35,45,150,3};
                               System.out.println("Array Before Bubble Sort");
                for(int i=0; i < intArray.length; i++){
                        System.out.print(intArray[i] + " ");
                }
               
                bubbleSort(intArray);
                               System.out.println("");
               
                System.out.println("Array After Bubble Sort");
                for(int i=0; i < intArray.length; i++){
                        System.out.print(intArray[i] + " ");
                }
 
        }
 
        private static void bubbleSort(int[] intArray) {
               
               
                int n = intArray.length;
                int temp = 0;
               
                for(int i=0; i < n; i++){
                        for(int j=1; j < (n-i); j++){
                               
                                if(intArray[j-1] > intArray[j]){
                                     
                                        temp = intArray[j-1];
                                        intArray[j-1] = intArray[j];
                                        intArray[j] = temp;
                                }
                               
                        }
                }
       
        }
}
import java.math.*;
import java.util.*;
public class aaa {
	
	public static void main(String args[]) {
		Map<String, Integer> items = new HashMap<>();
		items.put("A", 10);
		items.put("B", 20);
		items.put("C", 30);
		items.put("D", 40);
		items.put("E", 50);
		items.put("F", 60);
		
		items.forEach((k,v)->System.out.println("Item : " + k + " Count : " + v));
		
	}
}

import java.math.*;
import java.util.*;
public class aaa {
	
	public static void main(String args[]) {
		Map<String, Integer> items = new HashMap<>();
	items.put("A", 10);
	items.put("B", 20);
	items.put("C", 30);
	items.put("D", 40);
	items.put("E", 50);
	items.put("F", 60);
	
	items.forEach((k,v)->{
				if("E".equals(k))
			System.out.println(v);});
}
}


package ser;
import java.util.*;
public class ComparableDemo implements Comparable<ComparableDemo>{
  String name;
  ComparableDemo(String n){
    this.name=n;
  }
  public String getName(){
   return name;
  }
  public int compareTo(ComparableDemo e) {
    return (this.name).compareTo(e.name);
  }
  public static void main(String[] args) {
   List<ComparableDemo> l = new ArrayList<ComparableDemo>();
    System.out.println("Elements of list in a sorted order are =");
    l.add(new ComparableDemo("Anger"));
    l.add(new ComparableDemo("Tom"));
    l.add(new ComparableDemo("Titanic"));
    l.add(new ComparableDemo("Dummy"));
    l.add(new ComparableDemo("Bipul"));
    l.add(new ComparableDemo("Vinay"));
    l.add(new ComparableDemo("Rajesh"));
    l.add(new ComparableDemo("Ankit"));
    Collections.sort(l);
  for(ComparableDemo cd : l)
    System.out.println(cd.getName());
  }  
}


package ser;
import java.util.*;
class Person implements Comparable<Person>{
public String name;
public String lastName;

public Person(String name, String lastName){
  this.name=name;
  this.lastName=lastName;
}
public String getName(){
  return name;
}
public String getLastName(){
  return lastName;
}

public static void main(String arg[]){
  TreeSet myList = new TreeSet();
  myList.add(new Person("Robert","USA"));
  myList.add(new Person("Andy","UK"));
  myList.add(new Person("Harish","India"));
   for(Object persondata : myList){
	  Person person=(Person)persondata;
  System.out.println("My name is "+person.getName());
  }
}
public int compareTo(Person arg0) {
	 return this.name.compareTo(arg0.getName());
}
}
package ser;
import java.util.*;
public class Person {
	
	public static void main(String args[]) {
		int sum=0;
		Map<String, Integer> items = new HashMap();
		items.put("A", 10);
		items.put("B", 20);
		items.put("C", 30);
		items.put("D", 40);
		items.put("E", 50);
		items.put("F", 60);
		
		/*for (Map.Entry<String, Integer> entry : items.entrySet()) {
		    sum += entry.getValue();*/
		    System.out.println(sum);
		}
		
	}
}

package ser;
import java.util.*;
public class Person {
	
	public static void main(String args[]) {
		int sum=0;
		Map<String, Integer> items = new HashMap();
		items.put("A", 10);
		items.put("B", 20);
		items.put("C", 30);
		items.put("D", 40);
		items.put("E", 50);
		items.put("F", 60);
		
		for (float value : items.values()) {
		    sum += value;
		
		    System.out.println(sum);
		}
		
	}
}

package ser;
import java.util.ArrayList;  
import java.util.HashMap;  
import java.util.Iterator;  
import java.util.Map;  
  
public class Person {  
  
 static Map<String, ArrayList<String>> hashMap = new HashMap<String,  ArrayList<String>>();  
   
 public static void main(String[] args) {  
  retrieveValues();  
 }   
 public static void retrieveValues()  
 {     
  addValues("A", "a1");  
  addValues("A", "a2");  
  addValues("B", "b1");  
  addValues("B", "b2");  
  addValues("C", "c1");     
    
  Iterator<String> it = hashMap.keySet().iterator();   
  ArrayList<String> tempList = null;  
  
       while(it.hasNext()){   
           String key = it.next().toString();  
             tempList = hashMap.get(key);  
            if(tempList != null){  
                for(String value: tempList){   
                   System.out.println("Key : "+key+ " ,  Value : "+value); }  
               }   
        }  
 }    
 //Method to add duplicate key and values  
 private static void addValues(String key, String value)  
 {   
  ArrayList<String> tempList = null;        
  if(hashMap.containsKey(key)){    
   tempList=hashMap.get(key);   
   if(tempList == null)      
     tempList = new ArrayList<String>();       
   tempList.add(value);      
  }  
  else  
  {       
   tempList = new ArrayList();    
   tempList.add(value);       
   }       
  hashMap.put(key,tempList);  
 }   
}



import java.util.HashMap;
import java.util.Map;

public class HashMapExample {
	
	public static void main(String[] args) {
		Map vehicles = new HashMap();
		
		// Add some vehicles.
		vehicles.put("BMW", 5);
		vehicles.put("Mercedes", 3);
		vehicles.put("Audi", 4);
		vehicles.put("Ford", 10);
		
		System.out.println("Total vehicles: " + vehicles.size());
		
		// Iterate over all vehicles, using the keySet method.
		for(String key: vehicles.keySet())
			System.out.println(key + " - " + vehicles.get(key));
		System.out.println();
		
		String searchKey = "Audi";
		if(vehicles.containsKey(searchKey))
			System.out.println("Found total " + vehicles.get(searchKey) + " "
					+ searchKey + " cars!\n");
		
		// Clear all values.
		vehicles.clear();
		
		// Equals to zero.
		System.out.println("After clear operation, size: " + vehicles.size()); 
	}
}





package ser;

import java.util.*;

public class Person {
		public static void main(String[] args) {
		ArrayList<Integer> list = null;
		char sym;
		int num,sum=0;
		LinkedHashMap<Character,ArrayList<Integer>> cards = new LinkedHashMap<Character, ArrayList<Integer>>();
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter Number of Cards :");
		int n = sc.nextInt();
		for(int i = 0;i<n;i++){
			System.out.println("Enter card "+i+" :");
			sym = sc.next().charAt(0);
			num = sc.nextInt();
						if(cards.containsKey(sym))
			{
				list = (ArrayList<Integer>)cards.get(sym);
				list.add(num);
				cards.put(sym,list);
								}
			else {
				list = new ArrayList<Integer>();
				list.add(num);
				cards.put(sym, list);
				
				
			}
		}
		
		Set<Character> s = cards.keySet();
Iterator<Character> i = s.iterator();
		
		while(i.hasNext())
		{
			char c1 = i.next();
			
			if(cards.containsKey(c1))
			{
			Iterator number = cards.get(c1).iterator();
			while(number.hasNext()){
				sum=sum+(Integer)number.next();
				
			}
			
		}
			System.out.println(c1+" "+sum);
			sum=0;		
		}
		
	}
}
	

Feature of java
--------------
varargs
------------
class VarargsExample1{  
   
 static void display(String... values){  
  System.out.println("display method invoked ");  
 }  
  
 public static void main(String args[]){  
  
 display();   
 display("my","name","is","varargs");  
 }   
}  
      
foreach
-------------
class ForEachExample1{  
  public static void main(String args[]){  
   int arr[]={12,13,14,44};  
  
   for(int i:arr){  
     System.out.println(i);  
   }  
  
 }   
} 

static import
---------------------
import static java.lang.System.*;    
class StaticImportExample{  
  public static void main(String args[]){  
     
   out.println("Hello");//Now no need of System.out  
   out.println("Java");  
  
 }   
}

assertion
---------------
import java.util.Scanner;  
    
class AssertionExample{  
 public static void main( String args[] ){  
  
  Scanner scanner = new Scanner( System.in );  
  System.out.print("Enter ur age ");  
    
  int value = scanner.nextInt();  
  assert value>=18:" Not valid";  
  
  System.out.println("value is "+value);  
 }   
}

assertion enable
--------------------
javac AssertionExample.java
java -ea AssertionExample  


interface Clickable{
	default void click(){
		System.out.println("click");
	}
}
 
interface Accessible{
	default void access(){
		System.out.println("access");
	}
}
 
class Button implements Clickable, Accessible {
 
	public static void main(String[] args) {
		Button button = new Button();
		button.click();
		button.access();
	}
}



interface Clickable{
	static void click(){
		System.out.println("click");
	}
 
	default void print(){
		System.out.println("Clickable");
	}
}
 
interface Accessible{
	/*default void access(){
		System.out.println("access");
	}
 
	 default void print(){
		System.out.println("Accessible");
	}*/
}
 
 class Button implements Clickable, Accessible {
 
 public void print()
{
Clickable.super.print();
}

	public static void main(String[] args) {
		Button button = new Button();
		button.print();
Clickable.click();

		
	}
}

exception inside switch
------------------
package ser;

public class aaa {
	public static void main(String[] args) 
	{
	switch('/')
	{
	case '/':
        
        try{
                int i=10/0;                            

        }
        catch(ArithmeticException e)
        {System.out.println("eror");
        }
	}
	}    
}
import java.util.*;
class StringoHps
{

	public static void main(String[] args)
	{
		StringBuffer sb = new StringBuffer();
		Scanner sc = new Scanner(System.in);
		System.out.println("\n Enter a string : ");
		String s = sc.nextLine();
		s = Toggle(s.charAt(0),s);
		s = Toggle(s.charAt(s.length()-1),s);
		for(int i=s.length()-1;i>=0;i--)
		{
			sb.append(s.charAt(i));
		}
		String output = new String(sb);
		
		
		
		
		
		System.out.println(output);
		
		
	}
	public static String Toggle(char c,String s)
	{
		int a =c;
		int b=0;
		
		if(a>=65 && a<=90)
		{
			b = a+32;
		}
		if(a>=97 && a<=122)
			b = a-32;
	//	System.out.println("char a "+ (char)a + " char b"+ (char)b);
		s = s.replace((char)a,(char)b);	
		return s;
	}

}
multithreading
---------------------
class Multi extends Thread{  
public void run(){  
System.out.println("thread is running...");  
}  
public static void main(String args[]){  
Multi t1=new Multi();  
t1.start();  
 }  
}  



class Multi3 implements Runnable{  
public void run(){  
System.out.println("thread is running...");  
}  
  
public static void main(String args[]){  
Multi3 m1=new Multi3();  
Thread t1 =new Thread(m1);  
t1.start();  
 }  
}


class TestSleepMethod1 extends Thread{  
 public void run(){  
  for(int i=1;i<5;i++){  
    try{Thread.sleep(500);}catch(InterruptedException e){System.out.println(e);}  
    System.out.println(i);  
  }  
 }  
 public static void main(String args[]){  
  TestSleepMethod1 t1=new TestSleepMethod1();  
  TestSleepMethod1 t2=new TestSleepMethod1();  
   
  t1.start();  
  t2.start();  
 }  
} 


public class TestThreadTwice1 extends Thread{  
 public void run(){  
   System.out.println("running...");  
 }  
 public static void main(String args[]){  
  TestThreadTwice1 t1=new TestThreadTwice1();  
  t1.start();  
  t1.start();  
 }  
}  

class TestMultiPriority1 extends Thread{  
 public void run(){  
   System.out.println("running thread name is:"+Thread.currentThread().getName());  
   System.out.println("running thread priority is:"+Thread.currentThread().getPriority());  
  
  }  
 public static void main(String args[]){  
  TestMultiPriority1 m1=new TestMultiPriority1();  
  TestMultiPriority1 m2=new TestMultiPriority1();  
  m1.setPriority(Thread.MIN_PRIORITY);  
  m2.setPriority(Thread.MAX_PRIORITY);  
  m1.start();  
  m2.start();  
   
 }  
}  


Class Table{  
  
void printTable(int n){//method not synchronized  
   for(int i=1;i<=5;i++){  
     System.out.println(n*i);  
     try{  
      Thread.sleep(400);  
     }catch(Exception e){System.out.println(e);}  
   }  
  
 }  
}  
  
class MyThread1 extends Thread{  
Table t;  
MyThread1(Table t){  
this.t=t;  
}  
public void run(){  
t.printTable(5);  
}  
  
}  
class MyThread2 extends Thread{  
Table t;  
MyThread2(Table t){  
this.t=t;  
}  
public void run(){  
t.printTable(100);  
}  
}  
  
class TestSynchronization1{  
public static void main(String args[]){  
Table obj = new Table();//only one object  
MyThread1 t1=new MyThread1(obj);  
MyThread2 t2=new MyThread2(obj);  
t1.start();  
t2.start();  
}  
}  


   
ASSIGNMENT (THREAD)
----------------
class TestMultiNaming1 extends Thread{  
 public void run(){  
   System.out.println("running thread name is:"+Thread.currentThread().getName());  
   System.out.println("running thread priority is:"+Thread.currentThread().getPriority());  
  
  }  
 public static void main(String args[]){  
	 TestMultiNaming1 m1=new TestMultiNaming1();  
	 TestMultiNaming1 m2=new TestMultiNaming1();  
	 TestMultiNaming1 m3=new TestMultiNaming1();  
  m1.setPriority(Thread.MIN_PRIORITY);  
  m2.setPriority(Thread.MAX_PRIORITY);  
  m3.setPriority(Thread.NORM_PRIORITY);  
  m1.start();  
  m2.start();  
  m3.start();  
 }  
}    

//
 Runnable r = new Runnable1();
        Thread t = new Thread(r);
        Runnable r2 = new Runnable2();
        Thread t2 = new Thread(r2);
////////
public class Mythread {

    public static void main(String[] args) {
    	Runnable1 t= new Runnable1();
    	Runnable2 t2 = new Runnable2();
        t.start();
        t2.start();
    }
}

class Runnable2 extends Thread{
    public void run(){
        for(int i=0;i<11;i++){
            if(i%2 == 1)
                System.out.println("odd values"+i);
        }
    }
}

class Runnable1 extends Thread{
    public void run(){
        for(int i=0;i<11;i++){
            if(i%2 == 0)
                System.out.println("even values"+i);
        }
    }
}
class TestMultiNaming1 extends Thread{  
	
  public  void run(){  
	
	  System.out.println("After changing name:"+Thread.currentThread().getName()); 
	    
  }  
 public static void main(String args[]){  
  TestMultiNaming1 t1=new TestMultiNaming1();  
  TestMultiNaming1 t2=new TestMultiNaming1();  
  t1.start();  
     t1.setName("Scooby");
    t2.start();  
  t2.setName("Shaggy");  
  
 }  
} 



class MyThread extends Thread{  
 public void run(){  
  for(int i=1;i<=10;i++){
	  
	  if(i==6)
	  {
    try{Thread.sleep(5000);}catch(InterruptedException e){System.out.println(e);}
	  }
	  System.out.println(i); 
  }  
 }  
 public static void main(String args[]){  
	 MyThread t1=new MyThread();  
	 
  
  t1.start();  
 
 }  
} 

