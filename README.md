رنامج يحول رقم إلى صيغته المكتوبة بالحروف (مثلاً 42 ← forty two)، بالاعتماد على قاموس (numbers.dict) بدل ما تكون القيم مكتوبة يدويًا في الكود.
صيغة القاموس، الفرق بين Error وDict Error، حالة وجود وسيط واحد أو اثنين، شرط التعامل مع أرقام أكبر من unsigned int، إلخ
كيف تبني بارسر للقاموس، كيف تقسم الرقم لمجموعات (مئات، آلاف...)، وأي هياكل بيانات تناسب القيود المفروضة (بس malloc/free/open/read/write/close)
بالحالات الصعبة (الصفر، أرقام مو موجودة بالقاموس، أرقام كبيرة جدًا، تقليم الفراغات بسطور القاموس، إلخ



program that converts a number into its written-out form (e.g. 42 → forty two), driven by a dictionary file (numbers.dict) rather than hardcoded logic
dictionary format, error cases, Dict Error vs Error, 1 vs 2 arguments, the "handle numbers beyond unsigned int" constraint, etc.
design my approach — e.g. how to structure the dictionary parser, how to break the number into groups of hundreds/thousands, what data structures make sense given only malloc/free/open/read/write/close
tricky edge cases (leading zeros, "0" itself, numbers not covered by the dictionary, big numbers, trimming spaces in dict lines, etc.
