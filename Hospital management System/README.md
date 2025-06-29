# 🏥 نظام إدارة مستشفى - Hospital Management System

نظام برمجي مكتوب بلغة Java يُحاكي إدارة مستشفى صغير، ويغطي معلومات المرضى، الأطباء، التمريض، المواعيد، والفواتير. تم تصميم النظام باستخدام مبادئ البرمجة الكائنية (OOP) لتقسيم الكود بشكل منظم وقابل للتوسعة.

---

## 🎯 وصف المشروع

يهدف هذا النظام إلى تسهيل إدارة العمليات اليومية للمستشفى عبر واجهة تفاعلية نصية. يشمل:

- تسجيل المرضى والأطباء والممرضين والعاملين.
- إنشاء مواعيد بين المرضى والأطباء.
- إصدار الفواتير الطبية.
- عرض معلومات محدثة حول كل قسم.

---

## 🧩 مكونات النظام (الكلاسات)

| الكلاس                  | الوصف                                                   |
|-------------------------|----------------------------------------------------------|
| `Main.java`             | نقطة تشغيل البرنامج، تعرض القائمة وتتحكم بالتنقل بين الخيارات. |
| `HospitalManagement.java` | يحتوي على الدوال المسؤولة عن منطق إدارة المرضى، الأطباء، المواعيد... |
| `Person.java`           | كلاس أساسي يحتوي على الخصائص العامة مثل الاسم، العمر، الجنس. |
| `Patient.java`          | يرث من `Person`، يحتوي على رقم الهوية، التشخيص، بيانات الاتصال. |
| `Doctor.java`           | يرث من `Employee`، يحتوي على التخصص، الرقم المهني، القسم. |
| `Nurse.java`            | يمثل طاقم التمريض، يحتوي على معلومات مثل المسمى والدوام. |
| `Employee.java`         | كلاس عام للموظفين (الأطباء والممرضين)، يحتوي على ID وراتب. |
| `Worker.java`           | يمثل عمال المستشفى غير الطبيين (مثل خدمات النظافة). |
| `Appointment.java`      | يدير مواعيد المرضى مع الأطباء (تاريخ، وقت، طبيب، مريض). |
| `Invoice.java`          | يمثل الفاتورة المالية الخاصة بالمريض والمواعيد. |
| `Displayable.java`      | واجهة Interface لتنظيم آلية الطباعة والعرض للكائنات. |

---

## 🛠️ المواضيع المستخدمة

- **البرمجة الكائنية (OOP)**:
  - الوراثة (Inheritance)
  - التجريد (Abstraction)
  - التعدد (Polymorphism)
  - التغليف (Encapsulation)
- **المصفوفات/قوائم ArrayList** لتخزين البيانات مؤقتًا.
- **التعامل مع الكائنات** (Object Creation and Management).
- **Scanner** للتفاعل مع المستخدم.
- **واجهات (Interfaces)** لتنظيم السلوكيات المشتركة.

---

## 📈 أفكار مستقبلية لتطوير المشروع

في النسخ القادمة من المشروع، يمكن إضافة:

1. **حفظ واسترجاع البيانات** باستخدام ملفات `JSON` أو `CSV` أو قاعدة بيانات مثل `SQLite` أو `MySQL`.
2. **إضافة واجهة رسومية GUI** باستخدام JavaFX أو Swing لسهولة الاستخدام.
3. **نظام صلاحيات دخول (Login System)** للطبيب، المدير، والمستخدم العادي.
4. **ميزة التقارير**: عرض تقارير يومية أو شهرية عن الحالات والمواعيد.
5. **تحسين بنية الكود** باستخدام تصميم MVC (Model–View–Controller).
6. **دعم الطباعة وتوليد تقارير PDF أو Excel**.

---

## 👨‍💻 المطور

- الاسم: **ضيف الله الشارحي**  
- التخصص: هندسة برمجيـات
- مشروع مقرر :OOP
- تاريخ التنفيذ: 2025  
-جامعـة تعز المستوى الثاني  
---

## 📦 طريقة التشغيل

1. افتح المشروع في IntelliJ IDEA أو VS Code.
2. تأكد من وجود جميع ملفات `.java` داخل المسار `src/`.
3. شغّل البرنامج من `Main.java`.

```bash
javac Main.java
java Main