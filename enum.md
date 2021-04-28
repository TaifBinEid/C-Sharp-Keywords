<div dir=rtl>

#  الكلمة المفتاحية **enum**  

##  <p style="color: #c67ace">الفهرس </p>

  *  مفهوم | Concept   للكلمة  **enum** 
  * البناء | Syntax  للكلمة  **enum**  
  * مثال | Example   

 
 &nbsp;


  ##  مفهوم | Concept   للكلمة  **enum** 
تمثل الكلمة الأساسية **enum**   والتي هي اختصار ل ***enumeration***  نوع بيانات القيمة value data type  وهي عبارة عن مجموعة من ثوابت الأعداد الصحيحة تم تسميتها ، ويتم تعريفها او الإعلان عنها بإستخدام الكلمة الأساسية **enum**       ، ولا يمكن أن يرث.



 &nbsp;




  &nbsp;

## البناء | Syntax  للكلمة  **enum** 

<div dir= ltr>

```C#
enum <enum_name> {
   enumeration list 
};

```
</div>

> * ***enum name***  وهي تحدد نوع  **enum** 
 >  * ***enumeration list***  وهي القائمه وتفصل بينهم بالفاصلة 
   


  &nbsp;


# <p style="color: #c67ace">مثال | Example  </p>  

<div dir= ltr>

```C#
using System;

namespace EnumApplication {
   class EnumProgram {
      enum Days { Sun, Mon, tue, Wed, thu, Fri, Sat }; //هنا تم تعريف enum 

      static void Main(string[] args) {
         int WeekdayStart = (int)Days.Mon; //عرف متغير وعملنا هنا تحويل لانه سوف يرجع Mon مع التحويل يرجع رقم 1 
         int WeekdayEnd = (int)Days.Fri;
         
         Console.WriteLine("Monday: {0}", WeekdayStart);
         Console.WriteLine("Friday: {0}", WeekdayEnd);
         Console.ReadKey();

         // المخرجات | output
         //Monday: 1
        //Friday: 5
      }
   }
}

```

 </div>