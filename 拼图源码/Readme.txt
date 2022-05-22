
2012-5-10

演示了HTML5中SVG与CANVAS结合的功能，利用SVG PATH接收复杂区域的用户输入，而CANVAS作为高效的画布进行图片的显示
主要技术：
动态生成包含贝塞尔曲线的SVG路径字符串
正则表达式解析SVG PATH字符串，并等效的进行CANVAS CLIP
拖动和旋转，通过转换矩阵做到SVG与CANVAS的同步11

7-4
针对IE9+，使用page-画布的offset（如果有嵌套则需要循环），而不是offsetXY

			if( Sys.ie == null) //For FireFox/Chrome/Safari
			{
				cx = ev.originalEvent.layerX;
				cy = ev.originalEvent.layerY;
			}	
			else //For IE9
			{
				cx = ev.originalEvent.pageX - canvas.offsetLeft;
				cy = ev.originalEvent.pageY - canvas.offsetTop;

			}

或者都统一到page - canvas的offsetLeft，而不使用layer（推荐）

顺便增加几个简单的声音效果

HTML5拼图游戏代码+图片不规则

现在HTML5大热，但看了很多介绍，都是重点介绍CANVAS而相对忽略了SVG，我个人感觉这两个技术结合，优势互补，利用SVG的交互性和CANSVAS的绘图能力，才能更好地发挥各自的作用。

以前用纯SVG做到一个拼图的DEMO，现在改为SVG和CANVAS，花了一个星期的时间，重写了这个例子，在CHROME17和FF12中进行了测试。比纯SVG速度快。

一直看好SVG，但由于种种原因，包括浏览器是否支持等等，没有得到广泛的应用。在HTML5的框架内，SVG能够发挥自己应有的威力了吧？