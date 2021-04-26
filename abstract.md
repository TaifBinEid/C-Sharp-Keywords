# **abstract** keyword 

##  <p style="color:yellow">Outline </p>

  * Meaning of the **abstract** keyword 
  * purpose of the **abstract** keyword 
  * Sysntax
  * Example 
 
 &nbsp;


  ## Meaning of the **abstract** keyword 
enables you to create classes and class members (*Fields and Operations*) that are incomplete and must be implemented in a derived class or sub class.

 
 &nbsp;

## The purpose of an **abstract** class
 is to provide a common definition of a base class that multiple derived classes can share , For example, the class of coffee, we find that coffee has many types, but they share some characteristics and operations, and the method of preparing this process may be different.

 &nbsp;

## Sysntax of **abstract** keyword
* Classes can be declared as ***abstract*** by putting the keyword ***abstract*** before the class definition. 

* Abstract classes may also define abstract methods. This is accomplished by adding the ***keyword abstract*** before the **return** type of the method.

* Abstract methods have no implementation
* When an abstract class inherits a virtual method from a base class, the abstract class can override the virtual method with an abstract method ,let's see example :
```
public class Coffe
{
    public virtual void PrepareCoffee(string typeOfCoffe)
    {
        // Original implementation.
    }
}

public abstract class FlatWhite : Coffe
{
    public abstract override void PrepareCoffee(string typeOfCoffe);
}

public class Latte : FlatWhite 
{
    public override void PrepareCoffee(string typeOfCoffe)
    {
        // New implementation.
    }
}
```
 &nbsp;

## <p style="color:yellow">Example </p>

 &nbsp;
 This example Illustrates declared as abstract class and abstract method.
``` 
public abstract class Coffe   
{
    public abstract void PrepareCoffee(int i);
} 
```

