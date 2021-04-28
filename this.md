<div dir=rtl>

#  الكلمة المفتاحية **this**  

##  <p style="color: #c67ace">الفهرس </p>

  *   مفهوم | Concept   للكلمة  **this** 
  * البناء | Syntax  للكلمة  **this**  
  * مثال | Example  

 
 &nbsp;


  ##  مفهوم | Concept   للكلمة  **this** 

* يتم استخدام الكلمة الأساسية **this**   للإشارة الى instance من نفس الفئة **class**  
* يتم استخدامه أيضًا للتمييز بين معلمات **parameter** الداله وحقول الفئة إذا كان كلاهما يحمل نفس الاسم ، استخدام آخر  للكلمة الأساسية **this**   هو استدعاء مُنشئ آخر من مُنشئ في نفس الفئة **class**.


 &nbsp;




  &nbsp;

## البناء | Syntax  للكلمة  **this** 

<div dir= ltr>

```C#
public Student(int id, String name ) {
   this.id = id;
   this.name = name;

} 

```
</div>

> هنا بسبب تشابه اسماء parameter تم إستخدام **this** للتميز بينهم


  &nbsp;


# <p style="color: #c67ace">مثال | Example </p>  

<div dir= ltr>

```C#

using System;

class Student {
   public int id, 
   public String name ;

   public Student(int id, String name, ) {
      this.id = id;
      this.name = name;
 
   }

   public void showInfo() {
      Console.WriteLine(id + " " + name+);
   }
}

class StudentDetails {
   public static void Main(string[] args) {
      Student std1 = new Student(001, "Taif");
      Student std2 = new Student(002, "Waad");
      
      std1.showInfo();
      std2.showInfo();
     
   }
} 

```

 </div>