# 居中
文字、图片居中方法

## 水平居中
1.inline元素或者inline-block元素
```css
.parent{
  text-align: center
}
```

2.block元素
```css
.son{
  margin: 0 auto
}
```

## 垂直居中
1.inline元素
```css
.parent{
  line-height: 20px;
}
```

2.inline-block元素
```css
.parent{
  line-height: 100px;
}
.son{
  vertical-align: middle;
}
```

## 水平垂直居中
1.table
```css
.parent{
  display: table;
  text-align: center;
  vertical-align: middle;
}
```

2.position + margin、transform、calc(元素自身宽度的一半)
```css
.son{
  width: 20px;
  height: 20px;
  position: absolute;
  
  // margin 方法
  margin-left: -10px;
  margin-top: -10px;
  
  // transform 方法
  transform: translate3d(-50%, -50%, 0);
  
  // calc 方法
  left: calc(50% - 10px);
  top: calc(50% - 10px);
}
```

3.position + margin:auto
```css
.son{
  width: 20px;
  height: 20px;
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  margin: auto;
}
```

4.flex
```css
.parent{
  display: flex;
  justify-content: space-between;
  align-tiems: center;
}
```