# 响应式表格
在手机端表格往往是一个头痛的问题，按照bootstrap的响应式表格保持pc往往交互不好，这时可以尝试下把表格倒立
![表格](https://github.com/sihai00/training-css/blob/master/4/table1.png)

## bootstrap的响应式表格
![bootstrap的响应式表格](https://github.com/sihai00/training-css/blob/master/4/bootstrap.jepg)

## 倒立响应式表格
![bootstrap的响应式表格](https://github.com/sihai00/training-css/blob/master/4/table2.jepg)

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