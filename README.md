# iran-cities
Data of provinces and cities of Iran in the form of Jason file for Mongo.

<div dir="rtl">
  
# بانک اطلاعاتی شهر ها و استان های ایران برای دیتابیس مونگو

iran-cities بانک اطلاعاتی حاوی اخرین به روز رسانی ها و تقسیمات کشوری در استان ها و شهر ها است

![Divisions of Iran](/images/1008121-نقشه-جمهوری-اسلامی-ایران-با-استان-های-رنگی-در-رنگ-های-روشن.jpg)
    
تمامی شهر ها در این دستابیس با استان های شان در ارتباط هستند
    
    
# تاریخچه
این بانک را زمانی ایجاد کردم که در یک پروژه به تمامیه دیتا های شهر ها و استان های ایران در قالب یک جیسون برای پایگاه داده noSQL 
خودم نیاز داشتم اما هیچ جا نتونستم یه فرمت درست و رایگان و بهینه شده برای دیتابیس های noSQL پیدا کنم
    
    
- من با گرفتن یک شاخه از پروژه Ahmad Azizi یک دیتابیس با فرمت جیسون برای  noSql ساختم

به طور خلاصه اغلب بانک های موجود از روی چند منبع ناقص و قدیمی کپی شده بودند و دارای ایرادات فراوانی بودند.

این بانک تمام این اشکالات را برطرف کرده است و به طور کامل از روی آخرین داده های رسمی ایجاد گردیده است.



### ویژگی‌های جدید:
* فیلد amar_code به تمامی جداول اضافه شده است که یک کد منحصربه‌فرد مرکز آمار ایران برای هریک از تقسیمات کشوری می‌باشد.

اطلاعات تکمیلی مانند مختصات جغرافیایی برای کدهای آماری تاکنون به شکل آزاد توسط مرکز آمار ایران ارائه نشده است. 
**دسترسی به اطلاعات و آمار عمومی یک حق شهروندی است که متأسفانه علی‌رغم پیگیری‌های به عمل‌آمده، مرکز آمار ایران از ارائه آن سرباز می‌زند و مدارک آن هم موجود است.**

# نسخه ۲.۰
این نسخه به روز رسانی فروردین ۱۳۹۹ می باشد. پس از استخراج و پاکسازی داده ها، این نسخه شامل ۳۱ استان، ۴۳۴ شهرستان، ۱۰۷۱ بخش، ۲۶۰۱ دهستان، ۱۵۱۸ شهر و ۹۷۹۱۵ روستا(آبادی و آبادی بلوکه) می باشد. بدیهی است در صورت به روز رسانی آمار رسمی، نسخه جدید هم براساس آخرین داده ها به روزآوری خواهد شد.

همچنین این ویژگیها نسبت به نسخه قبلی افزوده شده اند:
- افزودن دهستان ها و روستاها(به تفکیک آبادی و آبادی-بلوکه مانند مرغداری ها و واحدهای صنعتی)
- افزودن نواحی شهری و شهرداری که در شهرهای بزرگ وجود دارد(مناطق شهرداری مثل تهران منطقه ۱، منطقه ۲ و ...)
- نام جداول از city, county, province به ostan, shahr و ... تغییر داده شده است.
    
# نسخه ۱.۰
این بانک براساس براساس آخرین تقسیمات کشوری تا پایان سال ۱۳۹۴ که توسط مرکز آمار ایران ارائه شده است ایجاد گردیده است. در زمان ایجاد این نسخه(فروردین ۱۳۹۶) این آخرین اطلاعات ارائه شده توسط مرکز آمار است که براساس آن  کشور ایران از ۳۱ استان، ۴۲۹ شهرستان، ۱۰۵۷ بخش، ۲۵۸۹ دهستان و ۱۲۴۵ شهر تشکیل یافته‌است. 
بدیهی است در صورت به روز رسانی آمار رسمی، نسخه جدید این بانک هم براساس آخرین داده ها به روزآوری خواهد شد.


# ساختار
ساختار فایل به بسیار ساده است یک کالکشن تحت عنوان cities وجود دارد که تمامی شهر ها درون ان قرار دارند
فایل دیگر states که ObjectId تمام شهر های مربوط به هر استان درون ان در یک ارایه قرار دارد



</div>

# License
MIT License

Created by Ahmad Azizi https://github.com/navidrezadoost/