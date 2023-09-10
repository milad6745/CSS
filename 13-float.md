## Float
`float` یک ویژگی در CSS است که برای تعیین چگونگی قرارگیری المان‌ها در کنار یکدیگر استفاده می‌شود. وقتی یک المان به `float` تنظیم می‌شود، آن المان از جریان معمول مستندات (Document Flow) خارج می‌شود و در چپ یا راست المان مادرش یا المان قبلی قرار می‌گیرد.

یک مثال ساده:

HTML:

```html
<div class="left-box">محتوای چپ</div>
<div class="right-box">محتوای راست</div>
```

CSS:

```css
.left-box {
  float: left;
  width: 50%;
}

.right-box {
  float: right;
  width: 50%;
}
```
![image](https://github.com/milad6745/CSS/assets/113288076/40cd87fb-1395-41ed-b962-481815b59445)



در این مثال، دو `div` داریم. اولین `div` که کلاس `.left-box` دارد، به چپ شناور شده و عرض آن ۵۰٪ از عرض والدین خود را دارد. دومین `div` که کلاس `.right-box` دارد، به راست شناور شده و همچنین ۵۰٪ از عرض والدین خود را دارد.

با این ترتیب، این دو المان کنار هم قرار می‌گیرند. توجه داشته باشید که ممکن است نیاز به تنظیمات اضافی (مانند `clear`) داشته باشید تا مشکلاتی که احتمالاً با `float` همراه می‌شوند را حل کنید.


## Clear

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>مثال ساده و زیبا</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="id1"></div>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quae quam vitae magnam ipsum sequi exercitationem veritatis temporibus cupiditate voluptatum, atque ducimus esse delectus veniam. Ab rerum voluptatum voluptatibus officia dolorem!</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident cupiditate optio placeat laudantium. Asperiores quisquam libero aut quaerat laboriosam commodi quae pariatur. Architecto nam nulla consequatur. Incidunt dolor praesentium veniam.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium veritatis possimus eos libero accusamus tempora inventore vero, animi numquam dignissimos assumenda natus quo eaque, sequi mollitia, ratione consequatur officiis magnam!</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis sunt dolorem iusto quidem quia atque mollitia culpa deserunt iste porro facere fugiat repudiandae sed illum, obcaecati natus ullam alias. Adipisci?</p>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Facere iste blanditiis mollitia amet temporibus dolores. Distinctio pariatur dolore inventore unde totam itaque rerum aut quia laudantium. Cupiditate doloribus eius commodi.</p>
</body>
</html>
```
```
#id1{
    width: 5cm;
    height: 5cm;
    background-color: blue;
    float: right;

}

p{
    font-size:larger;
    clear:none;
}
```
در این حالت به موردی که شناور تعریف شده واکنس نشان میدهد
![image](https://github.com/milad6745/CSS/assets/113288076/798c8e3e-e1b9-4d30-9c21-d69f9bed531f)

 clear:both;
در این حالت بعد از شناور اومده و پاراگراف را ایجاد کرده است

![image](https://github.com/milad6745/CSS/assets/113288076/8e75f621-4af5-433b-bd3a-626cb9e63309)
