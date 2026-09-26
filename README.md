# A Piece, A Story — حكاية قطعة

A static, dependency-free WebGL museum with a walkable gallery, 360-degree camera, touch/keyboard movement, 20 exhibits, and Arabic, English and Urdu content.

## Run
Serve `dist/` from any static HTTP server. No build or credentials are required. JavaScript modules require HTTP rather than file URLs.

## Navigation
Drag to look around; hold the on-screen arrows or WASD/arrow keys to walk. Select an exhibit or use the collection strip. The detail card provides story, origin, Islamic meaning, a question and linked sources. “Walk to this object” relocates the visitor next to its display. Browser-provided text-to-speech is available only when the selected language has an installed voice.

## Content and visual provenance
All 20 exhibit illustrations are AI-generated educational representations. They are NOT photographs, scans or exact replicas of accessioned objects. Their atlas was generated for this project; decorative writing must not be treated as readable scripture. The room is a fictional museum, not a reconstruction of an existing institution.

Historical examples refer to the primary collection records linked in each card, including The Metropolitan Museum of Art and the Khalili Collections. Quran and hadith references are linked separately. Generic object types have no invented maker, date or owner. Hypothetical scenes are marked as such. Content and translations have not received professional religious or linguistic review.

## Boundaries
This version provides curated content and fixed questions, not a live generative chatbot. It requires no API key and sends no visitor prompts to an AI service. Exhibit representations are images inside a genuinely three-dimensional gallery, not scanned 3D artifact models. Language preference is stored only on the visitor’s device. Institutional or competition use needs specialist review and any additional required AI service.

## Source layout
- dist/index.html: museum interface
- dist/style.css: responsive Arabic/English/Urdu layout
- dist/engine.js: WebGL gallery, picking and navigation
- dist/app.js: exhibit interactions, language selection and narration
- dist/data.js: 20 objects, three languages, primary reference links
- dist/artifacts.png: educational object atlas

No external runtime CDN dependencies. Static hosting manifest is in .openai/hosting.json.

## دليل عربي مختصر

«حكاية قطعة» متحف تعليمي تفاعلي يعرض 20 قطعة في قاعة ثلاثية الأبعاد، بالعربية والإنجليزية والأوردية.

### التشغيل محليًا

يتطلب الأمر التالي Python 3 مثبتًا. من مجلد المشروع شغّلي:

```sh
python3 -m http.server 8000 --directory dist
```

ثم افتحي `http://localhost:8000` في المتصفح. لا تفتحي ملف HTML مباشرة؛ ملفات JavaScript تستخدم الوحدات.

### التوثيق

- [المصادر لكل قطعة وحدود الاستدلال](SOURCES.md)
- [نسبة المحتوى والصور وحالة الترخيص](ATTRIBUTIONS.md)

### ملاحظة حول التسليم

يجب أن يكون رابط الكود المطلوب للمسابقة رابط مستودع GitHub عامًا بعد إنشائه على حساب صاحبة المشروع. رابط الموقع ورابط مستودع استضافة Sites لا يقومان مقام رابط GitHub. لا تُرفَع أي بيانات دخول أو مفاتيح سرية.
