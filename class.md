<div dir=rtl>

#  الكلمة المفتاحية **class**  

##  <p style="color: #c67ace">الفهرس </p>

  *  معنى كلمة  **class** 
  * بناء كلمة **Syntax of class** 
  *   الغرض  من إستخدام  كلمة **class** ؟
  * مثال  

 
 &nbsp;


  ##  معنى كلمة  **class** 

***class*** هي تعريف قالب للعمليات والمتغيرات في نوع معين من الكائنات. وبالتالي ، فإن الكائن هو نسخه محددة للفئة  ***class*** , حيث يحتوي على قيم حقيقية بدلاً من المتغيرات.
 
 &nbsp;


## الغرض  من إستخدام  كلمة **class** ؟

 يمكنك ***class*** من إنشاء أنواعك المخصصة عن طريق تجميع متغيرات من أنواع وعمليات وأحداث أخرى ، كما يمكنك إنشاء كائن ، ومن الممكن أيضًا أن يكون لديك العديد من الكائنات من نفس النوع التي تشترك في الخصائص: المستطيلات ، تسجيلات الموظفين ومقاطع الفيديو وما إلى ذلك.

  

 &nbsp;

## بناء كلمة **Syntax of class**
 <div dir=ltr>

```C#
public class MyClass

```



</div> 






 &nbsp;

# <p style="color: #c67ace">مثال </p>  

  &nbsp;

> 

<div dir=ltr>

```C#
public class Employee{

private int _empID;
private string _loginName;
private string _password;
private string _department;
private string _name;

//   توضح لك هذه العملية  كيف يمكن استخدام المتغيرات في العمليات //method

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
</div>


> نلاحظ في هذا المثال أننا أنشأنا كلاس موظفين حيث يجمع فيه جميع البيانات والعمليات المشتركة بينهم بعد ذلك يمكن إنشاء كائن object  
وكل كائن يحمل بياناته الخاصه به ويقوم بتنفيذ العمليات حسب طريقته . 

 </div>