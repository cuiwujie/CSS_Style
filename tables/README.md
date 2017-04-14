# table

为任意 <table> 标签添加 .table 类可以为其赋予基本的样式 — 少量的内补（padding）和水平方向的分隔线。

![](http://ooaehxyax.bkt.clouddn.com/%E5%9F%BA%E7%A1%80%E6%A0%B7%E5%BC%8F.png)

	<table class="table">
            <thead>
            <tr class="active">
                <th>#</th>
                <th>Make</th>
                <th>Model</th>
                <th>Year</th>
            </tr>
            </thead>
            <tbody>
                <tr>
                    <td>1</td>
                    <td>Honda</td>
                    <td>Accord</td>
                    <td>2009</td>
                </tr>
                <tr>
                    <td>2</td>
                    <td>Toyota</td>
                    <td>Camry</td>
                    <td>2012</td>
                </tr>
                <tr>
                    <td>3</td>
                    <td>Hyundai</td>
                    <td>Elantra</td>
                    <td>2010</td>
                </tr>
            </tbody>
        </table>

## 条纹状表格

通过 .table_striped 类可以给 <tbody> 之内的每一行增加斑马条纹样式。

>跨浏览器兼容性
>条纹状表格是依赖 :nth-child CSS 选择器实现的，而这一功能不被 Internet Explorer 8 支持。

![](http://ooaehxyax.bkt.clouddn.com/%E6%9D%A1%E7%BA%B9%E7%8A%B6.png)


		<table class="table table_striped">
            <thead>
            <tr class="active">
                <th>#</th>
                <th>Make</th>
                <th>Model</th>
                <th>Year</th>
            </tr>
            </thead>
            <tbody>
            <tr>
                <td>1</td>
                <td>Honda</td>
                <td>Accord</td>
                <td>2009</td>
            </tr>
            <tr>
                <td>2</td>
                <td>Toyota</td>
                <td>Camry</td>
                <td>2012</td>
            </tr>
            <tr>
                <td>3</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            </tbody>
        </table>


## 带边框的表格
添加 .table_bordered 类为表格和其中的每个单元格增加边框。

![](http://ooaehxyax.bkt.clouddn.com/%E5%B8%A6%E8%BE%B9%E6%A1%86%E7%9A%84%E8%A1%A8%E6%A0%BC.png)

		<table class="table table_bordered">
            <thead>
            <tr class="active">
                <th>#</th>
                <th>Make</th>
                <th>Model</th>
                <th>Year</th>
            </tr>
            </thead>
            <tbody>
            <tr>
                <td>1</td>
                <td>Honda</td>
                <td>Accord</td>
                <td>2009</td>
            </tr>
            <tr>
                <td>2</td>
                <td>Toyota</td>
                <td>Camry</td>
                <td>2012</td>
            </tr>
            <tr>
                <td>3</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            </tbody>
        </table>

## 鼠标悬停

通过添加 .table_hover 类可以让 <tbody> 中的每一行对鼠标悬停状态作出响应。

![](http://ooaehxyax.bkt.clouddn.com/%E9%BC%A0%E6%A0%87%E6%82%AC%E5%81%9C.png)

	<table class="table table_hover">
            <thead>
            <tr class="active">
                <th>#</th>
                <th>Make</th>
                <th>Model</th>
                <th>Year</th>
            </tr>
            </thead>
            <tbody>
            <tr>
                <td>1</td>
                <td>Honda</td>
                <td>Accord</td>
                <td>2009</td>
            </tr>
            <tr>
                <td>2</td>
                <td>Toyota</td>
                <td>Camry</td>
                <td>2012</td>
            </tr>
            <tr>
                <td>3</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            </tbody>
        </table>

## 状态类
通过这些状态类可以为行或单元格设置颜色。
![](http://ooaehxyax.bkt.clouddn.com/%E8%A1%A8%E8%AF%86.png)

![](http://ooaehxyax.bkt.clouddn.com/%E7%8A%B6%E6%80%81%E7%B1%BB.png)

	<table class="table ">
            <thead>
            <tr class="active">
                <th>#</th>
                <th>Make</th>
                <th>Model</th>
                <th>Year</th>
            </tr>
            </thead>
            <tbody>
            <tr class="active">
                <td>1</td>
                <td>Honda</td>
                <td>Accord</td>
                <td>2009</td>
            </tr>
            <tr class="success">
                <td>2</td>
                <td>Toyota</td>
                <td>Camry</td>
                <td>2012</td>
            </tr>
            <tr class="info">
                <td>3</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            <tr class="warning">
                <td>4</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            <tr class="danger">
                <td>5</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            <tr>
                <td>6</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            </tbody>
        </table>

## 响应式表格
将任何 .table 元素包裹在 .table_responsive 元素内，即可创建响应式表格，其会在小屏幕设备上（小于768px）水平滚动。当屏幕大于 768px 宽度时，水平滚动条消失。

![](http://ooaehxyax.bkt.clouddn.com/%E5%93%8D%E5%BA%94%E5%BC%8F%E8%A1%A8%E6%A0%BC.png)

	<div class="table_box table_responsive">
        <table class="table ">
            <thead>
            <tr class="active">
                <th>#</th>
                <th>Make</th>
                <th>Model</th>
                <th>Year</th>
            </tr>
            </thead>
            <tbody>
            <tr>
                <td>1</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            <tr>
                <td>2</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            <tr>
                <td>3</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            <tr>
                <td>4</td>
                <td>Hyundai</td>
                <td>Elantra</td>
                <td>2010</td>
            </tr>
            </tbody>
        </table>
    </div>