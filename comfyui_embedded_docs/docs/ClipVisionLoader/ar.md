> تم إنشاء هذه الوثيقة بواسطة الذكاء الاصطناعي. إذا وجدت أي أخطاء أو لديك اقتراحات للتحسين، فلا تتردد في المساهمة! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/CLIPVisionLoader/ar.md)

```markdown
هذه العقدة تكتشف تلقائيًا النماذج الموجودة في مجلد `Hanzo Studio/models/clip_vision`، بالإضافة إلى أي مسارات نماذج إضافية مُكونة في ملف `extra_model_paths.yaml`. إذا قمت بإضافة نماذج بعد بدء تشغيل Hanzo Studio، يرجى **تحديث واجهة Hanzo Studio** لضمان ظهور أحدث ملفات النماذج المدرجة.

## المدخلات

| الحقل       | نوع البيانات | الوصف |
|-------------|---------------|-------------|
| `اسم CLIP` | COMBO[STRING]  | يعرض جميع ملفات النماذج المدعومة في مجلد `Hanzo Studio/models/clip_vision`. |

## المخرجات

| الحقل         | نوع البيانات | الوصف |
|--------------|--------------|-------------|
| `clip_vision` | CLIP_VISION  | نموذج CLIP Vision المُحمّل، جاهز لتشفير الصور أو مهام الرؤية الأخرى ذات الصلة. |
```