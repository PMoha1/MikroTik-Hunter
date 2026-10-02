<div align="center">
  <h1>🎣 MikroTik Hunter v5</h1>
  <p><b>أداة متقدمة وهندسية لاصطياد وتحليل بوابات تسجيل الدخول لشبكات MikroTik.</b></p>
  <p><i>Developed by <a href="https://github.com/PMoha1">PMoha1</a></i></p>
</div>

---

## 👁️ نظرة عامة (Overview)

أداة **MikroTik Hunter** هي بيئة عمل هجومية تعمل بالكامل داخل المتصفح (Client-Side). تم تصميمها خصيصاً للتعامل مع بوابات تسجيل الدخول (Hotspot/Captive Portals) لشبكات مايكروتيك وتجاوز القيود الافتراضية.

تتيح لك الأداة استخراج، حقن، واختبار مسارات تسجيل الدخول، مع تخطي حماية **CORS** على مستوى المتصفح لضمان حرية إرسال الطلبات (Requests) واستقبال الاستجابات (Responses) دون قيود.

---

## ⚡ كيفية التشغيل وتجاوز حماية CORS

بما أن الأداة ترسل طلبات مباشرة إلى بوابات خارجية، فإن المتصفحات تمنع ذلك افتراضياً بسبب سياسة الـ **CORS** (Cross-Origin Resource Sharing).
لتخطي هذه الحماية وجعل المتصفح يعمل كبيئة استهداف مفتوحة، يجب تشغيل المتصفح بهذه الأوامر:

### 🐧 على أنظمة Linux (Arch / CachyOS)
قم بفتح الطرفية (Terminal) وتشغيل متصفح Chrome أو Chromium باستخدام الأعلام (Flags) التالية:
```bash
google-chrome --disable-web-security --user-data-dir=/tmp/hunter_session /path/to/hunter.html
```
*(ملاحظة: سيتم إنشاء بيئة متصفح معزولة تماماً خالية من قيود الأمان لضمان عمل الأداة بسلاسة).*

### 🪟 على أنظمة Windows
افتح نافذة موجه الأوامر (CMD) أو (Run) واكتب:
```cmd
chrome.exe --disable-web-security --user-data-dir="C:\hunter_session" "C:\path\to\hunter.html"
```

---

## 🎯 استخراج روابط تسجيل الدخول وحقنها

لجعل الأداة قادرة على التفاعل مع شبكات MikroTik، يجب استخراج مسار تسجيل الدخول الصحيح للشبكة المستهدفة:

1. **الاستخراج (Extraction):**
   - اتصل بالشبكة المستهدفة (بدون إنترنت).
   - افتح المتصفح وسيتم توجيهك إلى صفحة الدخول تلقائياً (مثال: `http://10.0.0.1/login`).
   - انسخ رابط الصفحة (URL) بالكامل.

2. **الحقن (Injection):**
   - افتح ملف `hunter.html` عبر المتصفح (الذي تم تشغيله بدون CORS).
   - قم بإدخال الرابط المستخرج في الحقل المخصص في واجهة الأداة.
   - ستقوم الأداة الآن بتوجيه الهجمات/الطلبات إلى هذا الرابط واستقبال الردود مباشرة بفضل تخطي قيود الـ CORS.

---


<div align="center">
  <b>PMoha1 | Offensive AI & Hardware Hacker</b><br>
  <a href="https://youtube.com/@PMoha1"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" /></a>
  <a href="https://github.com/PMoha1"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</div>
