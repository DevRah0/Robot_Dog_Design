# 🐕 Robot Dog Design
### تصميم كلب روبوتي

**Mechanical Engineering Project**  
**مشروع ضمن مسار الهندسة الميكانيكية**

---

This project is part of my **Mechanical Engineering** portfolio and presents the initial mechanical design, structural analysis, and kinematic study of a quadruped robot dog prototype. The model was designed using **Autodesk Fusion 360**, then imported into **Onshape** for model management and exporting all components as **STL** files. All parts were intentionally kept as separate bodies to simplify future modifications, manufacturing, and development.

يعد هذا المشروع جزءًا من معرض أعمالي (**Portfolio**) في **الهندسة الميكانيكية**، ويعرض التصميم الميكانيكي الأولي، والتحليل الإنشائي، والدراسة الحركية لنموذج كلب روبوتي رباعي الأرجل. تم تصميم النموذج باستخدام **Autodesk Fusion 360** ثم استيراده إلى **Onshape** لإدارة النموذج وتصدير جميع الأجزاء بصيغة **STL**، مع الإبقاء على جميع الأجزاء منفصلة لتسهيل عمليات التعديل والتصنيع والتطوير مستقبلًا.

---

## 📌 Project Information
### معلومات المشروع

- **Category:** Mechanical Engineering  
  **التصنيف:** الهندسة الميكانيكية

- **Project:** Robot Dog Design  
  **المشروع:** تصميم كلب روبوتي

- **Software:** Autodesk Fusion 360, Onshape  
  **البرامج المستخدمة:** Autodesk Fusion 360 و Onshape

- **Design Stage:** Mechanical Prototype  
  **مرحلة المشروع:** نموذج ميكانيكي أولي

---

## 🔗 Onshape Model
### نموذج Onshape

https://cad.onshape.com/documents/c39b19768dcb838bffcd3f7e/w/2cd258778683d608ab94cff5/e/42b435cb983a031294b8b7b3?renderMode=0&uiState=6a5d94c8355269141b9ea2cd

---

## 📂 STL Files
### ملفات الطباعة ثلاثية الأبعاد

All robot components have been exported as individual **STL** files and are available inside the **STL** directory of this project.

تم تصدير جميع أجزاء الروبوت بصيغة **STL**، وهي متوفرة داخل مجلد **STL** الخاص بهذا المشروع.

---

## 📸 Prototype Visuals
### صور النموذج الأولي

#### Top View
#### المنظور العلوي

![Robot Top View](projects/Robot_Dog_Design/top_view.bmp)


#### Side View
#### المنظور الجانبي

![Robot Side View](projects/Robot_Dog_Design/side_view.bmp)

---

## 🛠️ Mechanical & Structural Specifications
### المواصفات الميكانيكية والهيكلية

- **Main Chassis:** A symmetrical body designed to house the electronics and battery at the center to maintain a stable Center of Mass (CoM).  
  **الهيكل الرئيسي:** جسم متناظر مصمم لاستيعاب البطارية والمكونات الإلكترونية في المنتصف للحفاظ على مركز الجاذبية.

- **Legs & Degrees of Freedom (DOF):** Two joints per leg, providing 2 DOF for efficient pendulum-based locomotion, resulting in four active joints.  
  **الأرجل ودرجات الحرية:** يعتمد التصميم على مفصلين لكل رجل (2 DOF)، بإجمالي أربعة مفاصل متحركة توفر حركة بندولية فعالة.

- **Actuators:** Four SG90 micro servo motors mounted at the hip joints.  
  **المحركات:** أربعة محركات سيرفو SG90 مثبتة عند مفاصل الحوض.

- **Dynamic Counterweight:** An upper rear extension inspired by a scorpion tail acts as an experimental dynamic counterweight to improve stability during walking.  
  **الثقل الموازن:** امتداد خلفي علوي مستوحى من ذيل العقرب يعمل كثقل موازن ديناميكي تجريبي لتحسين الاتزان أثناء المشي.

