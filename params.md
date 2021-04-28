<div dir=rtl>

#  الكلمة المفتاحية **params**  

##  <p style="color: #c67ace">الفهرس </p>

  *  مفهوم | Concept   للكلمة  **params** 
  *  الغرض | Purpose من إستخدام كلمة **params** 
  * البناء | Syntax  للكلمة  **params**  
  * مثال | Example   

 
 &nbsp;


  ##  مفهوم | Concept   للكلمة  **params** 
الكلمة الأساسية **params** في لغه C#   تسمح للداله بإستقبال عدد من الParameter 
يتم استخدامها على المصفوفات Array   ، من خلال الكلمة الأساسية **params**
في مدخلات تعريف الداله  method argument    يمكن ان نمرر عدد من المدخلات arguments .




 &nbsp;

 ## الغرض | Purpose من إستخدام كلمة **params**
 يمكن استخدام الكلمة الأساسية **params**  في حال لم تكن تعرف عدد المدخلات إليك ،
كما أنها مفيدة لكتابه **كود نظيف** **clean code**     . بدلاً من استخدام طرق مختلفة ومجهده بشكل زائد لتمرير قيم متعددة ، يمكننا ببساطة إنشاء مصفوفة وتمريرها كقائمة قيم أو قائمة مفصولة بفاصلة.



  &nbsp;

## البناء | Syntax  للكلمة  **params**  

<div dir= ltr>

```C#
  public static int TotalMarks(params int[] list)  

```
</div>

> نلاحظ هنا انه عند تمرير المدخل وضع الكلمه **params**   والتي هي إشاره 
الى ***parameter***     أي يمكن تمرير عدد غير محدد من القيم .


  &nbsp;


# <p style="color: #c67ace">مثال | Example  </p>  

<div dir= ltr>

```C#
public MyClass {

        public static void UseParams(params object[] list)
        {
            for (int i = 0; i < list.Length; i++)
            {
                Console.WriteLine(list[i] + " ");
            }
            Console.WriteLine();
        }

static void Main(string[] args)
 {
     
            UseParams(1, 2, 3, 4);
            UseParams("1", 7, "Taif");
 //نلاحظ هنا مررنا اكثر من قيمه  ، وقيم من نوع مختلفه لان تم تحديد نوع ال Array as object 

}

```

 </div>