
## 🛠️ أداة ApkPatcher (إصدار حميد)

**صنع في العراق 🇮🇶 - Made in Iraq**

---

### 💢 المتطلبات الأساسية (قبل ما تبدي) 💢
افتح تطبيق Termux واكتب ذني الأوامر بالسرّة حتى يشتغل عندك كلشي تمام:
1. termux-setup-storage
2. pkg update -y
3. pkg upgrade -y
4. pkg install python -y

---

### 📥 طريقة التثبيت
حتى تثبت أداة ApkPatcher، اختار أي طريقة تعجبك من ذني الأوامر:

👉 **الطريقة الأولى (التثبيت المباشر):**
pip install --force-reinstall https://github.com/TechnoIndian/ApkPatcher/archive/refs/heads/main.zip

أو استعمل هذا الكود:
curl -Ls https://github.com/TechnoIndian/Tools/releases/download/Tools/ApkPatcher.sh | bash

👉 **الطريقة الثانية (عن طريق Git):**
pkg install python git && pip install git+https://github.com/TechnoIndian/ApkPatcher.git

❌ **إذا ردت تمسح الأداة نهائياً:**
pip uninstall ApkPatcherX

---

### ⚙️ شلون تستخدم الأداة (أمثلة)

الأداة تشتغل بنظام (Input Mode) يعني تنطيها مسار التطبيق وهي تعدل عليه. الشغل التلقائي مالتها هو تخطي الـ VPN والـ SSL.

* **الأمر الأساسي:**
  ApkPatcher -i اسم_تطبيقك.apk

* **استخدام APKEditor بدل APKTool:**
  ApkPatcher -i app.apk -a

* **دمج شهادة الفحص (Certificate):**
  ApkPatcher -i app.apk -c مسار_الشهادة.pem

* **تخطي حماية تطبيقات Flutter:**
  ApkPatcher -i app.apk -f

* **تخطي حماية Pairip (يفضل تشغله بـ VM أو تطبيق متعدد):**
  ApkPatcher -i app.apk -p

* **تغيير الـ Android ID (تخطي قفل الجهاز الواحد):**
  ApkPatcher -i app.apk -D 7e9f51f096bd5c83

* **تخطي كشف البكج (Spoofing):**
  ApkPatcher -i app.apk -pkg

* **تفعيل ميزات الشراء والمدفوع (Premium):**
  ApkPatcher -i app.apk -P

* **تخطي منع تصوير الشاشة (Anti-Screenshot):**
  ApkPatcher -i app.apk -rmss

* **تخطي كشف تصحيح الـ USB (USB Debugging):**
  ApkPatcher -i app.apk -rmusb

* **حذف الإعلانات من التطبيق:**
  ApkPatcher -i app.apk -rmads

* **تعديل تطبيقات التليجرام و Plus:**
  ApkPatcher -i app.apk -t

---

### 🖇️ نظام الدمج (Merge Mode)
إذا عندك تطبيق مقسم (مثل .apks أو .xapk) وتريد تجمعه بملف APK واحد عادي:
ApkPatcher -m اسم_الملف.apks

---

### 📋 أوامر المساعدة
* **للمساعدة:** ApkPatcher -h
* **لمعرفة باقي الإضافات:** ApkPatcher -O
* **للحقوق:** ApkPatcher -C

---
**ملاحظة من حميد:** أهلاً وسهلاً بيكم، هذا الشغل لخدمتكم 🇮🇶.
