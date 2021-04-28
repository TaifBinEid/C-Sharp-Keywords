<div dir=rtl>

#  الكلمة المفتاحية **as**  

##  <p style="color: #c67ace">الفهرس </p>

  *  مفهوم | Concept   للكلمة  **as** 
  * البناء | Syntax  للكلمة **Syntax of as** 
  *  الغرض | Purpose من إستخدام كلمة**as** ؟
  * مثال | Example   

 
 &nbsp;


  ##  مفهوم | Concept   للكلمة  **as** 
يتم استخدام عامل التشغيل ***as*** لإجراء التحويل بين أنواع المراجع المتوافقة أو الأنواع Nullable.
 
 &nbsp;


## الغرض | Purpose من إستخدام كلمة**as** ؟
 لإرجاع الكائن عندما يكون متوافقًا مع النوع المحدد وإرجاع **null** إذا لم يكن التحويل ممكنًا.


  

 &nbsp;

## البناء | Syntax  للكلمة**Syntax of as**
 <div dir=ltr>

```C#

 expression as type
```



</div> 






 &nbsp;

# <p style="color: #c67ace">مثال | Example  </p>  

  &nbsp;

> يوضح هذا المثال كيفية استخدام **as** 

<div dir=ltr>

```C#

class Test {
      
 
    public static void Main() {
          
        
        string value1 = "Test";
          
        
        object obj1 = value1;
          
        // هنا تم تحويل الاوبجكت إلى string 
        string value2 = obj1 as string;
          
        // للتأكد في حال تم التحويل او لا 
        if(value2 != null)
        {
            Console.WriteLine("Cast done successfully ");
        }
        // هنا ستتم طباعه هذه  الجمله لان نوع الاوبجكت اصبح string 
        // وتم اسناد قيمته الى value2
          
}

```

</div>

 </div>