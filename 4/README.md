# 响应式表格
在手机端表格往往是一个头痛的问题，按照bootstrap的响应式表格保持pc往往交互不好，参考了[响应式表格](http://lea.verou.me/2018/05/responsive-tables-revisited/)这时可以尝试下把表格倒立

## bootstrap的响应式表格
![表格](https://github.com/sihai00/training-css/blob/master/4/table1.png)
![bootstrap的响应式表格](https://github.com/sihai00/training-css/blob/master/4/bootstrap.jpeg)

## 倒立响应式表格
![表格](https://github.com/sihai00/training-css/blob/master/4/table1.png)
![bootstrap的响应式表格](https://github.com/sihai00/training-css/blob/master/4/table2.jpeg)

代码如下
```css
@media (max-width: 600px) {
  .my-table, .my-table tbody{
    display: flex;
  }
  .my-table tbody{
    overflow: scroll;
  }
  .my-table th, .my-table td{
    display: block;
  }
}
```