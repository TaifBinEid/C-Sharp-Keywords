# **class** keyword 

##  <p style="color: #ff79cd">Outline </p>

  * Meaning of the **class** keyword 
  * Purpose of the **class** keyword 
  * Sysntax
  * Example 
 
 &nbsp;


  ## Meaning of the **class** keyword 
a ***class*** is a template definition of the methods and variables in a particular kind of object . Thus, an object is a specific instance of a class; it contains real values instead of variables.

 
 &nbsp;

## The Purpose of an **class** keyword 
 A ***class*** enables you to create your custom types by grouping variables of other types, methods, and event , then you can make object ,  it's also possible to have many objects of the same kind that share characteristics: rectangles, employee records, video clips, and so on.


  

 &nbsp;

## Sysntax of **class** keyword 
* In ***C#***, a **class** can be defined by using the **class** keyword.
```
public class MyClass
```


 &nbsp;

## <p style="color: #ff79cd">Example  </p> 

 &nbsp;
 This example Illustrates  how to defined **class** and filed 
``` 
 public class Employee{

private int _empID;
private string _loginName;
private string _password;
private string _department;
private string _name;


// this is method show you how to use attributes of class in method.

public void Login(string loginName, string password)
{
    if (loginName == "TAIF" & password == "99g8")
    {
        _empID = 1;
        Department = "IT";
        Name = "TAIF BIN EID";
    }
    else if (loginName == "FAI" & password == "939t")
    {
        _empID = 2;
        Department = "IS";
        Name = "FAI AHMED";
    }
    else
    {
        throw new Exception("Login incorrect.");
    }
}

 }

```

