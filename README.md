# Learn-java
  Rules of oop:

1) inhertance:

class Animal{

 void display(){
 
System.out.println(" animals have four legs");

}

}

class Mammal extends Animal{
}

class Reptile extends Animal{
}

public class Dog extends Mammal{ 

void sleep(){

system.out.println("just night time");
}
 public static void main(String args[]){

      Animal a = new Animal();
      Mammal m = new Mammal();
      Dog d = new Dog();
     a.display();
     m.display();
     d.sleep();
   
   }
}

2)Encapsulation:

  class loan{

    private int loan;

    private String borrower;

    private int salary;

public int getloan()

{

    return loan; 
 
 }
 
public string getborrower()

{

    return borrower;
    
}

public int get salary()

{
    return salary;
}

public void setloan(int loan)

{

This.loan=loan;
 
}

public void setborrower(String borrower)

{

This.borrower=borrower;

}

public void setsalary(int salary)

{

This.salary=salary;

}

Public static void main(String[] args)

{

loan l=new loan();

l.setloan(70000);

l.setborrower("etc");

l.setsalary(25000);

System.out.println("the lone is"+l.getloan());

System.out.println("the brrower is "+ b.getbrrow());

System.out.println("The salary is" + b.salary());

}

3)polimorphism:

class Vehicle {

     public void move () {
     
         System.out.println ("Vehicles are used for moving from one place to another ");
    }
}

class Car extends Vehicle {

    public void move () {
    
      super. move (); // invokes the super class method
      
      System.out.println ("Car is a good medium of transport ");
      
    }
}

public class TestCar {

    public static void main (String args []){
    
        Vehicle b = new Car (); // Vehicle reference but Car object
        
        b.move (); //Calls the method in Car class
    }
}

4)Abstruct:

abstract class Shape{  

abstract void draw();  
}  
//In real scenario, implementation is provided by others i.e. unknown by end user 
 
class Rectangle extends Shape{  

void draw()

{

System.out.println("drawing rectangle");

}  

}  
  
class Circle1 extends Shape{

void draw(){System.out.println("drawing circle");

} 

}  
  
//In real scenario, method is called by programmer or user 

class TestAbstraction1{ 

public static void main(String args[])

{

Shape s=new Circle1();   //In real scenario, object is provided through method e.g. getShape() method 

s.draw(); 

} 

}  

 

 






