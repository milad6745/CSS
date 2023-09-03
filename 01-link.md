در CSS، عبارت "استفاده از `link`" به معنای اضافه کردن یک پیوند (link) به یک فایل CSS خارجی در صفحه HTML شما می‌باشد. این عمل به شما امکان می‌دهد تا استایل‌های تعریف شده در فایل CSS خارجی را در صفحه HTML خود استفاده کنید. بدین ترتیب، می‌توانید استایل‌های مشترک را برای چندین صفحه وب یا تمام صفحات وب خود به اشتراک بگذارید.

برای اضافه کردن یک فایل CSS خارجی به صفحه HTML، از عنصر `<link>` استفاده می‌کنید. این عنصر باید در بخش `<head>` اسناد HTML شما قرار گیرد. روش عمومی برای اضافه کردن فایل CSS به صفحه HTML به این صورت است:

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
  <!-- محتویات صفحه HTML -->
</body>
</html>
```

در اینجا:

- `<link>`: از عنصر `link` برای ایجاد یک پیوند به فایل CSS استفاده می‌کنیم.
- `rel="stylesheet"`: این ویژگی نشان می‌دهد که این پیوند به یک فایل CSS مرتبط است.
- `type="text/css"`: این ویژگی نوع محتوای پیوند را تعیین می‌کند که در اینجا متن CSS است.
- `href="styles.css"`: این ویژگی مسیر (URL) به فایل CSS خارجی را مشخص می‌کند. شما باید مسیر فایل CSS خود را در اینجا قرار دهید.

با افزودن این پیوند (`link`) به صفحه HTML، محتوای فایل CSS خارجی (`styles.css` در مثال بالا) در صفحه HTML شما اعمال می‌شود و می‌توانید از کلاس‌ها و تعریف‌های استایل موجود در آن استفاده کنید تا ظاهر صفحه HTML خود را سفارشی کنید.


## Example

```html
<!DOCTYPE html>
<html>
<head>
       <!-- لینک کردهhtmlدر اینجا فایل استایل رو به  -->
    <link rel="stylesheet" href="style.css">
</head>
<body>
<p> Random number generation is a process by which, often by means of a random number generator, a sequence of numbers or symbols that cannot be reasonably predicted better than by random chance is generated.</p>
</body>

</html>
```
در اینجا مشخصات فایل اعم از اندازه رنگ پیکسی و .. را گفته که به فایل اصلی مان لینک شده است .
```css
p{
    text-align: center;
    font-size: 20px;
    color: blue;
    background-color: lightgray;
    padding: 20px;
    width: 300px;
}
```
![image](https://github.com/milad6745/CSS/assets/113288076/9a8e4f39-1871-4175-9795-e6b15a3dd6c2)