---

## 📊 Preliminary Torque Analysis
### الحسابات المبدئية للعزم

To verify that the selected actuators can safely support the robot during static standing, the required torque was calculated using the following equation.

للتحقق من قدرة المحركات المختارة على حمل الروبوت أثناء الوقوف الثابت، تم حساب العزم المطلوب باستخدام المعادلة التالية.

- **Torque Formula:** Torque = Force × Lever Arm  
  **قانون العزم:** العزم = القوة × ذراع العزم

- **Estimated Robot Weight:** 250 g  
  **الوزن التقريبي للروبوت:** 250 جم

- **Load per Leg:** 0.125 kg  
  **الحمل على كل رجل:** 0.125 كجم

- **Lever Arm Length:** 4 cm  
  **طول ذراع العزم:** 4 سم

**Required Torque**

```
0.125 × 4 = 0.5 kg.cm
```

The SG90 micro servo provides approximately **1.8 kg.cm**, offering an excellent safety margin over the required **0.5 kg.cm**.

يوفر محرك **SG90** عزماً يصل إلى **1.8 kg.cm**، وهو أعلى بكثير من العزم المطلوب (**0.5 kg.cm**) مما يوفر عامل أمان جيد لدعم الروبوت.

---

## 🔄 Locomotion & Stability
### آلية الحركة والاتزان

- **Walking Pattern:** Static Crawl Gait, where one leg moves at a time while the other three legs maintain a stable support triangle.

  **نمط المشي:** يعتمد الروبوت على **Static Crawl Gait**، حيث تتحرك رجل واحدة في كل خطوة بينما تبقى الأرجل الثلاث الأخرى مرتكزة على الأرض للحفاظ على الاتزان.

---

## ⚠️ Expected Mechanical Challenges
### المشاكل الميكانيكية المتوقعة

- **Servo Gear Wear:** Plastic gears inside SG90 servos may wear or fail due to repeated impacts.  
  **إجهاد التروس:** قد تتعرض التروس البلاستيكية لمحركات SG90 للتآكل أو الكسر نتيجة الصدمات المتكررة.

- **Foot Slippage:** Smooth plastic feet may reduce traction on flat surfaces.  
  **انزلاق الأقدام:** قد يؤدي تصميم الأقدام البلاستيكي إلى انخفاض الاحتكاك على الأسطح الملساء.

- **Chassis Vibration:** Lack of a suspension system transfers impacts directly to the chassis.  
  **اهتزاز الهيكل:** يؤدي غياب نظام امتصاص الصدمات إلى انتقال الاهتزازات مباشرة إلى الهيكل الرئيسي.

---

## 🚀 Future Improvements
### التطويرات المستقبلية

- Integrate a mechanical suspension system for shock absorption.  
  **إضافة نظام تعليق ميكانيكي لامتصاص الصدمات.**

- Add rubberized feet or rolling mechanisms to improve traction.  
  **إضافة قواعد مطاطية أو آلية أقدام متدحرجة لزيادة الاحتكاك.**

- Improve structural rigidity and weight distribution.  
  **تحسين صلابة الهيكل وتوزيع الوزن.**

- Support additional sensors and mechanical mechanisms.  
  **دعم مستشعرات وآليات ميكانيكية إضافية مستقبلًا.**

---

## 📁 Project Structure
### هيكل المشروع

```text
Mechanical_Engineering/
└── Robot_Dog_Design/
    ├── README.md
    ├── STL/
    ├── Robot_dog_v1.step
    ├── top_view.bmp
    └── side_view.bmp
```

This project is one of several Mechanical Engineering projects included in this portfolio. Additional projects will be added over time.

يمثل هذا المشروع أحد مشاريع مسار **الهندسة الميكانيكية** ضمن معرض الأعمال، وسيتم إضافة المزيد من المشاريع مستقبلًا.
