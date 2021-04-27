<div dir=rtl>

#  الكلمة المفتاحية **virtual**  

##  <p style="color: #c67ace">الفهرس </p>

  *  معنى كلمة  **virtual** 
  * بناء كلمة **Syntax of virtual** 
  * مثال  

 
 &nbsp;


  ##  معنى كلمة  **virtual** 
تُستخدم الكلمة الأساسية **virtual** لتعديل طريقة أو خاصية أو حدث تم تعريفه في الفئة الأساسية base class    والسماح بتعديلها في الفئة المشتقة  derived class. 


 &nbsp;

## بناء كلمة **Syntax of virtual**

<div dir= ltr>

```
public virtual void Test() { Console.WriteLine("Print"); 
}

```
</div>

>    

  &nbsp;


# <p style="color: #c67ace">مثال </p>  

<div dir= ltr>

```C#
 class A
 {
public virtual void Test() { Console.WriteLine("Print"); 
}
; }
 }

 class B : A {

public override void Test() { 
Console.WriteLine("Print"); 
Console.WriteLine("Print2"); 
}
; }

 }


```

 </div>

> هنا في هذا المثال تم تعريف داله من نوع void   واضفنا لها كلمه **virtual** حيث انها اضافت خاصيه على الداله وهي إمكانيه  الفئة المشتقة  derived class من التعديل على تنفيذ الداله الموجودة في الفئه الأساسية base class  ، وهي اختياريه في حال أردت أن تعدل على تنفيذ الداله أو تركها كما هي .

</div>


