اگر از Chromebook استفاده نمی‌کنید می‌توانید [از این بخش ](http://tutorial.djangogirls.org/en/installation/#install-python) عبور کنید. اگر از آن استفاده می‌کنید تجربه نصب شما کمی متفاوت خواهد بود. شما می توانید بقیه دستورالعمل نصب را نادیده بگیرید.

### IDE ابری (PaizaCloud Cloud IDE, AWS Cloud9)

IDE ابری ابزاری است که به شما دسترسی به یک ویرایشگر کد و یک کامپیوتر در حال کار کردن روی اینترنت را می‌دهد که می‌توانید نصب، نوشتن و اجرای برنامه‌ها را در آن انجام دهید. در زمان این آموزش، IDE ابری به عنوان * دستگاه محلی شما * عمل خواهد کرد. شما همچنان مانند سایر همکلاسی‌ها که از OS X، اوبونتو یا ویندوز استفاده می‌کنند، دستورات را در ترمینال اجرا خواهید کرد اما ترمینال شما به کامپیوتری که IDE ابری برای شما آماده کرده متصل است. در اینحا دستورالعمل استفاده از IDE های ابری (PaizaCloud Cloud IDE و AWS Cloud9) را خواهید دید. شما می‌توانید یکی از IDE های ابری را انتخاب کنید و دستورالعمل را دنبال کنید.

#### IDE ابری PiazaCloud

1. به [PaizaCloud Cloud IDE](https://paiza.cloud/) بروید
2. یک حساب کاربری بسازید
3. بر روی *New Server* کلیک کنید
4. دکمه Terminal را (در سمت چپ صفحه) بزنید

حالا شما باید صفحه ای با یک ستون کناری و کلیدهایی در سمت چپ ببینید. بر روی دکمه "Terminal" کلیک کنید تا پنجره ترمینال با پیغامی شبیه به این باز شود:

{% filename %}Terminal{% endfilename %}

    $
    

ترمینال در IDE ابری PiazaCloud برای دستورات شما آماده شده است. شما می‌توانید اندازه این پنجره را تغییر دهید تا کمی بزرگتر دیده شود.

#### AWS Cloud9

1. به [AWS Cloud9](https://aws.amazon.com/cloud9/) بروید
2. یک حساب کاربری بسازید
3. *Create Environment* را کلیک کنید

حالا شما باید یک صفحه با یک ستون کناری، یک پنجره اصلی بزرگ به همراه مقداری نوشته و یک پنجره کوچک در پایین، شبیه به این ببینید:

{% filename %}bash{% endfilename %}

    yourusername:~/workspace $
    

این پنجره پایینی ترمینال شما است. شما می‌توانید برای فرستادن دستورات به کامپیوتر Cloud9 از این پنجره استفاده کنید. با تغییر اندازه این پنجره می‌توانید آن را کمی بزرگتر ببینید.

### محیط مجازی

یک محیط مجازی (Virtual Environment یا virtualenv) شبیه یک جعبه شخصی است که ما می‌توانیم کدهای کامپیوتری مربوط به یک پروژه را در آن جمع کنیم. ما از آن‌ها استفاده می‌کنیم تا تکه‌های مختلف کدهای هر پروژه را جدا از پروژه دیگر نگه داریم تا بین پروژه‌ها تداخل پیش نیاید.

در ترمینال پایین صفحه Cloud9 دستور زیر را اجرا کنید:

{% filename %}Cloud 9{% endfilename %}

    sudo apt update 
    sudo apt install python3.6-venv
    

اگر این دستور کار نکرد از مربی خود کمک بگیرید.

بعد، دستور زیر را اجراکنید:

{% filename %}Cloud 9{% endfilename %}

    mkdir djangogirls 
    cd djangogirls
     python3.6 -mvenv myvenv 
    source myvenv/bin/activate 
    pip install django~={{ book.django_version }}
    

(توجه کنید که در خط آخر ما از یک علامت مد و یک مساوی استفاده کردیم: `~=`).

### GitHub

یک حساب [گیت هاب](https://github.com) ایجاد کنید.

### PythonAnywhere

تمرین جنگو گرلز شامل بخشی است که به آن انتشار یا Deployment، می‌گوییم که در این فرایند کد مربوط به وب اپلیکیشن را به یک کامپیوتر در دسترس و عمومی (به نام سرور) منتقل می‌کنیم تا سایرین بتوانند کار شما را ببینند.

اگر تمرین را بر روی یک Chromebook انجام می‌دهید ممکن است این بخش کمی عجیب باشد به خاطر اینکه ما از یک کامپیوتر بر روی اینترنت استفاده می‌کنیم (بر خلاف یک لپ تاپ). با این‌حال، استفاده از Cloud 9 به عنوان یک محیط کاری برای کارهای در جریان و استفاده از Python Anywhere به عنوان یک فضای معرفی و نمایش پروژه هایی که در طول زمان کامل می‌شوند، مفید است.

یک حساب کاربری در [www.pythonanywhere.com](https://www.pythonanywhere.com) ایجاد کنید.