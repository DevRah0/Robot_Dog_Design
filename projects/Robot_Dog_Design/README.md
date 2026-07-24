# 🐕 Robot Dog Design

## Mechanical Engineering Project
### مشروع ضمن مسار الهندسة الميكانيكية

This project is part of my **Mechanical Engineering** portfolio and presents the initial mechanical design, structural analysis, and kinematic study of a quadruped robot dog prototype. The design was created using **Autodesk Fusion 360**, then imported into **Onshape** for model management and exporting all components as **STL** files. All parts were intentionally kept as separate bodies to simplify future modifications, manufacturing, and development.

### يعد هذا المشروع جزءًا من معرض أعمالي (Portfolio) في **الهندسة الميكانيكية**، ويعرض التصميم الميكانيكي الأولي والتحليل الإنشائي والدراسة الحركية لنموذج كلب روبوتي رباعي الأرجل. تم تصميم النموذج باستخدام **Autodesk Fusion 360** ثم استيراده إلى **Onshape** لإدارة النموذج وتصدير جميع الأجزاء بصيغة **STL**. وقد تم الحفاظ على جميع الأجزاء كأجسام منفصلة لتسهيل عمليات التعديل والتصنيع والتطوير المستقبلي.

---

## 📌 Project Information
### معلومات المشروع

| Item | Details |
|------|---------|
| **Category** | Mechanical Engineering |
| **Project** | Robot Dog Design |
| **Software** | Autodesk Fusion 360, Onshape |
| **Design Stage** | Mechanical Prototype |

| البند | التفاصيل |
|------|---------|
| **التصنيف** | الهندسة الميكانيكية |
| **المشروع** | تصميم كلب روبوتي |
| **البرامج المستخدمة** | Autodesk Fusion 360، Onshape |
| **مرحلة المشروع** | نموذج ميكانيكي أولي |

---

## 🔗 Onshape Model
### نموذج Onshape

https://cad.onshape.com/documents/c39b19768dcb838bffcd3f7e/w/2cd258778683d608ab94cff5/e/42b435cb983a031294b8b7b3?renderMode=0&uiState=6a5d94c8355269141b9ea2cd

---

## 📂 STL Files
### ملفات الطباعة ثلاثية الأبعاد

All robot components have been exported as individual **STL** files and are available inside the **STL** directory of this project.

### تم تصدير جميع أجزاء الروبوت بصيغة **STL**، وهي موجودة داخل مجلد **STL** الخاص بهذا المشروع.

---

## 📸 Prototype Visuals
### صور النموذج الأولي

### Top View
### المنظور العلوي

![Robot Top View](top_view.bmp)

### Side View
### المنظور الجانبي

![Robot Side View](side_view.bmp)

---

## 🛠️ Mechanical & Structural Specifications
### المواصفات الميكانيكية والهيكلية

- **Main Chassis:** A symmetrical body designed to house the electronics and battery at the center to maintain a stable Center of Mass (CoM).
- **Legs & Degrees of Freedom (DOF):** A two-jointed leg mechanism providing 2 DOF per leg for efficient pendulum-based locomotion, totaling four active joints.
- **Actuators:** Four SG90 micro servo motors mounted at the hip joints.
- **Dynamic Counterweight:** An upper rear extension inspired by a scorpion tail acts as an experimental dynamic counterweight to improve stability during walking.

### المواصفات

- **الهيكل الرئيسي:** جسم متناظر يستوعب البطارية والمكونات الإلكترونية في المنتصف للمحافظة على مركز الجاذبية.
- **الأرجل ودرجات الحرية:** تصميم يعتمد على مفصلين لكل رجل (2 DOF) بإجمالي أربعة مفاصل متحركة.
- **المحركات:** أربعة محركات سيرفو SG90 مثبتة عند مفاصل الحوض.
- **الثقل الموازن:** امتداد خلفي علوي يعمل كثقل موازن ديناميكي لتحسين الاتزان أثناء الحركة.

---

## 📊 Preliminary Torque Analysis
### الحسابات المبدئية للعزم

To verify that the selected actuators can support the robot during static standing:

- **Torque Formula:** Torque = Force × Lever Arm
- **Estimated Robot Weight:** 250 g
- **Load per Leg:** 0.125 kg
- **Lever Arm Length:** 4 cm

**Required Torque**

```
0.125 × 4 = 0.5 kg.cm
```

The SG90 micro servo provides approximately **1.8 kg.cm**, giving a comfortable safety margin over the required **0.5 kg.cm**.

### الحسابات

- قانون العزم: القوة × ذراع العزم.
- الوزن التقريبي للروبوت: 250 جم.
- الحمل على كل رجل: 0.125 كجم.
- طول ذراع العزم: 4 سم.

**العزم المطلوب**

```
0.125 × 4 = 0.5 kg.cm
```

يوفر محرك SG90 عزماً يصل إلى **1.8 kg.cm**، وهو أعلى بكثير من العزم المطلوب، مما يوفر عامل أمان جيد.

---

## 🔄 Locomotion & Stability
### آلية الحركة والاتزان

- **Walking Pattern:** Static Crawl Gait.
- One leg moves at a time while the remaining three legs maintain a stable support triangle.

### نمط الحركة

- يعتمد الروبوت على **Static Crawl Gait**.
- تتحرك رجل واحدة في كل خطوة مع بقاء ثلاث أرجل مرتكزة على الأرض للحفاظ على الاتزان.

---

## ⚠️ Expected Mechanical Challenges
### المشاكل الميكانيكية المتوقعة

- Plastic servo gear wear.
- Foot slippage on smooth surfaces.
- Chassis vibration due to the absence of shock absorption.

### المشاكل

- تآكل تروس محركات السيرفو البلاستيكية.
- انزلاق الأقدام على الأسطح الملساء.
- انتقال الاهتزازات إلى الهيكل الرئيسي.

---

## 🚀 Future Improvements
### التطويرات المستقبلية

- Mechanical suspension system.
- Rubberized feet for improved traction.
- Enhanced structural rigidity.
- Support for additional sensors and mechanisms.

### التطويرات

- إضافة نظام تعليق ميكانيكي.
- إضافة قواعد مطاطية لزيادة الاحتكاك.
- تحسين صلابة الهيكل.
- دعم مستشعرات وآليات إضافية.

---

## 📚 Repository Structure
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

### يمثل هذا المشروع أحد مشاريع مسار الهندسة الميكانيكية ضمن معرض الأعمال، وسيتم إضافة المزيد من المشاريع مستقبلًا.
