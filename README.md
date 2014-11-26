# 响应式Web设计实践

## 简介

*作者：Tim Kadlec*

*[豆瓣主页](http://book.douban.com/subject/21263576/)*



> 唯有响应式设计是最近似于银弹的子弹

## 无处不在的Web

- 设备：Android，iPhone，Nook，iPad，Kindle，XBox 360， Wii，

	> 最好的浏览器就是你手里那个
	
- 屏幕尺寸：512x342，1024x768，320x480，280-1920，
- 网速：EDGE，3G，LTE
- 标准支持程度：
- 输入方式：键盘鼠标，滚动球，触控版，手势（滑动，下拉，拖动...）
- 使用环境：
- 解决方案1：为每种设备创建独立的站点
- 解决方案2：成为**响应式**的站点

	> [Responsive Web Design by Ethan Marcotte in 2010-05](http://alistapart.com/d/responsive-web-design/ex/ex-site-FINAL.html), at "A List Apart"
	
	- 媒介查询，Media queries
	- 流动布局，Fluid grids
	- 自适应图片，Scalable images
	
	> 与设备无关
	
- 渐进增强 vs 优雅降级

## 流动布局

- 4种常见的布局：
	- 固定布局：960px是使用最广泛的宽度。
	- 流体布局：百分比单位，页面可变。
	- 弹性布局：通常以em为单位。1em相当于当前字体的大小。
	- 混合布局
	
- 字体大小
	- 像素px：
	- em：em值 = 目标/上下文环境，级联的
	- 百分比：解决IE兼容em问题
	- rem：root em，非级联
	
- 网格布局
	- 从内容出发：遗留图片，广告iAB
	- 9列网格：9 * 84 + 24 * 8 = 948px + 2 * 6 = 960px
	- 表格布局：
	- 为IE7及以下提供备用样式 
	
## 媒介查询

- 视口 viewport

	` <head><meta name="viewprot" content="directive, directive"></head>`
	
- 缩放 user-scalable = no

	` <mate name="viewport" content="initial-scale=1, width=device-width" /> `
	
- 媒介查询

	` @media [not | only] type [and] (expr) { rules }`
	
	- all, screen, print
	- width, height, device-width, device-height, orientation, aspect-ratio
	- and, not, or, only
	
- 内嵌样式，or外链样式
- 媒介查询顺序：建议采用从移动端向上的设计思路

	

	
