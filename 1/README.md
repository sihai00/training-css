# 文字内容溢出省略号表示

## 单行
1. text-overflow:ellipsis; [效果地址](http://dabblet.com/gist/13716404926363eb756a76ebdb1cc68b)

```css
width:50px;
overflow:hidden;  
text-overflow:ellipsis;
```

## 多行
1. -webkit-line-clamp(但只使用于webkit浏览器) [效果地址](http://dabblet.com/gist/5301008ffebb6f237267a28b45266e07)

```css
width: 100px;
overflow: hidden;
display: -webkit-box;    
-webkit-line-clamp: 3;    
-webkit-box-orient: vertical;
```

2. 伪元素实现 [效果地址](http://dabblet.com/gist/33a4ea34e2507af389740e5a2c4d3db7)

```css
.a{
  width: 100px;
  overflow: hidden;
  position: relative;
}
.a::after{
  content: '...';
  position: absolute;
  bottom: 0;
  right: 0;
  transform: translateX(-100%);
  background: linear-gradient(to right, transparent, #000 40%)
}
```