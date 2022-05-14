# Data Types



## نظرة على مفهوم أنواع البيانات

أنواع البيانات هي أنواع القيم التي تحتفظ فيها المتغيرات والثوابت والتي يمكن أن نتعامل معها في البرنامج مثل `String`   `Numbers` `` ، `Double` و `Boolean`.


- String : يمثل هذا نوع البيانات النصية مثل characters والنصوص strings.
- Number : يمثل هذا نوع البيانات الرقمية مثل الأعداد الصحيحة integers والأعداد ذات النقطة العشرية double و float.
- Boolean : يمثل هذا النوع إحدى القيمتين إما true أو false.
- null : يدل هذا النوع على عدم وجود قيمة.
- dynamic : يمثل هذا النوع جميع الانواع .

فيما يلي، ستتم مناقشة كل نوع من هذه الأنواع بشكل مفصل.

# 
# Dart – Data Types


| Data Type  انواع البيانات | Keyword الكلمه المفتاحيه |
| ------------------------- | ------------------------ |
| Numbers                   | int, double, num         |
| Strings                   | String                   |
| Booleans                  | bool                     |
| Lists                     | List                     |
| Maps                      | Map                      |


**الارقام Numbers :** 
الرقم في Dart Programming هو نوع البيانات المستخدم للاحتفاظ بالقيمة كرقم. 
يمكن تصنيف أرقام Dart على النحو التالي: 

- يتم استخدام نوع البيانات int لتمثيل الأعداد الصحيحة. 
- يتم استخدام نوع البيانات double لتمثيل أرقام الفاصلة . 
- نوع num هو نوع بيانات يأخذ صفات النوعين int و double.


    void main() {
       // declare an integer
       int valueInt1 = 2;             
       var valueInt2 = 4;
       // print the values integer 
       print(valueInt1);
       print(valueInt2);
      
       // declare a double
       double valueDouble1 = 1.2;  
       var valueDouble2 = 4.1;  
       // print the values double 
       print(valueDouble1);
       print(valueDouble2);
      
       // declare a num
       num valueNum1 = 1;
       num valueNum2 = 1.5; 
       // print the values num 
       print(valueNum1);
       print(valueNum1);
    }

المخرجات :


    2
    4
    1.2
    4.1
    1
    1



**النصوص String:** 
تستخدم لتمثيل الحروف والكلمات والجمل. ويتم تضمين النصوص في علامات اقتباس(“”) مفردة أو مزدوجة.

- كل ما يتم وضعه بين علامات الاقتباس (“”) يصبح نص


    void main() {
       // declare an String
       var welcomeMsg = "Welcome to dart languages course";
       String firstLetter = "F";
       String fullName = "Fahad Turki Alazmi";             
       String address = "321 Main Street";  
       String message = "The keyword string is used to represent string literals.";
       String alert = "(-_-) I watch you don't stop learning ... (-_^)"; 
    
       // print the values String 
       print(welcomeMsg);
       print(firstLetter);
       print(fullName);
       print(address);
       print(message);
       print(address);
    }

المخرجات :


    Welcome to dart languages course
    F
    Fahad Turki Alazmi
    321 Main Street
    The keyword string is used to represent string literals.
    321 Main Street



**القيمة منطقية Boolean:** 
تمثل القيم المنطقية معنى الصواب او الخطأ. ويتم استخدام الكلمات التالية (true and false) لتمثيل المنطق في DART.


    void main() {
       // declare an Boolean
       var isTvOn = false;      
       bool isDoorOpen = false;
       bool isstudentPass = true;
           
       // print the values Boolean 
       print(isTvOn);
       print(isDoorOpen);
       print(isstudentPass);
    
    }

المخرجات :


    false
    false
    true

 **القوائم او المصفوفات List :** 
نوع بيانات List يشبه array في لغات البرمجة الأخرى. ويتم استخدام List لتمثيل مجموعة من العناصر. يتم ترتيبها عن طريق index
فكر في القوائم على أنها متغير أو ثابت يتكون من مجموعة من القيم أو العناصر، ويمكن الوصول لكل خانة توجد بها قيمة أو عنصر من خلال رقم يدعى index والذي يمثل ترتيب القيمة أو العنصر بداخل المصفوفة.

لتعريف مصفوفة سنستخدم الأقواس المربعة `[]` ونضع القيم بداخلها ونفصل بين كل قيمة والأُخرى بفاصلة `,` ولتوضيح الفكرة دعنا نعرّف مصفوفة باسم `listNumbers` وتحتوي على ثلاثة أعداد، كما هو موضح في المثال التالي:


     
    void main() {
    var listNumbers = [1, 2, 3]; 
    }

في المثال السابق قمنا بإنشاء متغير باسم `listNumbers` يحتفظ بمصفوفة من الأعداد. لاحظ أن جميع القيم من نوع بيانات واحد وهو `Int`.


    void main() {
    
       // declare an List
       var nameInstructors = ["Fahad","Eman"];
       List nameStudents = ["Seed","Reem","Khaled","Sara","Slman"];
       List studentsDegree = [89.4,78,97.6,77,66.3,99];
       List<int> highDegrees = [89,97,99];
       List<double> lowDegrees = [67.2,64.3,70.9];
       List<String> languages = ["Arabic","English","Italian"];
    
     // print the values List 
       print(nameInstructors);
       print(nameStudents);
       print(studentsDegree);
       print(highDegrees);
       print(lowDegrees);
       print(languages);
    }

المخرجات :


    [Fahad, Eman]
    [Seed, Reem, Khaled, Sara, Slman]
    [89.4, 78, 97.6, 77, 66.3, 99]
    [89, 97, 99]
    [67.2, 64.3, 70.9]
    [Arabic, English, Italian]





مسودة
