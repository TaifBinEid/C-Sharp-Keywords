# **as** keyword 

##  <p style="color: #aa2ee6">Outline </p>

  * Meaning of the **as** keyword 
  *  Why we use **as** keyword ?
  * Sysntax
  * Example 

 
 &nbsp;


  ## Meaning of the **as** keyword 
 The ***as*** operator is used to perform conversion between compatible reference types or Nullable types.

 
 &nbsp;

##   Why we use **as** keyword ?
 to returns the object when they are compatible with the given type and return **null** if the conversion is not possible.




  

 &nbsp;

## Sysntax of **as** keyword 
 ```
 expression as type
 ```


 &nbsp;

## <p style="color: #aa2ee6">Example  </p> 


  > This example Illustrates  how to use **as**  operator
```
class Test {
      
 
    public static void Main() {
          
        
        string value1 = "Test";
          
        
        object obj1 = value1;
          
        // now try it to cast to a string
        string value2 = obj1 as string;
          
        // checking Successfully cast or not
        if(value2 != null)
        {
            Console.WriteLine("Cast done successfully ");
        }
          
}
 ```
  