<div dir=rtl>

#  الكلمة المفتاحية **abstract**  

##  <p style="color: #ff005c">الفهرس </p>

  *  معنى كلمة  **abstract** 
  * الغرض من استعمال كلمة **abstract** 
  * بناء كلمة **Syntax of abstract** 
  * مثال  

 
 &nbsp;


  ##  معنى كلمة  **abstract** 
يمكّنك من إنشاء فئات وأعضاء فئة ( **الحقول والعمليات ** ) غير مكتملة ويجب تنفيذها في فئة مشتقة أو فئة فرعية.
 &nbsp;

##  الغرض من استعمال كلمة **abstract** 
هو تقديم تعريف مشترك للفئة الأساسية التي يمكن للفئات المشتقة المتعددة أن تشترك فيها ، على سبيل المثال ، فئة القهوة ، نجد أن للقهوة أنواعًا عديدة ، لكنها تشترك في بعض الخصائص والعمليات ، وقد تكون طريقة تحضير هذه العملية مختلف.


  

 &nbsp;

## بناء كلمة **Syntax of abstract**


> يمكن إعلان الفئات على أنها ***abstract***  بوضع الكلمة الرئيسية ***abstract***  class قبل تعريف الفئة class.

<div dir =ltr>

```C#
public abstract class Coffe   
{
    public abstract void PrepareCoffee(int i);
} 

```
</div>

* قد تحدد فئات  **abstract** أيضًا طرقًا  **abstract**. يتم تحقيق ذلك عن طريق إضافة  الكلمة الرئيسية **abstract** قبل النوع إرجاع العملية.

* العمليات  **abstract** ليس لها تنفيذ في الفئة الأساسية base class
* عندما ترث فئة  **abstract** طريقة افتراضية من فئة أساسية ، يمكن للفئة abstract تجاوز الطريقة الافتراضية بطريقة  **abstract** ، دعنا نرى المثال:


> 






 &nbsp;

# <p style="color: #ff005c">مثال </p>  

  &nbsp;

  >
  <div dir =ltr> 

  ```C#
public class Coffe
{
    public virtual void PrepareCoffee(string typeOfCoffe)
    {
        // التنفيذ الاصلي
    }
}

public abstract class FlatWhite : Coffe
{
    public abstract override void PrepareCoffee(string typeOfCoffe);
} // هنا التنفيذ يعتمد على من سيرث الابستراكت كلاس

public class Latte : FlatWhite 
{
    public override void PrepareCoffee(string typeOfCoffe)
    {
        // التنفيذ الجديد
    }
}
```
 &nbsp;

 
 </div>