---
title: Quickstart
permalink: /docs/
redirect_from:
  - /docs/home/
  - /docs/quickstart/
  - /docs/extras/
---

Jekyll هو أداة لإنشاء المواقع الساكنة (Static Site Generator). يقوم البرنامج بأخذ النصوص المكتوبة بلغة الترميز المفضلة لديك واستخدام قوالب التخطيط (layouts) لإنشاء موقع ويب ساكن. يمكنك تعديل مظهر الموقع وطابعه العام، وعناوين URL، والبيانات المعروضة على الصفحة، والمزيد.

## المتطلبات الأساسية

يتطلب Jekyll ما يلي:

*   إصدار Ruby رقم **{{ site.data.ruby.min_version }}** أو أحدث
*   RubyGems
*   GCC و Make

راجع قسم [المتطلبات]({{ '/docs/installation/#requirements' | relative_url }}) للاطلاع على الأدلة والتفاصيل.

## التعليمات

1.  ثبّت جميع [المتطلبات الأساسية]({{ '/docs/installation/' | relative_url }}).
2.  ثبّت حزم (gems) كل من jekyll و bundler.
```sh
gem install jekyll bundler
```
3.  أنشئ موقع Jekyll جديداً في المسار `./myblog`.
```sh
jekyll new myblog
```
4.  انتقل إلى المجلد الجديد.
```sh
cd myblog
```
5.  قم ببناء الموقع وإتاحته على خادم محلي.
```sh
bundle exec jekyll serve
```
6.  تصفح الموقع عبر الرابط [http://localhost:4000](http://localhost:4000){:target="_blank"}

{: .note .warning}
إذا كنت تستخدم الإصدار 3.0.0 أو أحدث من Ruby، فقد تفشل الخطوة رقم 5 [في العمل](https://github.com/github/pages-gem/issues/752). يمكنك إصلاح ذلك بإضافة `webrick` إلى قائمة الاعتمادات (dependencies) الخاصة بك: `bundle add webrick`

{: .note .info}
مرّر الخيار `--livereload` إلى الأمر `serve` ليتم تحديث الصفحة تلقائياً مع كل تغيير تجريه على الملفات المصدرية: `bundle exec jekyll serve --livereload`


إذا واجهت أي أخطاء أثناء هذه العملية، فتأكد من تثبيت جميع المتطلبات المذكورة في قسم [المتطلبات]({{ '/docs/installation/#requirements' | relative_url }}).
إذا استمرت المشكلات، راجع قسم [استكشاف الأخطاء وإصلاحها]({{ '/docs/troubleshooting/#configuration-problems' | relative_url }}). {: .note .info}
تختلف عملية التثبيت باختلاف نظام التشغيل لديك. راجع [أدلتنا]({{ '/docs/installation/#guides' | relative_url }}) للاطلاع على التعليمات الخاصة بكل نظام تشغيل.
