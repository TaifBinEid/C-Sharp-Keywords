<div dir=rtl>

#  الكلمة المفتاحية **protected**  

##  <p style="color: #c67ace">الفهرس </p>

  * مفهوم | Concept   للكلمة **protected** 
  * البناء | Syntax  للكلمة**protected** 
  * مثال | Example   

 
 &nbsp;


  ## مفهوم | Concept   للكلمة **protected** 
الكلمة الأساسية **protected** هي معدل أي تعدل على وصول الأعضاء، 
يمكن الوصول إلى member **protected**  ضمن class     ومن سيرث من هذا ال class  أي الفئة المشتقة.



 &nbsp;

## البناء | Syntax  للكلمة**protected** 

<div dir= ltr>

```C#
protected string name ="taif;

```
</div>

> **protected** للفئة الأساسيه base class  يتم الوصول إليه فقط  من خلال الفئة  المشتقة  derived class


  &nbsp;


# <p style="color: #c67ace">مثال | Example  </p>  

<div dir= ltr>

```C#
class A
{
    protected int x = 123;
}

class B : A
{
    static void Main()
    {
        var a = new A();
        var b = new B();

        // a.x = 10;

        // صحيحة لأن B 
         ترث من  A
        b.x = 10;
    }
}

```
```
 تولد العبارة a.x = 10
 خطأً لأنه يتم إجراؤه ضمن 
  main method ،
   وليس مثيلاً للفئة B.

```

 </div>