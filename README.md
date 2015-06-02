# Slider
基于jQuery幻灯模块

## 参数列表
```javascript
/**
 * @mod switchable
 * @tuthor zhw
 * @param 参数列表
 *     effect:          {String}    切换效果，默认为slide
 *     showNav:         {Boolean}   是否显示切换导航(0,1,2,3,4..)，默认为true
 *     showPage:        {Boolean}   是否显示翻页(next,prev)，默认为true
 *     animateSpeed:    {Number}    动画执行时间，默认为500
 *     interval:        {Number}    帧切换间隔时间，默认为2000
 *     restartDelay:    {Number}    停止后再次播放延迟时间，默认为2000
 *     pauseOnHover:    {Boolean}   鼠标hover时不否停止播放，默认为true
 *     loadImg:         {Boolean}   是否加载延迟图片(<img data-src="..." />)，默认为true
 *     autoPlay:        {Boolean}   是否自动播放
 *     transformFix:    {Boolean}   CSS3切换，目前未实现
 *     switchNavEvent:  {String}    切换导航(0,1,2,3,4..)事件类型，默认为click
 *     switchMainClass: {String}    切换项目Wrap类名，默认为switch_main
 *     switchItemClass: {String}    切换项目类名，默认为switch_item
 *     pageClass:       {String}    翻页Wrap类名，默认为switch_page
 *     pageItemClass:   {String}    翻页项类名，默认为switch_page_item
 *     navClass:        {String}    切换导航(0,1,2,3,4..)Wrap类名，默认为switch_nav
 *     navItemClass:    {String}    切换导航(0,1,2,3,4..)项类名，默认为switch_nav_item
 *     navCurrentClass: {String}    切换导航(0,1,2,3,4..)选中类名，默认为switch_nav_item_current
 *     mixClass:        {String}    切换图片项类名，默认为item，用于图片滚动切换中，未实现真正图片无缝滚动，利用mixClass组合凑整以幻灯形式切换
**/
```
## 快速开始
### 使用requireJS
```javascript
<script src="lib/require.js"></script>
<script>
require.config({
	paths: {
		'jquery': 'lib/jquery'
		,'switchable': 'lib/switchable'
	}
});
require(['jquery', 'switchable'], function($, switchable){
	switchable({$element: $('#slides')});
});
</script>
```
### 不使用requireJS
```javascript
<script src="lib/jquery.js"></script>
<script src="lib/switchable.js"></script>
<script>
switchable({$element: $('#slides')});
</script>
```
