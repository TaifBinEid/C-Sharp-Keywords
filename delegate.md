<div dir=rtl>

#  الكلمة المفتاحية **delegate**  

##  <p style="color: #c67ace">الفهرس </p>

  *  معنى كلمة  **delegate** 
  * بناء كلمة **Syntax of delegate** 
  *   الغرض  من إستخدام  كلمة **delegate** ؟
  * مثال  

 
 &nbsp;


  ##  معنى كلمة  **delegate** 
هو متغير نوع مرجعي  **reference type** يحمل المرجع أو المؤشر على عملية. يمكن تغيير المرجع في وقت التشغيل.

 &nbsp;


## الغرض  من إستخدام  كلمة **delegate** ؟
يتم استخدام  **delegate**  بشكل خاص من أجل تنفيذ الأحداث وطرق  معاودة الاتصال.**call-back** methods .



 &nbsp;

## بناء كلمة **Syntax of delegate**
>  يمكن **delegate** أن يشير إلى method لها نفس توقيع **delegate**. على سبيل المثال،
 <div dir=ltr>

```C#
public delegate string MyDelegate (string s);

```
</div> 

> ![Sysntax delegate](https://www.tutorialsteacher.com/Content/images/csharp/delegate-mapping.png)   
> مثال يوضح هيكله **delegate** وكيف يتم استدعاءه عن طريق اسم ال method 

 &nbsp;






 &nbsp;

# <p style="color: #c67ace">مثال </p>  

 > ![Sysntax goto](https://aspblogs.blob.core.windows.net/media/zeeshanhirani/WindowsLiveWriter/DelegatesinC3.0_11DC8/image_2.png
)
>   في هذا المثال بالبدايه تم تعريف توقيع او Signature of method **delegate** 
وتم استخدمه هذا التوقيع في دالتين بعد ذلك تم إنشاء متغير من نوع مرجعي يشير الى الmethod
وتم استخدامه كمتغير من نوع اخر واجراء العمليات عليه ثم الطباعه .




  &nbsp;


 </div>