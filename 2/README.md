# 有关html和body的一些点

## html和body的html的background属性(html会覆盖body的background属性)
1. html的background-color没设置，body的background-color设置，浏览器背景色取body [效果地址](https://sihai00.github.io/training-css/2/1-1.html)
```css
htlm{

}
body{
  background-color: red;
}
```

2. html和body同时设置background-color，浏览器背景色取html，body的背景色被覆盖 [效果地址](https://sihai00.github.io/training-css/2/1-2.html)
```css
htlm{
  background-color: green;
}
body{
  background-color: red;
}
```

## html和body的盒子属性
html和body都可以设置margin、padding、width、height(height: 100%很有用) [效果地址](https://sihai00.github.io/training-css/2/2-1.html)

```css
html{
  height: 100%;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
}
body{
  width: 100px;
  height: 100px;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
}
```

## html和body的定位属性 
绝对定位元素的相对最顶层元素是屏幕(viewport)[效果地址](https://sihai00.github.io/training-css/2/3-1.html)

```css
html{
  background-color: green;
}
body{
  background-color: red;
}
.test{
  position: absolute;
  top: 0;
  left: 0;
}
```

## 浏览器滚动条
最顶层的滚动条元素是html [效果地址](https://sihai00.github.io/training-css/2/4-1.html)

```css
html{
  background-color: green;
  overflow: auto;
}
body{
  background-color: red;
  overflow: hidden;
}
```
