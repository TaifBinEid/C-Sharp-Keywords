<div dir=rtl>

#  الكلمة المفتاحية **in**  

##  <p style="color: #c67ace">الفهرس </p>

  *   مفهوم | Concept   للكلمة  **in** 
  *  البناء | Syntax  للكلمة **in** 
  * مثال | Example   

 
 &nbsp;


  ##   مفهوم | Concept   للكلمة  **in** 
تؤدي الكلمة الأساسية **in** إلى تمرير المدخلات بواسطة المرجع ولكنها تضمن عدم تعديل المدخلات. بمعنى آخر ، يتم إجراء أي عملية على المعامل . يتشابه إلى حد كبير مع  الكلمات الأساسية ref أو out ، باستثناء أنه لا يمكن تعديل المدخلات بالطريقة المطلوبة. 
 
 &nbsp;





  

 &nbsp;

##  البناء | Syntax  للكلمة **in** 
 <div dir=ltr>

```C#
in string word;
```



</div> 






 &nbsp;

# <p style="color: #c67ace">مثال | Example  </p>  

  &nbsp;



<div dir=ltr>

```C#
int readonlyArgument = 44;
InArgExample(readonlyArgument);
Console.WriteLine(readonlyArgument);     //  القيمه لازالت 44

void InArgExample(in int number)
{
 
    number = 19;
}
```

</div>

> يوضح المثال السابق أن المُعدِّل in غير ضروري عادةً في موقع الاستدعاء. مطلوب فقط في إعلان method.




 </div>