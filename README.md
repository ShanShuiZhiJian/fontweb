<html lang="en"><head>
    <meta charset="UTF-8">
    <title></title>
<style id="system" type="text/css">h1,h2,h3,h4,h5,h6,p,blockquote {    margin: 0;    padding: 0;}body {    font-family: "Helvetica Neue", Helvetica, "Hiragino Sans GB", Arial, sans-serif;    font-size: 13px;    line-height: 18px;    color: #737373;    margin: 10px 13px 10px 13px;}a {    color: #0069d6;}a:hover {    color: #0050a3;    text-decoration: none;}a img {    border: none;}p {    margin-bottom: 9px;}h1,h2,h3,h4,h5,h6 {    color: #404040;    line-height: 36px;}h1 {    margin-bottom: 18px;    font-size: 30px;}h2 {    font-size: 24px;}h3 {    font-size: 18px;}h4 {    font-size: 16px;}h5 {    font-size: 14px;}h6 {    font-size: 13px;}hr {    margin: 0 0 19px;    border: 0;    border-bottom: 1px solid #ccc;}blockquote {    padding: 13px 13px 21px 15px;    margin-bottom: 18px;    font-family:georgia,serif;    font-style: italic;}blockquote:before {    content:"C";    font-size:40px;    margin-left:-10px;    font-family:georgia,serif;    color:#eee;}blockquote p {    font-size: 14px;    font-weight: 300;    line-height: 18px;    margin-bottom: 0;    font-style: italic;}code, pre {    font-family: Monaco, Andale Mono, Courier New, monospace;}code {    background-color: #fee9cc;    color: rgba(0, 0, 0, 0.75);    padding: 1px 3px;    font-size: 12px;    -webkit-border-radius: 3px;    -moz-border-radius: 3px;    border-radius: 3px;}pre {    display: block;    padding: 14px;    margin: 0 0 18px;    line-height: 16px;    font-size: 11px;    border: 1px solid #d9d9d9;    white-space: pre-wrap;    word-wrap: break-word;}pre code {    background-color: #fff;    color:#737373;    font-size: 11px;    padding: 0;}@media screen and (min-width: 768px) {    body {        width: 748px;        margin:10px auto;    }}</style><style id="custom" type="text/css"></style></head>
<body marginheight="0"><h1>开发报告</h1>
<pre><code>*5.21日我参加了学校的摇滚音乐节，便被其中的魅力所吸引，这天学校也举行了十佳歌手，而且回顾杭电的历史，
学校出了几个音乐名人，摇滚巨星郑钧，流行歌手刘瑞琦，还有其他做音乐的人，学校的音乐资源比较丰富，做一个
音乐类的网站也符合实际。
*期望的效果：目前是先把网站的主体做出来，有个大体效果，最后随着本人技术的提升，再进行完善。
*内容来源：图片来源于自己参加此类的活动，音频和视频就是在网上找。</code></pre>
<h2>1.关于首页</h2>
<h3>导航栏</h3>
<pre><code>* 主要运用了a标签，其中用a:hover伪类和padding来调节a标签的背景效果。</code></pre>
<h3>轮播图</h3>
<pre><code>*引入了jequary插件。</code></pre>
<h3>div主体</h3>
<pre><code>*首先设置了一个大的div来控制主体内容，里面逃了一个div（居中），其里面还有三个小的div里面是页面的新闻简介。</code></pre>
<h3>footer</h3>
<pre><code> *每个优秀的网站都会介绍自己的网站主题的地址，我的也不例外。</code></pre>
<h2>2.音乐新闻</h2>
<h3>导航栏</h3>
<pre><code>*导航栏和主页的保持一致</code></pre>
<h3>右边侧边栏</h3>
<pre><code>*右边一个小的导航栏，更便于了浏览</code></pre>
<h3>主体div</h3>
<pre><code>*文章的主题部分</code></pre>
<h2>3.十佳歌手</h2>
<pre><code>*主要用一些css动画来展示动画效果，这也是一个技术难点</code></pre>
<h2>4.自我介绍</h2>
<h1>开发工具</h1>
<pre><code>*主要是Dreamweaver还有sublime</code></pre>
<h1>开发心得</h1>
<pre><code>*通过对web前端这门课的学习，让我更加了解了网页以及网站的制作技术，学了一个学期的课程然后在制作自己的网站过程中使用所
学的知识那真是一件很美妙的事，而且还和同学室友们一起讨论其中的一些技术难点。由于我在设计之初想的是建立一个大的音乐网
站，但后来参加了一次要摇滚音乐节，对于学校的音乐资源感觉有许多地方值得利用，鉴于此我制作了关于学校的音乐网站。我本人
喜欢弹吉他，慢慢的音乐和吉他渗透在了我的生活里，总之有一件自己喜欢的事是那么美好有趣。</code></pre>
<h1>开发难点1、</h1>
<pre><code>.port-1{float: left; width: 100%; position: relative; overflow: hidden; text-align: center; border: 4px solid rgba(255, 255, 255, 0.9);}
.port-1 .text-desc{opacity: 0.9; top: -100%; transition: 0.5s; color: #000; padding: 45px 20px 20px;}
.port-1 img{transition: 0.5s;}
.port-1:hover img{transform: scale(1.2);}

.port-1.effect-1:hover .text-desc{top: 0;}

.port-1.effect-2 .text-desc{top: auto; bottom: -100%;}
.port-1.effect-2:hover .text-desc{bottom: 0;}

.port-1.effect-3 .text-desc{top: 50%; left: 50%; width: 0; height: 0; overflow: hidden; padding: 0;}
.port-1.effect-3:hover .text-desc{width: 100%; top: 0; left: 0; height: 100%; padding: 45px 20px 20px;}</code></pre>
<h1>开发难点2、</h1>
<pre><code>设立了多个div，所以就要不断地进行调试</code></pre>
<h1>开发难点3、</h1>
<pre><code>image.onload = function() {
var pattern = context.createPattern(image, "no-repeat");
context.arc(110, 110, 80, 0, 2 * Math.PI);
context.fillStyle = pattern;
context.fill();    
};</code></pre>
</body></html>