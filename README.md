<div align="center">
  <h1>🎣 MikroTik Hunter v5</h1>
  <p><b>أداة متقدمة وهندسية لاصطياد وتحليل بوابات تسجيل الدخول لشبكات MikroTik.</b></p>
  <p><i>Developed by <a href="https://github.com/PMoha1">PMoha1</a></i></p>
</div>

---

## 👁️ نظرة عامة (Overview)
أداة **MikroTik Hunter** هي بيئة عمل هجومية تعمل بالكامل داخل المتصفح (Client-Side). تم تصميمها خصيصاً للتعامل مع بوابات تسجيل الدخول (Hotspot/Captive Portals) لشبكات مايكروتيك وتجاوز القيود الافتراضية.

## 🚀 التشغيل السريع (Quick Start)
تعمل الأداة بكفاءة عالية وبشكل مباشر على أغلب الشبكات. بعد تحميل الأداة وفتحها، كل ما عليك فعله هو إدخال الرابط الأساسي لصفحة تسجيل الدخول في الواجهة الرئيسية، وستقوم الأداة بالباقي.

## ⚡ بيئة الهجوم وتجاوز CORS
بما أن الأداة ترسل طلبات مباشرة إلى بوابات خارجية، يجب تخطي حماية **CORS** (Cross-Origin Resource Sharing) على مستوى المتصفح لتعمل كبيئة استهداف مفتوحة.
**💡 ملاحظة:** أوامر تشغيل المتصفح المعزول (بدون قيود الأمان) متوفرة داخل **إعدادات الأداة** وقابلة للنسخ المباشر بضغطة زر!

### 🐧 تشغيل البيئة على Linux
```bash
google-chrome --disable-web-security --user-data-dir=/tmp/hunter_session /path/to/hunter.html
```

### 🪟 تشغيل البيئة على Windows
```cmd
chrome.exe --disable-web-security --user-data-dir="C:\hunter_session" "C:\path\to\hunter.html"
```

---

## 💀 التسليح المتقدم: الهندسة العكسية للمسارات (Advanced Weaponization)
للمهندسين والمحترفين، للحصول على أقصى استقرار وأفضل نتيجة هجومية، يجب استخراج مسارات الشبكة الدقيقة (Endpoints) بالهندسة العكسية وحقنها في قسم **الإعدادات المتقدمة (Advanced Settings)** داخل الأداة:

1. **تجهيز التنصت:** افتح صفحة تسجيل الدخول للشبكة الهدف، واضغط `F12` لفتح أدوات المطور (Developer Tools)، ثم انتقل لتبويب **Network**. قم بتفعيل خيار `Preserve log`.
2. **التقاط رابط الدخول (Login URL):** قم بإدخال كرت شبكة صحيح وسجل الدخول. راقب طلب الـ `POST` الذي يرسل البيانات للخادم، وانسخ الرابط الدقيق للطلب.
3. **التقاط رابط الحالة (Status URL):** بعد الدخول، سيبدأ المتصفح بإرسال طلبات للتحقق من الرصيد والوقت المتبقي. انسخ رابط هذا الطلب.
4. **التقاط رابط الخروج (Logout URL):** اضغط على زر "تسجيل الخروج"، وانسخ رابط الطلب الذي يقوم بإنهاء الجلسة.
5. **الحقن النهائي:** عد إلى الأداة، افتح **الإعدادات المتقدمة**، وألصق الروابط الثلاثة في الحقول المخصصة لها لتسليح الأداة بأعلى دقة.

---

## 🎬 التطبيق العملي (Video Tutorial)
*(سيتم إرفاق رابط فيديو الشرح العملي لعمليات الهندسة العكسية قريباً...)*

---

<div align="center">
  <b>PMoha1 | Offensive AI & Hardware Hacker</b><br>
  <a href="https://youtube.com/@PMoha1"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" /></a>
  <a href="https://github.com/PMoha1"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</div>
