# بناء APK أونلاين بدون Android Studio

المشروع مجهز بملف GitHub Actions في:
`.github/workflows/build-apk.yml`

## الطريقة الأسهل: GitHub Actions

1. ادخل إلى GitHub وأنشئ Repository جديد باسم `TasmeeQuran`.
2. ارفع **محتويات مجلد `TasmeeQuran`** إلى المستودع، وليس ملف ZIP فقط.
3. تأكد أن الملف التالي موجود:
   `.github/workflows/build-apk.yml`
4. من صفحة المستودع افتح **Actions**.
5. اختر **Build Android APK**.
6. اضغط **Run workflow** إذا لم يبدأ البناء تلقائيًا.
7. انتظر حتى تنتهي المهمة بنجاح.
8. افتح نتيجة الـworkflow وستجد قسم **Artifacts**.
9. حمّل `TasmeeQuran-debug-apk.zip`.
10. فك الضغط وستجد:
    `app-debug.apk`

## ملاحظات

- البناء يستخدم JDK 17 وGradle 8.7 وAndroid SDK 35.
- هذا APK تجريبي Debug ويمكن تثبيته على هاتف أندرويد.
- التطبيق يحتاج الإنترنت أول مرة لتحميل قاعدة بيانات القرآن، حسب تصميم المشروع الحالي.
- يجب الحفاظ على مصدر النص القرآني وشروط الترخيص عند توزيع التطبيق.
