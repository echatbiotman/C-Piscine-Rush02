
مجلد التسليم: ex00
الملفات المطلوب تسليمها ملف Makefile وجميع الملفات الضرورية
write, malloc, free, open, read, close الدوال المسموح بها
أنشئ برنامجا يأخذ رقما كوسيط ويحوله إلى قيمته الحرفية المكتوبة. .
اسم الملف التنفيذي : 02-rush .
سيتم تجميع كود المصدر الخاص بك على النحو التالي: .
make fclean
make
.
يمكن لبرنامجك أن يأخذ وسيطين كحد أقصى
.
إذا كان هناك وسيط واحد فقط، فهو الرقم الذي تحتاج إلى تحويله
.
إذا كان هناك وسيطان، فإن الوسيط الأول هو قاموس المرجع الجديد والوسيط الثاني هو الرقم الذي تحتاج إلى تحويله.
إذا لم يكن الوسيط الذي يمثل الرقم عددًا صحيحًا موجبا صالحا، فيجب أن يخرج .
برنامجك "خطأ" متبوعا بسطر جديد.
i
يجب أن يتعامل برنامجك مع الأرقام التي تتجاوز نطاق unsigned int
Exercise 00
rush-02
Turn-in directory: ex00/
Files to turn in: Makefile and all the necessary files
Allowed functions: write, malloc, free, open, read, close
• Create a program that takes a number as an argument and converts it to its written
letter value.
• Executable name: rush-02
• Your source code will be compiled as follows:
make fclean
make
• Your program can take up to 2 arguments:
◦ If there is only one argument, it is the number that you need to convert.
◦ If there are two arguments, the first argument is the new reference dictionary
and the second argument is the number that you need to convert.
• If the argument representing the number is not a valid and positive integer, your
program must output "Error" followed by a newline.
Your program should handle numbers beyond the range of unsigned int
يجب على برنامجك تحليل القاموس المعطى كمورد للمشروع. يجب استخدام القيم الموجودة بداخله . الطباعة النتيجة. يمكن تعديل هذه القيم.
يجب تحرير أي ذاكرة مخصصة على الكومة باستخدام (3) malloc) بشكل صحيح.
.
سيتم التحقق من ذلك أثناء التقييم.
سيحتوي القاموس على القواعد التالية: .
[رقم] من 0 إلى مسافات]: من 0 إلى مسافات] [أي أحرف قابلة للطباعة ] ni
ستقوم بإزالة المسافات قبل وبعد القيم في القاموس .
سيحتوي القاموس دائما على الأقل على المفاتيح الموجودة في قاموس المرجع. يمكن تعديل قيمها . ويمكن إضافة المزيد من الإدخالات، ولكن لا يمكن إزالة المفاتيح الأولية.
يمكن تخزين إدخالات القاموس بأي ترتيب .
يمكن أن تكون هناك أسطر فارغة في القاموس .
.
إذا واجهت أي أخطاء من تحليل القاموس، فيجب أن يخرج برنامجك "خطأ في القاموس \n".
إذا لم يسمح لك القاموس بإجراء تحويل الرقم المقدم، فيجب أن يخرج برنامجك "خطأ في . القاموس \n".
Your program must parse the dictionary given as a resource to the project. The
values inside it must be used to print the result. These values can be modified.
• Any memory allocated on the heap (with malloc(3)) must be freed correctly. This
will be verified during the evaluation.
• The dictionary will have the following rules:
[a number][0 to n spaces]:[0 to n spaces][any printable characters]\n
◦ You will trim the spaces before and after the values in the dictionary.
◦ The dictionary will always have at least the keys contained in the reference
dictionary. Their values can be modified, more entries can be added, but the
initial keys can’t be removed.
◦ The entries of the dictionary can be stored in any order.
◦ There can be empty lines in the dictionary.
◦ If you have any errors from the dictionary parsing, your program must output
"Dict Error\n".
◦ If the dictionary does not allow you to perform the conversion of the provided
number, your program must output "Dict Error\n".
• Example:
$> ./rush-02 42 | cat -e
forty two$
$> ./rush-02 0 | cat -e
zero$
$> ./rush-02 10.4 | cat -e
Error$
$> ./rush-02 100000 | cat -e
one hundred thousand$
$> grep "20" numbers.dict | cat -e
20 : hey everybody ! $
$> ./rush-02 20 | cat -e
hey everybody !$
يمكنك إكمال المكافآت التالية:
.
استخدام "-"، و"" ""، و"و " للاقتراب من الصيغة الكتابية الصحيحة.
القيام بنفس التمرين بلغة مختلفة، باستخدام قاموس آخر يحتوي على الإدخالات المترجمة.
.
.
استخدام read لقراءة الأرقام من المدخلات القياسية رقم واحد في كل سطر عندما تكون وسيطة سطر الأوامر للرقم هي "-".
Bonuses
You can complete the following bonuses:
• Using “-”, “,”, “and” to be closer to the correct written syntax.
• Doing the same exercise in a different language, using another dictionary which will
contain the translated entries.
• Using read to read numbers from the standard input (one per line) when the
command line argument for the number is “-”.
Example:
$> ./rush-02 -
42
forty two
0
zero
^D
$>

This assignment is not verified by a program. You are free to organize your files as
you wish, provided you submit the mandatory files and comply with the requirements.
Submit only the files requested by the subject of this project.
لا يتم التحقق من هذا الواجب بواسطة برنامج أنت حر في تنظيم ملفاتك كما تشاء، بشرط أن تقدم الملفات الإلزامية وتلتزم بالمتطلبات
!
قدم فقط الملفات المطلوبة من قبل موضوع هذا المشروع.
