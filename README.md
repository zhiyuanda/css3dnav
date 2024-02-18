# HTML+CSS案例展示(CSS3d效果导航栏)
>  参考来源：
>
> [黑马程序员pink老师前端入门教程，零基础必看的h5(html5)+css3+移动端前端视频教程_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV14J4114768?p=390&spm_id_from=pageDriver)

# 网页如下（CSS3d效果导航栏）：

https://zhiyuanda.github.io/css3dnav/

# 网页代码如下：

### HTML+CSS：

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>css3dphoto</title>
    <style>
        * {
            margin: 0;
            padding: 0;
        }
        body {
            perspective: 500px;
        }
        ul {
            margin: 100px auto;
            width: 1200px;

        }
        ul li {
            float: left;

            margin: 0 20px;
            width: 160px;
            height: 60px;
            line-height: 50px;
            text-align: center;
            list-style: none;

        }
        .box {
            position: relative;
            width: 100%;
            height: 100%;
            transform-style: preserve-3d;
            transition: all .6s;
        }
        .box:hover {
            transform: rotateX(90deg);
        }
        .front,
        .back {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            color: #fff;
        }
        .front {
            background-color: pink;
            z-index: 1;
            transform: translateZ(30px);
        }
        .back {
            background-color: skyblue;
            transform: translateY(30px) rotateX(-90deg);
        }
    </style>
</head>
<body>
    <ul>
        <li>
            <div class="box"><div class="front">1</div>
            <div class="back">2</div></div>
            
        </li>
        <li>
            <div class="box"><div class="front">3</div>
            <div class="back">4</div></div>
            
        </li>        
        <li>
            <div class="box"><div class="front">5</div>
            <div class="back">6</div></div>
            
        </li>       
        <li>
            <div class="box"><div class="front">7</div>
            <div class="back">8</div></div>
            
        </li>        
        <li>
            <div class="box"><div class="front">9</div>
            <div class="back">10</div></div>
            
        </li>        
        <li>
            <div class="box"><div class="front">11</div>
            <div class="back">12</div></div>
            
        </li>
    </ul>
</body>
</html>
```

