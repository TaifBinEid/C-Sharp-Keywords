<div dir=rtl>

#  الكلمة المفتاحية **object**  

##  <p style="color: #c67ace">الفهرس </p>

  *  مفهوم | Concept   للكلمة  **object** 
  * مثال | Example 

 
 &nbsp;


  ## مفهوم | Concept   للكلمة  **object** 


تمثل الكلمة الأساسية **object** وهي اسم مستعار System.Object type
النوع الأساسي في التسلسل الهرمي لفئات(class hierarchy) في C# ، وتعتبر أيضا 
من الأنظمة الغير معرفه ***unified type system*** بالنسبة C# ، لذلك المستخدم هو الذي يعرف 
نوع المؤشر وقيمة النوع ، والوراثه سواء كانت مباشرة او غير مباشرة من ***System.object***
ويمكنك إسناد قيم للمتغيرات وقيم افتراضية.

 



 &nbsp;





  &nbsp;





  &nbsp;


# <p style="color: #c67ace">مثال | Example  </p>  

<div dir= ltr>

```C#
using System;
using System.Text;

class Program
{
    static void Main()
    {
        // هنا تم استخدام متغير val 
        // مؤشر لكائن وحيث من خلاله تم استدعاء داله GetType();
        object val = new StringBuilder();
        Console.WriteLine(val.GetType());
    }
}
```

 </div>