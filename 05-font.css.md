## External Font
مثال:

```html

<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.cdnfonts.com/css/persian" rel="stylesheet">
</head>
<body>
<p id="id1"> تست فونت فارسی </p>
</body>

</html>

```

 شما می‌توانید این کد لینک را به قسمت `<head>` اسناد HTML خود اضافه کنید.

 حالا می‌توانید از این فونت در قوانین CSS خود استفاده کنید. برای مثال:

```css
.id1{
    font-family: 'Persian', sans-serif;
}

```

در این مثال، ما از فونت "persian" که با استفاده از لینک فراهم شده است، در المان `body` استفاده کردیم. اگر مرورگر اجازه داشته باشد،
این روش برای اضافه کردن فونت‌های خارجی به وبسایت‌های شما بسیار راحت است و امکان دارد فونت‌های زیبا و متنوعی را به پروژه‌های وب خود اضافه کنید.

## internal font @font-face

استفاده از `@font-face` در CSS به شما امکان می‌دهد تا فونت‌های سفارشی خود را به وبسایت خود اضافه کنید و از آنها در قوانین CSS استفاده کنید. این روش بسیار مفید است زمانی که می‌خواهید از فونت‌هایی که در سیستم کاربران شما ممکن است وجود نداشته باشند، استفاده کنید. این نحوه استفاده از `@font-face` به صورت زیر است:

 ابتدا فایل فونت خود را بارگیری کنید (معمولاً در فرمت‌های مانند TTF یا OTF). به نام‌های مختلف فونت دقت کنید و فرمت‌های مختلف فونت را از دستگاه‌های مختلف برای پشتیبانی بهینه استفاده کنید.

 سپس فایل فونت را در دایرکتوری مناسب برای پروژه خود قرار دهید و مطمئن شوید که می‌توانید به آن دسترسی داشته باشید.

 در CSS خود، از `@font-face` برای تعریف فونت استفاده کنید. به عنوان مثال:


```css
/* font face create by name irannastaliq */
/* و مسیرش را هم با یو آر ال میدهیم*/
@font-face{
    font-family: "IranNastaliq";
    src: url(font/IranNastaliq.ttf)
}

/* در اینجا در قسمت پاراگذاف فونت مربوطه را صدا میزنیم */
p{
    font-family: "IranNastaliq";
    font-size: 12px;
}

```

```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.cdnfonts.com/css/persian" rel="stylesheet">
</head>
<body>
<p> تست فونت فارسی </p>
</body>

</html>
```
![image](https://github.com/milad6745/CSS/assets/113288076/7e4c1db0-d06f-4bc9-bcaf-2abc39cdf998)
