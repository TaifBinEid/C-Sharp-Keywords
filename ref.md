<div dir=rtl>

#  الكلمة المفتاحية **ref**  

##  <p style="color: #c67ace">الفهرس </p>

  *  معنى كلمة  **ref** 
  * الغرض من استعمال كلمة **ref** 
  * بناء كلمة **Syntax of ref** 
  * مثال  

 
 &nbsp;


  ##  معنى كلمة  **ref** 
 **ref**  هي كلمة أساسية في ***C #*** تُستخدم  لتمرير مدخلات العملية من خلال مرجع. أو يمكننا القول أنه إذا تم إجراء أي تغييرات في هذه المدخلات في العملية فسوف تنعكس في هذا المتغير عندما يعود عنصر التحكم إلى ميثود الاستدعاء.
 
 &nbsp;

##  الغرض من استعمال كلمة **ref** 
تشير الكلمة الأساسية ref إلى أنه تم تمرير القيمة عن طريق المرجع. يتم استخدامه في أربعة سياقات مختلفة:

* في تعريف  method  وفي استدعاءه  ، لتمرير مدخلات إلى method عن طريق المرجع. 
 * في إرجاع method.
لإرجاع قيمة إلى المستدعي .

* في نص الكلاس ، للإشارة إلى تخزين قيمة مرجعية مرجعية محليًا كمرجع ينوي المتصل تعديله. أو للإشارة إلى أن متغيرًا محليًا يصل إلى قيمة أخرى عن طريق المرجع.




  

 &nbsp;

## بناء كلمة **Syntax of ref**
 <div dir=ltr>

```
ref string word;
```



</div> 






 &nbsp;

# <p style="color: #c67ace">مثال </p>  

  &nbsp;



<div dir=ltr>

```C#

using System;
  
class Tuwaiq {
  
    // Main Method
    public static void Main()
    {
  
        // هنا يتم إسناد قيمة المتغير 
        string str = "tuwaiq";
  
        // تمريره كمعامل مرجعي من خلال الكلمة ref
        SetValue(ref str);
  
        // لعرض النص 
        Console.WriteLine(str);
    }
  
    static void SetValue(ref string str1)
    {
  
        // للتأكد من قيمة المدخل
        if (str1 == "tuwaiq") {
            Console.WriteLine("Hello!! C#");
        }
  
        // إسناد قيمه جديده للمعامل
      
        str1 = "Welcome in tuwaiq bootcamp :)";

        //output
         // Hello!! C#
         //Welcome in tuwaiq bootcamp :)
    }
}
```

</div>






 </div>