# 有关html\body的一些点

## html\body的html的background属性(html会覆盖body的background属性)
1. html的background-color没设置，body的background-color设置，浏览器背景色取body [效果地址](./1-1.html)
```css
htlm{

}
body{
  width: 100px;
  height: 100px;
  background-color: red;
}
```

2. html和body同时设置background-color，浏览器背景色取html，body的背景色被覆盖 [效果地址](./1-2.html)
```css
htlm{
  background-color: green;
}
body{
  width: 100px;
  height: 100px;
  background-color: red;
}
```

## html\body的盒子属性
html\body都可以设置margin、padding、width、height(height: 100%很有用) [效果地址](./2-1.html)

```css
html{
  height: 100%;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
  background-color: green;
}
body{
  width: 100px;
  height: 100px;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
  background-color: red;
}
```

## html\body的定位属性 
绝对定位元素的相对最顶层元素是屏幕(viewport)[效果地址](./3-1.html)

```css
html{
  background-color: green;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
  height: 100%;
}
body{
  background-color: red;
  width: 100px;
  height: 100px;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
}
.test{
  width: 100px;
  height: 100px;
  background-color: blue;
  position: absolute;
  top: 0;
  left: 0;
}
```

## 浏览器滚动条
最顶层的滚动条元素是html [效果地址](./4-1.html)

```css
html{
  background-color: green;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
  height: 150%;
  /*overflow: hidden;*/
  overflow: auto;
}
body{
  background-color: red;
  width: 100px;
  height: 100px;
  margin: 20px;
  padding: 20px;
  border: 20px solid #000;
  /*overflow: scroll;*/
  overflow: hidden;
}
```
