# **base** keyword 

##  <p style="color: #fed049">Outline </p>

  * Meaning of the **base** keyword 
  * Purpose of the **base** keyword 
  * Sysntax
  * Example 

 
 &nbsp;


  ## Meaning of the **base** keyword 
 Using the base keyword, we can :
 > * Call a ***base*** class method that has been overridden by another method in the derived class.

> * and we can specify which ***base*** class constructor should be called while creating an instance of the derived class.

 
 &nbsp;

##   Purpose of the **base** keyword 
 to acces ***base*** class members such as properties, methods, etc., in the derived class.



  

 &nbsp;

## Sysntax  and example of **base** keyword  
 ```
 public class Person
{
    protected string id = "444-55-9999";
    protected string name = "Taif Bin Eid";

    public virtual void GetInfo()
    {
        Console.WriteLine("Name: {0}", name);
        Console.WriteLine("ID: {0}", id);
    }
}
class Student : Person
{
    public string acadmicNo = "437004866";
    public int leve = 8 ; 
    public string major = "IT";
    public override void GetInfo()
    {
        // Here i use base to call method GetInfo by parent or super class .

        base.GetInfo();
        Console.WriteLine("Student Acadmic Number : {0} Level : {1} Major {2}",  acadmicNo  , level, major );
    }
}
 ```

