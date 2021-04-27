<div dir=rtl>

#  الكلمة المفتاحية **override**  

##  <p style="color: #c67ace">الفهرس </p>

  *  معنى كلمة  **override** 
  * بناء كلمة **Syntax of override** 
  * مثال  

 
 &nbsp;


  ##  معنى كلمة  **override** 

تُستخدم الكلمة الأساسية **override**  للفئة المشتقة  أو تعديل داله افتراضية / أو حدث من فئة أساسية   class إلى فئة مشتقة  derived class. 


 &nbsp;

## بناء كلمة **Syntax of override**

<div dir= ltr>

```C#
public override void printInfo(){}

```
</div>

> أي داله override  نتستنج منها انها قابله للتعديل ويمكن إعاده صياغه الأوامر البرمجية فيها من super class .     

  &nbsp;


# <p style="color: #c67ace">مثال </p>  

<div dir= ltr>

```C#
abstract class Shape
{
    // تجاوز تنفيذ هذه الداله 
    public abstract int GetArea();
}

class Square : Shape
{
    int side;

    public Square(int n) => side = n;

    // هنا بما أن الداله abstract 
    // فهذا يعني انها تم فرض تنفيذها على الكلاس المشتق نكتب التعريف للداله مع اضافه كلمه override 
    public override int GetArea() => side * side;

    static void Main()
    {
        var sq = new Square(12);
        Console.WriteLine($"Area of the square = {sq.GetArea()}");
    }
}
// Output: Area of the square = 144


```

 </div>