# مشروع التصميم الميكانيكي الأولي لكلب روبوتي
# Mechanical Design Prototype for a Quadruped Robot Dog

---

## 📐 1. النسخة العربية (Arabic Version)

هذا المستودع يحتوي على التصميم الميكانيكي الأولي والتحليل الحركي لنموذج كلب روبوتي رباعي الأرجل تم تصميمه ميكانيكياً باستخدام برنامج Autodesk Fusion 360. تم الحفاظ على الأجسام منفصلة (Separate Bodies) دون دمجها لتسهيل عمليات التعديل والتطوير المستقبلي.

### 📸 صور النموذج الأولي (Visuals)

#### المنظور العلوي للروبوت
![منظور الروبوت العلوي](top_view.bmp)

#### المنظور الجانبي للروبوت
![منظور الروبوت الجانبي](side_view.bmp)

### 🛠️ المواصفات الميكانيكية والهيكلية
* **الهيكل الرئيسي:** صندوق متناظر مصمم بعناية لاستيعاب المكونات الإلكترونية والبطارية في المنتصف لضمان توازن مركز الجاذبية (Center of Mass).
* **الأرجل ودرجات الحرية (Legs & DOF):** تصميم يعتمد على مفصلين لكل رجل، بمجموع درجتي حرية (2-DOF) لكل رجل للحركة البندولية الفعالة، مما يجعل مجموع المفاصل الكلي للروبوت 4 مفاصل متحركة.
* **نظام الدفع والمحركات:** يعتمد التصميم الحالي على محركات سيرفو من نوع SG90 (عدد 4 محركات تثبت عند الفخذ/الحوض).
* **آلية توازن ديناميكي إضافية (ذيل خلفي):** تم دمج امتداد خلفي علوي (على شكل ذيل عقرب) كميزة تجريبية مبتكرة تعمل كثقل موازن ديناميكي (Dynamic Counterweight) للمساعدة في تعديل مركز الجاذبية ومنع الانقلاب أثناء الحركة البندولية للأرجل.

### 📊 الحسابات المبدئية والعزم (Torque Analysis)
لضمان قدرة المحركات على دعم جسم الروبوت أثناء الوقوف الثابت، تم حساب العزم المطلوب ($T$) عند مفصل الفخذ بناءً على المعادلة التالية:

$$T = F \times L$$

حيث أن:
* **القوة المؤثرة ($F$):** بفرض أن كتلة الروبوت التقريبية $M = 250\text{ g}$، وتتوزع بالتساوي على الأرجل عند الوقوف الثابت، فإن القوة لكل رجل تساوي تقريباً $0.125\text{ kg}$.
* **طول ذراع العزم ($L$):** طول الفخذ الممتد أفقياً يساوي $4\text{ cm}$.

**حساب العزم المطلوب:**
$$T = 0.125\text{ kg} \times 4\text{ cm} = 0.5\text{ kg.cm}$$

* **كفاءة المحرك:** يقدم محرك سيرفو SG90 عزماً أقصى يصل إلى $1.8\text{ kg.cm}$، وبمقارنته بالعزم المطلوب ($0.5\text{ kg.cm}$)، نجد أن المحرك كافٍ جداً وفيه عامل أمان (Safety Factor) ممتاز لدعم وزن الروبوت وديناميكية حركته.

### 🔄 آلية الحركة والاتزان المقترحة (Gait & Balance)
* **نمط المشي:** نمط الزحف الرباعي المستقر استاتيكياً (Static Crawl Gait) عن طريق تحريك رجل واحدة في كل خطوة، مما يضمن بقاء مركز الجاذبية دائماً داخل مثلث الدعم المكون من الثلاث أرجل الأخرى الملامسة للأرض.

