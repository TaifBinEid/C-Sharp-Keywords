<div dir=rtl>

#  الكلمة المفتاحية **base**  

##  <p style="color: #c67ace">الفهرس </p>

  *  استخدامات كلمة  **base** 
  * بناء كلمة **Syntax of base** 
  *  لماذا نستخدم  كلمة **base** ؟
  * مثال  

 
 &nbsp;


  ##  استخدامات  كلمة  **base** 
  باستخدام الكلمة الأساسية ، يمكننا:
 * الاستدعاء  من class  method الذي تم وراثته بواسطة ***base***  في الفئة المشتقة.

 * يمكن تحديد أي **base** class  منشئ والذي يجب استدعاؤه أثناء إنشاء instance للفئة (class )المشتقة.
 &nbsp;


## لماذا نستخدم  كلمة **base** ؟
 للوصول إلى أعضاء الفئه class member مثل الخصائص والعمليات وما إلى ذلك ، في الفئة المشتقة.


  

 &nbsp;

# <p style="color: #c67ace">مثال </p>  
هذا المثال يوضح القواعد  او syntax لل **base**
 <div dir=ltr>

```C#
 public class Person
{
    protected string id = "444-55-9999";
    protected string name = "Taif Bin Eid";

    public virtual void GetInfo()
    {
        Console.WriteLine("Name: {0}", name);
        Console.WriteLine("ID: {0}", id);
    }
}
class Student : Person
{// نلاحظ هناان كلاس الطالب يرث من الطالب لذلك بإمكانه الوصول الى الخصائص والعمليات //

    public string acadmicNo = "437004866";
    public int leve = 8 ; 
    public string major = "IT";
    public override void GetInfo()
    {
        //هنا تم استخدام  base
        //    لإستدعاء عملية GetInfo من  
        // خلال كلاس الأب.

        base.GetInfo();
        Console.WriteLine("Student Acadmic Number : {0} Level : {1} Major {2}",  acadmicNo  , level, major );
    }
}

```



</div> 




 </div>