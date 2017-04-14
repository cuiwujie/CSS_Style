# 按钮

为 &lt;a&gt;、&lt;button&gt;或 &lt;input&gt; 元素添加按钮类（button class）即可使用相应的样式。

## 基础样式
实例：
	
![](http://ooaehxyax.bkt.clouddn.com/default.png)

 	<a class="btn btn_default" href="#" role="button">Link</a>
    <button class="btn btn_default" type="submit">Button</button>
    <input class="btn btn_default" type="button" value="Input">
    <input class="btn btn_default" type="submit" value="Submit">

## 颜色
![](http://ooaehxyax.bkt.clouddn.com/%E9%A2%84%E5%AE%9A%E4%B9%89%E6%A0%B7%E5%BC%8F.png)

 	<!--颜色样式-->
    <button type="button" class="btn btn_default">（默认样式）Default</button>

    <button type="button" class="btn btn_primary">（首选项）Primary</button>

    <button type="button" class="btn btn_success">（成功）Success</button>

    <button type="button" class="btn btn_info">（一般信息）Info</button>

    <button type="button" class="btn btn_warning">（警告）Warning</button>

    <button type="button" class="btn btn_danger">（危险）Danger</button>

    <button type="button" class="btn btn_link">（链接）Link</button>

## 尺寸

![](http://ooaehxyax.bkt.clouddn.com/%E5%B0%BA%E5%AF%B8.png)

		<!--大小样式-->
        <button type="button" class="btn btn_primary btn_large">（大按钮）Large button</button>

        <button type="button" class="btn btn_primary btn_normal">（默认尺寸）Default button</button>

        <button type="button" class="btn btn_primary btn_small">（小按钮）Small button</button>

        <button type="button" class="btn btn_primary btn_xsmall">（超小尺寸）Extra small button</button>

## 激活禁用

![](http://ooaehxyax.bkt.clouddn.com/%E6%BF%80%E6%B4%BB%E7%A6%81%E7%94%A8%E7%8A%B6%E6%80%81.png)

  	<!--激活状态-->
    <button type="button" class="btn btn_default btn_large active">Button</button>
    <button type="button" class="btn btn_primary btn_large active">Button</button>
    <!--禁止使用-->
    <button type="button" class="btn btn_default btn_large" disabled="disabled">Button</button>
    <button type="button" class="btn btn_primary btn_large "disabled="disabled">Button</button>
    <button type="button" class="btn btn_success btn_large "disabled="disabled">Button</button>
    <button type="button" class="btn btn_info btn_large "disabled="disabled">Button</button>
    <button type="button" class="btn btn_warning btn_large "disabled="disabled">Button</button>
    <button type="button" class="btn btn_danger btn_large" disabled="disabled">Button</button>
    <button type="button" class="btn btn_link btn_large "disabled="disabled">Button</button>