### ⚠️ المشاكل الميكانيكية المتوقعة (Anticipated Mechanical Issues)
* **إجهاد تروس المحركات (Gear Stress):** نظراً لأن محركات SG90 تعتمد على تروس بلاستيكية، فإن الصدمات المباشرة مع الأرض أثناء المشي قد تؤدي إلى تآكل التروس أو كسرها مع الوقت.
* **انزلاق الأقدام (Foot Slippage):** تصميم الأقدام الحالي المصنوع من البلاستيك الصلب قد يسبب انزلاق الروبوت على الأسطح الناعمة، مما يخل بتوازنه أثناء نقل الخطوات.
* **اهتزاز الهيكل (Chassis Vibration):** غياب نظام امتصاص الصدمات قد ينقل الاهتزازات مباشرة إلى الهيكل الرئيسي والمكونات الإلكترونية.

### 🚀 الحلول والتطويرات المستقبلية (Future Enhancements)
* دمج نظام تعليق ميكانيكي مرن (Suspension System) لامتصاص الصدمات وحماية التروس.
* إضافة طبقة مطاطية أو آلية أقدام متدحرجة (Rolling Feet) أسفل الأرجل لزيادة الاحتكاك ومنع الانزلاق.

---

## 🇬🇧 2. English Version

This repository contains the initial mechanical design and kinematic analysis of a quadruped robot dog prototype, modeled using Autodesk Fusion 360. All parts have been kept as separate bodies (without combining) to allow flexible future modifications and development.

### 📸 Prototype Visuals

#### Top View
![Robot Top View](top_view.bmp)

#### Side View
![Robot Side View](side_view.bmp)

### 🛠️ Mechanical & Structural Specifications
* **Main Chassis:** A symmetrical body designed to house the electronics and battery in the center to maintain a stable Center of Mass (CoM).
* **Legs & Degrees of Freedom (DOF):** A 2-jointed leg design providing 2 Degrees of Freedom (2-DOF) per leg for efficient pendulum movement, totaling 4 active joints across the robot.
* **Actuators:** The current setup utilizes 4x SG90 micro servo motors mounted at the hip joints.
* **Active Counterweight (Tail Mechanism):** An upper rear extension (scorpion-tail style) was integrated as an innovative experimental feature to act as a dynamic counterweight. This mechanism helps dynamically shift the Center of Mass and enhance stabilization during walking gaits.

### 📊 Preliminary Torque Analysis
To ensure the actuators can support the robot during a static stand, the required torque ($T$) at the hip joint is calculated using the following equation:

$$T = F \times L$$

Where:
* **Acting Force ($F$):** Assuming the total estimated weight is $M = 250\text{ g}$, distributed evenly across the legs during a static stand, the force per leg is approximately $0.125\text{ kg}$.
* **Lever Arm ($L$):** The horizontal extension length of the thigh is $4\text{ cm}$.

**Torque Calculation:**
$$T = 0.125\text{ kg} \times 4\text{ cm} = 0.5\text{ kg.cm}$$

* **Actuator Capacity:** The SG90 micro servo provides a stall torque of up to $1.8\text{ kg.cm}$. Comparing this to the required torque ($0.5\text{ kg.cm}$), the actuator is highly capable and offers an excellent Safety Factor to support the robot's mass and dynamic movements.

### 🔄 Locomotion & Stability (Gait & Balance)
* **Gait Pattern:** Utilizes a statically stable **Static Crawl Gait**, moving one leg at a time to ensure the Center of Mass remains within the support triangle formed by the other three legs.

### ⚠️ Anticipated Mechanical Issues
* **Gear Stress & Backlash:** Since SG90 servos utilize plastic gears, direct ground impact forces during walking can lead to gear wear or stripping over time.
* **Foot Slippage:** The current rigid plastic foot design may cause slippage on smooth surfaces, disrupting the robot's balance during leg transitions.
* **Chassis Vibration:** The lack of a damping mechanism transmits ground impacts directly to the main chassis and electronic components.

### 🚀 Future Enhancements
* Integrating a mechanical suspension system for shock absorption to protect the servo gears.
* Adding a rubberized grip or a rolling-feet mechanism at the lower legs to increase traction and prevent slippage.
