<div dir="rtl">

# تطوير موقع إدارة محتوى

### الشيفرة المصدرية لتطبيق موقع إدارة محتوى من دورة "تطوير تطبيقات الويب باستخدام PHP" المقدمة من أكاديمية حسوب

<a href="https://academy.hsoub.com/learn/php-web-application-development/">دورة تطوير تطبيقات الويب باستخدام  PHP</a>

# خطوات تشغيل المشروع

* إنشاء ملف باسم `env.` في المسار الأساسي للمشروع
* تعبئة الملف `env.` بالبيانات، و نستطيع نسخ هذه البيانات من الملف `env.example.` ولصقها بداخل الملف `env.` و التعديل عليها
* تغيير اسم قاعدة البيانات في الملف `env.` باسم مشابه تمامًا لقاعدة البيانات التي أنشأناها
* نهجر الجداول إلى قاعدة البيانات ونعبئها بالمعلومات من `البذور` بتنفيذ الأمر:

<h6 dir="ltr">

`php artisan migrate --seed`

</h6>

* لكي تُعرض الصور في المشروع يجب علينا إنشاء رابط link بتنفيذ الأمر:
<h6 dir="ltr">

`php artisan storage:link`

</h6>

* إنشاء الحزم اللازمة لتشغيل المشروع بتنفيذ الأمر:
<h6 dir="ltr">

`composer install`

</h6>

<h6 dir="ltr">

`npm install`

</h6>
* بعدها ننفذ الأمر:
<h6 dir="ltr"> 

`php artisan key:generate`

</h6>

* نستخدم في المشروع نظام الإشعارات باستخدام pusher لذلك لضبط إعداداته من ملف `env.`

<h6 dir="ltr">

`BROADCAST_DRIVER=pusher`<br>
`PUSHER_APP_ID=`<br>
`PUSHER_APP_SECRET=`<br>
`PUSHER_APP_KEY=`<br>
`PUSHER_APP_SECRET=`<br>
`PUSHER_APP_CLUSTER=`<br>

</h6>

* الآن أصبح المشروع جاهز للتشغيل ننفذ الأمر:

<h6 dir="ltr">

`php artisan serve`

</h6>

* ننسخ الرابط الذي ظهر ونلصقه بالمتصفح.

</div>