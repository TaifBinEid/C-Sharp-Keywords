<div dir=rtl>

#  الكلمة المفتاحية **private**  

##  <p style="color: #c67ace">الفهرس </p>

  *  مفهوم | Concept   للكلمة **private** 
  * البناء | Syntax  للكلمة **private** 
  * مثال | Example   

 
 &nbsp;


  ##  مفهوم | Concept   للكلمة **private** 
الكلمة الأساسية **private** هي معدل أي تعدل على وصول الأعضاء، 
**private** هو مستوى الوصول الأقل سماحًا. يمكن الوصول إلى الأعضاء الخاصين فقط داخل جسم الفصل class body  أو الهيكل الذي تم الإعلان عنه فيه مثل داله .





 &nbsp;

## البناء | Syntax  للكلمة **private** 

<div dir= ltr>

```C#
private string name ="taif;

```
</div>

>الان في هذا المثال ان المتغيرname   لا أحد يستطيع الوصول إليه ، الا المكان المعرف به لأنه private 


  &nbsp;


# <p style="color: #c67ace">مثال | Example  </p>  

<div dir= ltr>

```C#
public MyClass {

public int id ;
private string name; 

}

static void Main(string[] args)
 {
     MyClass c = nrw MyClass();

      c.id = 99887;
      c.name = "Taif"; //هنا سوف يظهر خطأ 
      
/* لأن المتغير name  تم تعريفه في class  ب private  لذلك تم منع الوصل له من خارج ال class
*/



}

```

 </div>