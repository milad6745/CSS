
# CSS Border
```html
<!DOCTYPE html>
<html>
<head>
       <!-- لینک کردهhtmlدر اینجا فایل استایل رو به  -->
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.cdnfonts.com/css/persian" rel="stylesheet">
</head>
<body>
<p id="id1"> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nisi voluptatem suscipit doloribus harum, necessitatibus aliquam distinctio laboriosam molestiae, quam, ex dicta. Tempore excepturi placeat repudiandae veritatis soluta? Vel, temporibus nostrum. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nisi voluptatem suscipit doloribus harum, necessitatibus aliquam distinctio laboriosam molestiae, quam, ex dicta. Tempore excepturi placeat repudiandae veritatis soluta? Vel, temporibus nostrum.</p>
</body>
</html>
```
```css
#id1{
  /* رنگ بوردر */
    border-color: red;
    /* فاصله نوشته ها از بوردر */
    padding: 1cm;
    /* رنگ بکگراند داخلی بوردر */
    background-color: yellow;
    /* حداکثر میزان ارتفاع بوردر ، بیشترش  رو یا نمایش نده یا اسکرول کن  */
    max-height: 60px;
    /* عرض بوردر */
    width: 200px;
    /* استایل بوردر خط خط باشد */
    border-style: dashed;
        /* بعد از اینکه ماکس طولی بوردر پر شد اسکرول بده */
    overflow-y: scroll;
}
```
