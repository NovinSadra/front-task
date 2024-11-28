
# **ساخت فروشگاه آنلاین چندزبانه با استفاده از Fake Store API**

### **توضیحات کلی:**

یک اپلیکیشن وب بسازید که داده‌ها را از Fake Store API دریافت کرده و به کاربران نمایش دهد. این اپلیکیشن باید به زبان‌های فارسی و انگلیسی قابل تغییر باشد و به طور کامل در محیط واقعی قابل استفاده باشد.

#### **ویژگی‌ها و چالش‌ها:**

###### 1. *صفحه اصلی (UI و طراحی):*
-   صفحه اصلی باید شامل یک لیست محصولات از Fake Store API باشد.
-   هر محصول باید شامل ویژگی‌های زیر باشد:
-   تصویر محصول
-   نام محصول
-   قیمت محصول
-   دکمه‌ای برای مشاهده جزئیات بیشتر
-   طراحی باید با استفاده از Vue.js 3 و Tailwind CSS یا Vuetify انجام شود. صفحه باید ریسپانسیو و مناسب برای موبایل باشد.
-   یک منوی ناوبری برای تغییر زبان (فارسی/انگلیسی) و دسترسی به بخش‌های مختلف اپلیکیشن (مانند صفحه جزییات محصول) باید وجود داشته باشد.
.

###### 2. *چندزبانه کردن اپلیکیشن:*

-   اپلیکیشن باید به طور داینامیک به دو زبان فارسی و انگلیسی قابل تغییر باشد.
-   برای این کار از Vue I18n یا یک ابزار مشابه برای ترجمه متون در اپلیکیشن استفاده کنید.
-   تمامی متون در اپلیکیشن (منوها، دکمه‌ها، عنوان‌ها و پیام‌ها) باید به دو زبان ترجمه شوند.
-   هنگام تغییر زبان، تمامی محتوای اپلیکیشن باید به زبان جدید بارگذاری شود (ترجمه متون، تغییر فرمت تاریخ‌ها و اعداد در صورت نیاز).

###### 3. *دریافت داده‌ها از Fake Store API:*

-   استفاده از Fake Store API برای دریافت لیست محصولات.
-   Endpoint مورد استفاده:  [https://fakestoreapi.com/products](https://fakestoreapi.com/products "https://fakestoreapi.com/products")
-   داده‌های دریافتی باید در اپلیکیشن به نمایش درآید. از Axios یا Fetch API برای انجام درخواست‌های HTTP استفاده کنید.
-   برای هر محصول، اطلاعات آن باید به صورت داینامیک از API دریافت و در قالب مناسب نمایش داده شود.

  

###### 4. *صفحه جزئیات محصول:*

-   هنگامی که کاربر بر روی یک محصول کلیک می‌کند، باید به یک صفحه جزئیات محصول منتقل شود.
-   این صفحه باید شامل اطلاعات کامل محصول مانند تصویر بزرگ، توضیحات محصول، قیمت، و دکمه‌ای برای بازگشت به صفحه اصلی باشد.
-   این داده‌ها باید با استفاده از Vue Router بارگذاری شوند.

  

###### 5. *فیلتر کردن محصولات:*

-   به صفحه اصلی یک بخش فیلتر اضافه کنید که به کاربران این امکان را بدهد که محصولات را بر اساس دسته‌بندی و قیمت فیلتر کنند.
-   فیلتر دسته‌بندی‌ها و قیمت‌ها باید به صورت داینامیک بارگذاری شوند.
-   هنگام فیلتر کردن محصولات، وضعیت محصولات باید به طور خودکار به روزرسانی شود.

  

#### **نکات فنی:**

-   استفاده از SOLID principles برای نوشتن کد تمیز و قابل نگهداری.
-   کد باید با Git مدیریت شود. یک README شامل توضیحات پروژه، نحوه نصب و اجرا، و نحوه استفاده از API بنویسید.



#### **چالش‌های اضافی (اختیاری برای امتیاز اضافی):**

-   از Nuxt.js برای پیاده‌سازی Server-Side Rendering (SSR) استفاده کنید.
-   اپلیکیشن را به گونه‌ای طراحی کنید که SEO-friendly باشد.
-   بهینه‌سازی اپلیکیشن برای عملکرد بهتر، از جمله کش کردن داده‌ها برای بارگذاری سریع‌تر.
-   اگر آشنایی با تست‌نویسی دارید، تست‌های واحد (Unit Tests) برای بخش‌های مختلف اپلیکیشن بنویسید (مثلاً برای درخواست‌های API، مدیریت وضعیت و نمایش داده‌ها).
-   از Pinia برای مدیریت وضعیت داده‌ها استفاده کنید:  وضعیت لیست محصولات باید در Pinia ذخیره شود و هنگامی که کاربر زبان را تغییر می‌دهد یا فیلتر جدیدی اعمال می‌کند، این وضعیت باید به روز رسانی شود. یک حالت بارگذاری (Loading State) برای نمایش در زمان دریافت داده‌ها از API ایجاد کنید.
-   - 

### مدت زمان انجام تمرین بین 4 تا 7 روز است
 جواب تسک (بدون پوشه module) را به صورت زیپ به ایمیل من ارسال کنید.

آدرس ایمیل
a.khosravi@newcash.me
