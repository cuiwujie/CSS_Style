# 栅格系统

栅格系统用于通过一系列的行（row）与列的组合来创建页面布局，你的内容就可以放入这些创建好的布局中。

1. 通过“行（row）”在水平方向创建一组“列”。
2. 你的内容应当放置于“列”内，并且，只有“列”可以作为行（row）”的直接子元素。
3. 类似 .row 和 .xsmall_4 这种预定义的类，可以用来快速创建栅格布局。 源码中定义的 mixin 也可以用来创建语义化的布局。
4. 栅格类适用于与屏幕宽度大于或等于分界点大小的设备 ， 并且针对小屏幕设备覆盖栅格类。 因此，在元素上应用任何 .medium_6* 栅格类适用于与屏幕宽度大于或等于分界点大小的设备 ， 并且针对小屏幕设备覆盖栅格类。 因此，在元素上应用任何 .large_3* 不存在， 也影响大屏幕设备。

# 媒体查询


	
	/* 小屏幕（平板，大于等于 768px） */
	@media (min-width: @screen-small-min) { ... }
	
	/* 中等屏幕（桌面显示器，大于等于 992px） */
	@media (min-width: @screen-medium-min) { ... }
	
	/* 大屏幕（大桌面显示器，大于等于 1200px） */
	@media (min-width: @screen-large-min) { ... }

# 栅格参数

 ![](http://ooaehxyax.bkt.clouddn.com/%E6%A0%85%E6%A0%BC%E5%8F%82%E6%95%B0.png)

# 实例  流式布局容器

![](http://ooaehxyax.bkt.clouddn.com/%E5%AE%9E%E4%BE%8B.png)

代码：
                                   
    <div class="row show-grid">
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
        <div class="medium_1">.medium_1</div>
    </div>
    <div class="row show-grid">
        <div class="medium_8">.medium_8</div>
        <div class="medium_4">.medium_4</div>
    </div>
    <div class="row show-grid">
        <div class="medium_4">.medium_4</div>
        <div class="medium_4">.medium_4</div>
        <div class="medium_4">.medium_4</div>
    </div>
    <div class="row show-grid">
        <div class="medium_6">.medium_6</div>
        <div class="medium_6">.medium_6</div>
    </div>
    
   
# 实例：移动设备和桌面屏幕

![](http://ooaehxyax.bkt.clouddn.com/%E7%A7%BB%E5%8A%A8%E8%AE%BE%E5%A4%87%E5%92%8C%E6%A1%8C%E9%9D%A2%E5%B1%8F%E5%B9%95.png)

	<!-- Stack the columns on mobile by making one full-width and the other half-width -->
	<div class="row show-grid">
	    <div class="xsmall_12 medium_8">.xsmall_12 .medium_8</div>
	    <div class="xsmall_6 medium_4">.xsmall_6 .medium_4</div>
	</div>
	
	<!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
	<div class="row show-grid">
	    <div class="xsmall_6 medium_4">.xsmall_6 .medium_4</div>
	    <div class="xsmall_6 medium_4">.xsmall_6 .medium_4</div>
	    <div class="xsmall_6 medium_4">.xsmall_6 .medium_4</div>
	</div>
	
	<!-- Columns are always 50% wide, on mobile and desktop -->
	<div class="row show-grid">
	    <div class="xsmall_6 medium_6">.xsmall_6 .medium_6</div>
	    <div class="xsmall_6 medium_6">.xsmall_6 .medium_6</div>
	</div>

# 实例：手机、平板、桌面

![](http://ooaehxyax.bkt.clouddn.com/%E6%89%8B%E6%9C%BA%E3%80%81%E5%B9%B3%E6%9D%BF%E3%80%81%E6%A1%8C%E9%9D%A2.png)

	
	<div class="row show-grid">
	    <div class="small_12 medium_8">.small_12 .medium_6 .medium_8</div>
	    <div class="small_6 medium_4">.small_6 .medium_4</div>
	</div>
	<div class="row show-grid">
	    <div class="xsmall_6 small_4">.xsmall_6 .small_4</div>
	    <div class="xsmall_6 small_4">.xsmall_6 .small_4</div>
	    <!-- Optional: clear the XS cols if their content doesn't match in height -->
	    <div class="clearfix visible-xs-block"></div>
	    <div class="xsmall_6 medium_4">.xsmall_6 .medium_4</div>
	</div>

# 多余的列（column）将另起一行排列
![](http://ooaehxyax.bkt.clouddn.com/%E5%A4%9A%E4%BD%99%E5%9B%9E%E9%80%80.png)


	<div class="row show-grid">
	    <div class="xsmall_9">.xsmall_9</div>
	    <div class="xsmall_4">.xsmall_4<br>Since 9 + 4 = 13 &gt; 12, this 4-column-wide div gets wrapped onto a new line as one contiguous unit.</div>
	    <div class="xsmall_6">.xsmall_6<br>Subsequent columns continue along the new line.</div>
	</div>


# 列偏移
![](http://ooaehxyax.bkt.clouddn.com/%E5%88%97%E5%81%8F%E7%A7%BB.png)


	
	<div class="row show-grid">
	    <div class="medium_4">medium_4</div>
	    <div class="medium_4 medium_offset-4">medium_4 medium_offset-4</div>
	</div>
	<div class="row show-grid">
	    <div class="medium_3 medium_offset-3 ">medium_3 medium_offset-3</div>
	    <div class="medium_3 medium_offset-3 ">medium_3 medium_offset-3</div>
	</div>
	<div class="row show-grid">
	    <div class="medium_6 medium_offset-3">medium_6 medium_offset-3</div>
	</div>


# 嵌套列
![](http://ooaehxyax.bkt.clouddn.com/%E5%B5%8C%E5%A5%97%E5%88%97.png)


	<div class="row show-grid">
	    <div class="small_9">
	        Level 1: .small_9
	        <div class="row show-grid">
	            <div class="xsmall_8 small_6">
	                Level 2: xsmall_8 .small_6
	            </div>
	            <div class="xsmall_4 small_6">
	                Level 2: .xsmall_4 .small_6
	            </div>
	        </div>
	    </div>
	</div>


# 列排序

![](http://ooaehxyax.bkt.clouddn.com/%E5%88%97%E6%8E%92%E5%BA%8F.png)

	<div class="row show-grid">
	    <div class="medium_9 medium_left-3">.medium_9 .medium_right-3</div>
	    <div class="medium_3 medium_right-9">.medium_3 .medium_right-9</div>
	</div>