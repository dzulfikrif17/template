<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html lang='en' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>

<head>
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async='async' src='https://www.googletagmanager.com/gtag/js?id=UA-123036359-1'/>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag(&#39;js&#39;, new Date());

  gtag(&#39;config&#39;, &#39;UA-123036359-1&#39;);
</script>

<!-- MaterialMix 1.0 -->
<!-- Meta content -->
<meta expr:charset='data:blog.encoding'/>
<meta content='blogger' name='generator'/>
<meta content='summary_large_image' name='twitter:card'/>
<b:if cond='data:blog.url == data:blog.homepageUrl'>
	<meta content='blog' property='og:type'/>
<b:elseif cond='data:blog.pageType == &quot;item&quot;'/>
	<meta content='article' property='og:type'/>
</b:if>

<!-- Adding Canonical URL -->
<meta expr:content='data:blog.canonicalUrl' property='og:url'/>
<meta expr:content='data:blog.canonicalUrl' name='twitter:url'/>
<!-- Link rel=canonical -->
<link expr:href='data:blog.canonicalUrl' rel='canonical'/>

<!-- Scalable device -->
<meta content='width=device-width, initial-scale=1, user-scalable=no' name='viewport'/>
<meta content='blogger' name='generator'/>



<!--  Meta keywords -->
<b:if cond='data:blog.metaDescription'>
	<meta expr:content='data:blog.metaDescription' property='og:description'/>
	<meta expr:content='data:blog.metaDescription' name='description'/>
	<meta expr:content='data:blog.metaDescription' name='twitter:description'/>
<b:else/>
	<b:if cond='data:blog.url == data:blog.homepageUrl'>
		<meta expr:content='data:blog.metaDescription' property='og:description'/>
		<meta expr:content='data:blog.metaDescription' name='description'/>
		<meta expr:content='data:blog.metaDescription' name='twitter:description'/>
	</b:if>
</b:if>

<meta content='materialmix, material blogger template, material blogger theme, material design' name='keywords'/>

<!-- Adding follow Robots to post and index only -->
<b:if cond='data:blog.pageType == &quot;archive&quot;'>
	<meta content='noindex,nofollow' name='robots'/>
<b:else/>
	<b:if cond='data:blog.pageType == &quot;error_page&quot;'>
		<meta content='noindex,nofollow' name='robots'/>
	<b:else/>
		<b:if cond='data:blog.pageType == &quot;index&quot;'>
			<b:if cond='data:blog.homepageUrl == data:blog.url'>
				<meta content='index,follow' name='robots'/>
				<meta content='noodp' name='robots'/>
			<b:else/>
				<meta content='noindex,nofollow' name='robots'/>
			</b:if>
		<b:else/>
			<meta content='index,follow' name='robots'/>
			<meta content='noodp' name='robots'/>
		</b:if>
	</b:if>
</b:if>

<!-- Optimizing the post -->
<b:if cond='data:blog.pageType == &quot;item&quot;'>
	<!-- La primera imagen del post -->
	<b:if cond='data:blog.postImageThumbnailUrl'>
		<link expr:href='data:blog.postImageThumbnailUrl' rel='image_src'/>
		<meta expr:content='resizeImage(data:blog.postImageThumbnailUrl, 800)' name='twitter:image'/>
		<meta expr:content='resizeImage(data:blog.postImageThumbnailUrl, 800)' property='og:image'/>
	</b:if>

	<!-- The Navigation -->
	<b:if cond='data:blog.newerPageUrl'>
		<link expr:href='data:blog.newerPageUrl' rel='next'/>
	<b:elseif cond='data:blog.olderPageUrl'/>
		<link expr:href='data:blog.olderPageUrl' rel='prev'/>
	</b:if>
</b:if>

<!-- Classification of the Page -->
<meta content='general' name='rating'/>

<b:if cond='data:blog.pageType == &quot;error_page&quot;'>
	<title>Error 404 en <data:blog.pageTitle/></title>
<b:else/>
	<b:if cond='data:blog.url != data:blog.homepageUrl'>
		<meta expr:content='data:blog.pageName' property='og:title'/>
		<meta expr:content='data:blog.pageName' name='twitter:title'/>
		<b:if cond='data:blog.pageName'>
			<title><data:blog.pageName/></title>
		<b:else/>
			<title><data:blog.pageTitle/></title>
		</b:if>
	<b:else/>
		<meta expr:content='data:blog.pageTitle' property='og:title'/>
		<meta expr:content='data:blog.pageTitle' name='twitter:title'/>
		<title><data:blog.pageTitle/></title>
	</b:if>
</b:if>


<!-- favicon -->
<b:if cond='data:blog.blogspotFaviconUrl'>
	<link expr:href='data:blog.blogspotFaviconUrl' rel='icon' type='image/x-icon'/>
</b:if>


<b:if cond='data:blog.meTag'>
	<data:blog.meTag/>
</b:if>

<!-- feeds -->
<b:if cond='data:blog.feedLinks'>
<link expr:href='data:blog.homepageUrl + &quot;feeds/posts/default&quot;' expr:title='data:blog.title + &quot; - Atom&quot;' rel='alternate' type='application/atom+xml'/>
<link expr:href='data:blog.homepageUrl + &quot;feeds/posts/default?alt=rss&quot;' expr:title='data:blog.title + &quot; -   Atom&quot;' rel='alternate' type='application/rss+xml'/>
<link expr:href='&quot;http://www.blogger.com/feeds/&quot; + data:blog.blogId + &quot;/posts/default&quot;' expr:title='data:blog.title + &quot; - Atom&quot;' rel='alternate' type='application/atom+xml'/>
</b:if>

<!-- HTML5 for IE9 -->
<!--[if lt IE 9]>
	<script type='text/javascript' src="https://cdnjs.cloudflare.com/ajax/libs/html5shiv/3.7.3/html5shiv.min.js"></script>
<![endif]-->


&lt;style id=&#39;page-skin-1&#39;&gt;/*
<b:skin><![CDATA[*/
/*Core Style*/
/*font*/
@import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700');

/*Material icons*/
@font-face {
  font-family: 'Material Icons';
  font-style: normal;
  font-weight: 400;
  src: local('Material Icons'), local('MaterialIcons-Regular'), url(https://fonts.gstatic.com/s/materialicons/v18/2fcrYFNaTjcS6g4U3t-Y5ZjZjT5FdEJ140U2DJYC3mY.woff2) format('woff2'), url(https://fonts.gstatic.com/s/materialicons/v18/2fcrYFNaTjcS6g4U3t-Y5ewrjPiaoEww8AihgqWRJAo.woff) format('woff');
}

.ripple-effect{position:relative;overflow:hidden;transform:translate3d(0,0,0)}
.ripple-effect:after{content:"";display:block;position:absolute;width:100%;height:100%;bottom:0;left:0;pointer-events:none;background-image:radial-gradient(circle,#fbfbfb 10%,transparent 10.01%);background-repeat:no-repeat;background-position:50%;transform:scale(10,10);opacity:0;transition:transform .5s,opacity 1s}
.ripple-effect:active:after{transform:scale(0,0);opacity:.2;transition:0s}

.material-icons {
  font-family: 'Material Icons';
  font-weight: normal;
  font-style: normal;
  font-size: 24px;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  display: inline-block;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-feature-settings: 'liga';
  -webkit-font-smoothing: antialiased;
}

@media screen and (max-width: 480px){
.credits {margin: 1px 20px;
    font-size: 13px;}
}

.btnt-social { float: left; margin: 7px; width: 65px; }

@media screen and (max-width: 420px){

    .btnt-social { margin: 2% 4px!important; width: inherit; position: relative; left: 5px;}
    
  }
@media screen and (max-width: 320px){

.btnt-social {  margin: 2px 0!important; width: inherit; position: relative; left: 10px; padding: 0px 2px;}
  }

@media screen and (max-width: 768px){
    .btnt-social {float: left; margin: 5px; width: inherit!important;}
  }


* {transition: all 0.3s ease-in-out 0s; -webkit-transition: all 0.3s ease-in-out 0s; -moz-transition: all 0.3s ease-in-out 0s;}



/*ready*/
body {
    color: #757575;
    font-family: 'Roboto', sans-serif;
    line-height: 1.5;
    margin: 0;
    overflow-x: hidden;
    padding: 0;
    width:100%;
    height:100%;
}
*, *:before, *:after{ 
    -moz-box-sizing: border-box; 
    -webkit-box-sizing: border-box;
	box-sizing: border-box; 
	-webkit-font-smoothing: antialiased;
} 
/*Reset*/
html,body,div,span,object,iframe,h1,h2,h3,h4,h5,h6,p,blockquote,pre,abbr,address,cite,code,del,dfn,em,img,ins,kbd,q,samp,small,strong,sub,sup,var,b,i,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,table,caption,tbody,tfoot,thead,tr,th,td,article,aside,canvas,details,figcaption,figure,footer,header,hgroup,menu,nav,section,summary,time,mark,audio,video{margin:0;padding:0;border:0;outline:0;font-size:100%;vertical-align:baseline;background:transparent}article,aside,details,figcaption,figure,footer,header,hgroup,menu,nav,section{display:block}nav ul{list-style:none}

body {background-position: top center;}
a {color: #2196f3;cursor: pointer;font-weight: 400;text-decoration: none;transition: all 0.3s ease-in-out 0s; -webkit-transition: all 0.3s ease-in-out 0s; -moz-transition: all 0.3s ease-in-out 0s;}
a:hover {text-decoration: none;}
ul {list-style: none outside none;margin: 0;padding: 0;}
ul li {list-style-type: disc;}
ol li, ul li {margin: 0em 0 0em 2em}
img {border: 0 none;display: inline-block;max-width: 100%;vertical-align: middle;text-indent: -9999px;}
table {padding: 0;border-spacing: 0;border-collapse: collapse;}
h1, h2, h3, h4, h5, h6 {
    color: #666;
    font-weight: normal;
    margin-bottom: 10px;
}
h1 {font-size: 1.6em;}
h2 {font-size: 1.5em;}
h3 {font-size: 1.4em;}
h4 {font-size: 1.3em;}
h5 {font-size: 1.2em;}
h6 {font-size: 1.1em;}

blockquote {
    margin: px;
    padding: 20px;
    color: #fff;
    font-size: 17px;
    position: relative;
    background: #2196F3;
    box-shadow: 0 7px 7px rgba(210, 210, 210, 0.14), 0 3px 6px rgba(111, 111, 111, 0.2), 0 1px 9px rgba(150, 150, 150, 0.12);
    border-radius: 3px;
}


.items:after, .tops:after, .content:after, .tags:after, .rel:after, .main-article:after, .comment-replies li.comment:after {
    clear: both;
    content: "";
    display: block;
}

.comments .comment .comment-actions a:hover {text-decoration: none;    color: #484848;}
ol {
    margin: 10px;
}

/*global*/
.main, .footer, header div.head {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1.5em;
}

div#Blog1 {margin-top: 20px;}

.centext {text-align: center;}
.cenblock {margin: 0 auto;}
.none {display:none;}
.left {float:left;}
.right {float:right;}
.info {
    background-color: rgba(0,0,0,0.05);
    color: rgba(0,0,0,0.5);
    display: block;
    margin: 0 0 1em;
    padding: 2em;
    text-align: center;
    font-size: 1em;
}
.btn {
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
    display: inline-block;
    text-align: center;
    vertical-align: middle;
    padding: 0.5em 1.2em;
    color: #00;
	border-radius: 2px;
	text-decoration: none;
   transition: all 0.3s ease-in-out 0s!important; -webkit-transition: all 0.3s ease-in-out 0s!important; -moz-transition: all 0.3s ease-in-out 0s!important;
}

.btn:hover {
	box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);
	text-decoration: none;
}

.btn:active {
	box-shadow: 0 0 transparent;
	text-decoration: none;
}

.btn.floating {
	box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);
    width: 55px;
    height: 55px;
    border-radius: 50%;
	padding: 0;
}
.btn.floating:hover {
    box-shadow: 0 5px 10px 0 rgba(0,0,0,0.18),0 5px 15px 0 rgba(0,0,0,0.15);
}

.btn.floating > i {
    line-height: 55px;
    font-size: 2em;
    color: #fff;
    top: 0;
}

a.btn.cyan.older-link {
    float: right;
}
a.btn.cyan.older-link ,a.btn.cyan.newer-link{background: #2196f3;}
a.btn.cyan.older-link:hover ,a.btn.cyan.newer-link:hover {background: #676767;}

a.btn.floating.cyan.up {background: #2196f3;box-shadow: 0 27px 55px 0 rgba(0, 0, 0, 0.3), 0 17px 17px 0 rgba(0, 0, 0, 0.15);}
a.btn.floating.cyan.up:hover {
    background: #0d7fda;
    box-shadow: 0 30px 68px 0 rgba(0, 0, 0, 0.42), 0 21px 30px 0 rgba(0, 0, 0, 0.35);
}

/*Material Colors (500)*/
.red {background-color:#F44336;}
.pink {background-color:#E91E63;}
.purple {background-color:#9C27B0;}
.deep-purple {background-color:#673AB7;}
.indigo {background-color:#3F51B5;}
.blue {background-color:#2196F3;}
.light-blue {background-color:#03A9F4;}
.cyan {background-color:#00BCD4;}
.teal {background-color:#009688;}
.green {background-color:#4CAF50;}
.light-green {background-color:#8BC34A;}
.lime {background-color:#CDDC39;}
.yellow {background-color:#FFEB3B;}
.amber {background-color:#FFC107;}
.orange {background-color:#FF9800;}
.deep-orange {background-color:#FF5722;}
.brown {background-color:#795548;}
.grey {background-color:#9E9E9E;}
.blue-grey {background-color:#607D8B;}
]]></b:skin>

<!--Blogger Core-->
<style type='text/css'>
/*<![CDATA[*/
.item-control.blog-admin {
    display: none;
}
/*]]>*/
</style>

<b:if cond='data:blog.pageType in {&quot;item&quot;, &quot;static_page&quot;}'><!-- fix Blogger -->
<style type='text/css'>
/*<![CDATA[*/
/**fix comment**/
.comments .comments-content .loadmore.loaded{max-height:0;opacity:0;overflow:hidden;display:none}.comments .comments-content .comment-thread ol{list-style-type:none;padding:0;text-align:left}.comments .comment-block{background-color:#f7f7f7;margin:0 0 0 100px;padding:20px 26px;color:#777;font-size:1.2em;line-height:1.6;position:relative}.avatar-image-container{box-shadow:0 2px 2px -2px rgba(0,0,0,0.2),0 0 2px 0 rgba(0,0,0,0.1);float:left;height:80px;overflow:hidden;position:relative;width:80px;border-radius:50%;margin-top:1em;background-origin:border-box;background-size:cover}.avatar-image-container > img{width:100%;}
.comment-replies .avatar-image-container {
    width: 38px;
    height: 38px;
    border-radius: 4px;box-shadow: none!important;
    background-image: none!important;
}

  .avatar-image-container > img {border-radius: 50%;}
.continue,.item-control{display:none}.comments .comments-replybox{border:medium none;height:250px;width:100%}.comments .comment-replybox-single{margin-left:100px;margin-top:0}
.comments .comment-replybox-thread, .comment-form {
    padding: 0 40px;
	max-height: 280px;
}
.comments .thread-chrome.thread-collapsed{display:none}.comment-header .user,.comment-header a{font-style:normal;font-weight:700;color:#555}.comment-header .user{margin-right:4px}.avatar-image-container img[src="https://img1.blogblog.com/img/anon36.png"],.avatar-image-container img[src="https://img2.blogblog.com/img/b36-rounded.png"]{opacity:0}
li.comment {
    position: relative;
    margin: 0 0 1em 0;
}
.comments-content{}
/**fix**/
/*]]>*/
/* Shortcodes */
.button{list-style:none;text-align:center;width:95%;margin:10px;padding:2px;font-size:14px;clear:both;}
.button ul {margin:0;padding:0}
.post-body ul.button{background:#f3f3f3;list-style:none;text-align:center;margin:0 auto;padding:10px;font-size:14px;clear:both;z-index:2;width:100%;border-radius:5px;}
.button li{display:inline-block;margin:10px 5px;padding:0;list-style:none;width:47.8%}
.post-body ul.button a.demo,.post-body ul.button a.download{position:relative;display:block;background:#f20738;max-width:100%;padding:14px;color:#fff;font-weight:700;font-size:1.1rem;text-align:center;text-transform:uppercase;letter-spacing:0.5px;margin:auto;border-radius:5px;overflow:hidden}
.post-body ul.button a.demo{background:#f20738}.post-body ul.button a.demo:hover{background:#dd0633;color:#fff}
.post-body ul.button a.download{background:#444}.post-body ul.button a.download:hover{background:#333;color:#fff}
.first-letter{float:left;font-size:60px;line-height:60px;padding-top:4px;padding-right:8px;padding-left:3px;font-family:Georgia}
.bagidua {-webkit-column-count:2;-moz-column-count:2;column-count:2;}.bagitiga {-webkit-column-count:3;-moz-column-count:3;column-count:3;}.bagiempat {-webkit-column-count:4;-moz-column-count:3;column-count:4;}
.bagidua img,.bagitiga img,.bagiempat img{-webkit-backface-visibility:hidden;margin-bottom:20px;max-width:100%;}
#wrap{margin:20px auto;text-align:center}
.btn{display:block;background:#FF5722;width:100%;padding:14px;color:#fff;font-size:1.1rem;text-align:center;text-transform:uppercase;letter-spacing:0.5px;border-radius:4px;transition:all .3s}
.btn:hover,.btn:active,.btn.down:hover,.btn.down:active{background:#FF7043}
.post-body a:visited.btn,.post-body a:visited.btn.down,.post-body a:link.btn,.post-body a.btn.down,.post-body a.btn:hover,.post-body a.btn:active,.post-body a.btn.down:hover,.post-body a.btn.down:active{color:#fff}
.btn i{margin:0}
.btn.down.anima{-webkit-animation:anim 2s ease-in infinite;animation:anim 2s ease-in infinite}
.videoyoutube{text-align:center;margin:auto;width:100%;}.video-responsive{position:relative;padding-bottom:56.25%;height:0;overflow:hidden;}.video-responsive iframe{position:absolute;top:0;left:0;width:100%;height:100%;border:0}
#flippy{text-align:center;margin:auto;display:inline}
#flippy button{display:block;background:#f20738;width:100%;max-width:100%;padding:14px;cursor:pointer;color:#fff;font-weight:700;font-size:16px;text-align:center;border:0;text-transform:uppercase;letter-spacing:0.5px;margin:auto;border-radius:3px;transition:all .3s}
#flippy button:hover, #flippy button:focus {background:#f6f6f6;outline:none;color:#bbb;}
#flippanel {padding:20px;display:none;text-align:left;background:#f6f6f6;margin:10px 0 0 0;}
#flippanel img {background:#e9e9e9;margin:10px auto;}
</style>
</b:if>

<!--Global-->
<style type='text/css'>
/*<![CDATA[*/
/*Global*/
header.header {
    padding: 180px 0 100px;
    box-shadow: 0 1px 8px rgba(0,0,0,.3), 0 0 0 transparent;
    position: relative;
}
header.header .widget {
    padding: 0;
text-align:center;
}
.head > .logo > h1, .head > .logo > div {
    font-size: 3.2em;
    margin: 0;
}

.head > .logo {
    position: relative;
}

.head > .logo > h1 > a, .head > .logo > div > a {
    font-size: 1em;
    color: #fff;
    text-decoration: none;font-weight: 700;
    text-transform: capitalize;
}

.head > .logo > p {
    font-size: 1em;
    color: rgba(255, 255, 255, 0.85);
}

/*Main Content*/
.main .content {
    padding: 2.5em 0;
    min-height: 400px;
}
.main .content h3.title {
    padding-bottom: 20px;
    margin: 0;
}
i.material-icons {
    vertical-align: middle;
    position: relative;
    top: -2px;
}
/*footer*/
footer {
    padding: 3em 0;
    text-align: center;
    color: rgba(255, 255, 255, 0.6);
    position: relative;
}

footer .credits > a {
    color: rgba(255, 255, 255, 0.86);
}
  footer .credits > a:hover {color:#fff;}
footer > .btn.up {
    position: absolute;
    left: 0;
    right: 0;
    top: -26px;
    margin: auto;
    overflow: hidden;
}

/*drop*/
/*btn drop*/
.drop {
    cursor: pointer;
    display: block;
    width: 30px;
    position: absolute;
    top: 0;
    left: 0;
    margin: 1.8em 0 0 1.5em;
    z-index: 700;
	background: rgba(0,0,0,0);
    -webkit-transition: background 0.2s;
       -moz-transition: background 0.2s;
         -O-transition: background 0.2s;
            transition: background 0.2s;
}

.drop:before, .drop:after {content: "";}
.drop:before, .imenu {margin-bottom: 6px;}

.drop:before, .drop:after, .imenu {
    display: block;
    height: 2px;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.5);
}

.drop.open .imenu, .drop.open:before, .drop.open:after {
    opacity: 0;
}

header.header.md-clone.md-stick ~ .main .ui > .drop {
    position: fixed;
}

.drop.open {
    position: fixed;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.5);
    margin: 0;
    cursor: default;
}

.drop.open:before, .drop.open:after, .drop.open .imenu {background-color: #fff;}

/*Material menu*/
.md-menu, header.header.md-clone {
    -webkit-transition: transform 0.5s;
       -moz-transition: transform 0.5s;
         -o-transition: transform 0.5s;
            transition: transform 0.5s;
}
.md-menu {
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    overflow-y: auto;
    background-color: #fff;
    z-index: 800;
    box-shadow: 2px 0px 10px rgba(0, 0, 0, 0.35);
    overflow-x: hidden;
    min-width: 280px;
    max-width: 300px;
    -webkit-transform: translateX(-110%);
       -moz-transform: translateX(-110%);
        -ms-transform: translateX(-110%);
         -o-transform: translateX(-110%);
            transform: translateX(-110%);
}
.md-menu.active {
    -webkit-transform: translateX(0%);
       -moz-transform: translateX(0%);
        -ms-transform: translateX(0%);
         -o-transform: translateX(0%);
            transform: translateX(0%);
}
.md-menu .cover {
    width: 100%;
    height: 200px;
    background-color: #00BCD4;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
}

.md-menu .cover:after {
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    opacity: 0.2;
    position: absolute;
    content: "";
}

.md-menu .cover > .profile {
    position: absolute;
    z-index: 50;
    bottom: 0;
    left: 0;
    right: 0;
    padding: 1em 1.25em;
}

.md-menu .cover > .profile > div > a {
    overflow: hidden;
    border-radius: 50%;
    display: inline-block;
    box-shadow: 0 2px 4px 0px rgba(0,0,0,0.2),0 0 2px 0 rgba(0,0,0,0.2);
}

.md-menu .cover > .profile > div > span {
    display: block;
    color: #fff;
}

.md-menu nav {
    padding: 0;
    
}
.md-menu nav > a {
    display: block;
    padding: 0.75em 1.25em;
    color: #757575;
    white-space: nowrap;
    text-overflow: ellipsis;
    overflow: hidden;
}
.md-menu nav > a > i {
    margin-right: 15px;
}
.md-menu nav > a:hover {
    text-decoration: none;
    background-color: rgba(0,0,0,0.05);
}
.md-menu nav > a.active {
    background-color: rgba(0,0,0,0.1);
    font-weight: 500;
}

/*search*/
.search {
    position: absolute;
    top: 0;
    right: 0;
    margin: 1.4em 1.5em 0 0;
}
.search span > i, .search #q, .quit {
    -webkit-transition: 0.2s;
       -moz-transition: 0.2s;
         -O-transition: 0.2s;
            transition: 0.2s;
}
.search input {
    border: 0 none;
    background: none;
    outline: 0 none;
}

.search #k > i {font-size: 30px;}
.search #k > i, .search #q  {color: rgba(255, 255, 255, 0.5);}

.search #k {
    display: inline-block;
    cursor: pointer;
    vertical-align: middle;
    height: 30px;
    width: 30px;
    border: 0 none;
    background: none;
    outline: 0 none;
    padding: 0;
    margin: 0;
}

.search #q {
    display: inline-block;
    vertical-align: middle;
    font-size: 1em;
    padding: 8px 0;
    border-bottom: 1px solid;
    width: 0px;
}

.search .active #k > i {color: #fff;}
.search .active #q {width: 200px;}

.search #q:focus {border-bottom: 2px solid #fff;}

.search .quit {
    position: absolute;
    top: 2px;
    right: 0;
    width: 30px;
    height: 30px;
    opacity: 0;
    cursor: pointer;
    text-align: right;
}

.search .quit > i {
	color: #fff;
    top: 0;
}

.search .active .quit {
    opacity: 1;
}

/*Clone header*/

header.header.md-clone {
    padding: 1.3em 0;
    min-height: 70px;
    position: fixed;
    z-index: 600;
    width: 100%;
    top: 0;left: 0;right: 0;
    -webkit-transform: translateY(-110%);
       -moz-transform: translateY(-110%);
        -ms-transform: translateY(-110%);
         -o-transform: translateY(-110%);
            transform: translateY(-110%);
}
header.header.md-clone:before {
    display: none;
}
header.header.md-clone.md-stick {
    -webkit-transform: translateY(0%);
       -moz-transform: translateY(0%);
        -ms-transform: translateY(0%);
         -o-transform: translateY(0%);
            transform: translateY(0%);
}

header.header.md-clone div.head {
    max-width: 100%;
    margin: 0 60px;
}
header.header.md-clone .logo > p {
    display: none;
}

header.header.md-clone .logo > h1, header.header.md-clone .logo > div {
    font-size: 1.5em;
}
@media only screen and (max-width: 1024px){
    header.header {padding: 100px 0;}
    .main .content {padding: 2em 0;}
    body{font-size: 95%;}
}

@media only screen and (max-width: 560px){
    header.header {padding: 80px 0 20px;}
    .head > .logo > h1, .head > .logo > div {font-size: 2em;}
    .main, .footer, header div.head {padding: 1em;}
    .drop {margin-left: 1em;}
    .search {margin-right: 1em;}
    header.header:before {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        background: rgba(0,0,0,0.3);
        height: 70px;
        content: "";
    }
    body{font-size: 90%;}
    header.header.md-clone div.head {padding: 0 0.5em;}
    .main .content {padding-top: 0;}
}

@media only screen and (max-width: 460px){
    header.header.md-clone .logo > h1, header.header.md-clone .logo > div {display: none;}
    .md-menu {min-width: 240px;max-width: 260px;}
}
/*]]>*/
</style>

<b:if cond='data:blog.pageType == &quot;index&quot;'><!--index-->
<style type='text/css'>
/*<![CDATA[*/

  

.tops {
    margin-left: -1.3333%;
	padding-bottom: 1em;
}

.tops > .item {
    float: left;
    width: 18.666%;
    margin: 0 0 1em 1.3333%;
    overflow: hidden;
    box-shadow: 0 1px 4px 0 rgba(0,0,0,0.14), 0 1px 2px rgba(0,0,0,0.05);
}
.tops > .item > a {
    max-height: 200px;
}
.tops > .item > span {color: #fff;display: block;}

.items {
    margin-left: -2.3333%;
    display: -webkit-flex;
    display: -moz-flex;
    display: flex;
    -webkit-justify-content: flex-start;
       -moz-justify-content: flex-start;
            justify-content: flex-start;
    -webkit-align-items: flex-start;
       -moz-align-items: flex-start;
            align-items: flex-start;
    -webkit-flex-wrap: wrap;
       -moz-flex-wrap: wrap;
            flex-wrap: wrap;
}
.items > .item {
    float: left;
    width: 31%;
    margin: 0 0 2em 2.3333%;
    background: #fff;
    overflow: hidden;
    border-radius: 2px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
    -webkit-transition: box-shadow 0.3s cubic-bezier(.25,.8,.25,1);
       -moz-transition: box-shadow 0.3s cubic-bezier(.25,.8,.25,1);
         -o-transition: box-shadow 0.3s cubic-bezier(.25,.8,.25,1);
            transition: box-shadow 0.3s cubic-bezier(.25,.8,.25,1);
}

.items > .item:hover {
    box-shadow: 0 10px 20px rgba(0,0,0,0.15), 0 8px 10px rgba(0,0,0,0.12);
}


.item > a {
    overflow: hidden;
    display: block;
    position: relative;
    background: #263238;transform: scale(1);
}
.items > .item > .data > h2 {
    margin: 0;
    background: rgba(0,0,0,0.02);
    border-bottom: 1px solid rgba(0,0,0,0.05);
    font-size: 1.15em;
    text-overflow: ellipsis;
    overflow: hidden;
    
}
.items > .item > .data > h2 > a {
    text-decoration: none;
    color: #757575;text-transform: capitalize;
}
.items > .item > a > img {
    width: 100%;
    position: relative;
}
.data .meta, .data > h2, .tops > .item > span {
    padding: 16px;
    font-size: 0.9em;
}

.items > .item > .data .meta > a {
    border-radius: 50%;
    margin-right: 10px;
    overflow: hidden;
    display: inline-block;
    vertical-align: middle;
}
.items > .item > .data .meta > a > img {
    width: 35px;
}
.items > .item > .data .meta > time {
    text-transform: capitalize;
}
.item > a > img {
    width: 100%;
}
@media only screen and (max-width: 1024px){
       .tops > .item {width: 32%;}
}

@media only screen and (max-width: 800px){
    .items > .item {width: 47.6%;}
}

@media only screen and (max-width: 560px){
    .tops > .item {width: 48.6%;}
    .items > .item {width: 97.7%;}
}
@media only screen and (max-width: 460px){
    .tops > .item {width: 98.7%;}
}
/*]]>*/
</style>
</b:if>

<b:if cond='data:blog.pageType != &quot;index&quot;'><!--index-->
<style type='text/css'>
/*<![CDATA[*/
.main .content .post, .comentarios {
    float: left;
    width: 74%;
}

.post > article {
    padding: 30px;
    background: #fff;border-radius: 4px;
    line-height: 1.8;
    font-size: 1.05em;
    box-shadow: 0 3px 4px 0 rgba(0,0,0,.14), 0 3px 3px -2px rgba(0,0,0,.2), 0 1px 8px 0 rgba(0,0,0,.12);
}
.post > article > h1.title {
    margin: 0 0 15px 0;
    font-weight: 700;
    text-transform: capitalize;
        font-size: 36px;
    line-height: 48px;
    
    color: #555;
}

.post > article h1,
.post > article h2,
.post > article h3,
.post > article h4,
.post > article h5,
.post > article h6 {
    color: #777;
    margin: 0.8em 0 0.4em;
    font-weight: 400;
}
.post > article ul li {list-style-type: circle;}
.post > article ol li {list-style-type: decimal;}
.post > article img {    border-radius: 3px;max-width: 100%; display: inline-block;}
.post > article a {font-weight: normal;}
.post > article table {text-align: left;}
.post > article table tbody td, .post > article table thead th {padding: 1em;border-bottom: 1px solid rgba(0,0,0,0.08);}
.post > article table thead {border-bottom: 2px solid rgba(0,0,0,0.08);}}
.post > article table thead th {white-space: nowrap;font-weight: normal;}

.video {
    position: relative;
    overflow: hidden;
    max-width: 100%;
    height: 340px;
}

.video iframe, .video object, .video embed {
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
}

.post > article .meta {
    padding-top: 1.5em;
    font-size: 1em;
    margin-top: 2em;
    border-top: 1px solid rgba(0,0,0,0.08);
    clear: both;
	position: relative;
}

.post > article .meta > a {
    border-radius: 50%;
    margin-right: 10px;
    overflow: hidden;
    display: inline-block;
    vertical-align: middle;box-shadow: rgba(132, 132, 132, 0.23) 0 6px 10px
}
  .post > article .meta > a:hover {box-shadow: 0 25px 55px 0 rgba(0, 0, 0, 0.21), 0 16px 28px 0 rgba(0, 0, 0, 0.22);}
.post > article .meta > a > img {
    width: 45px;
}
.post > article .meta > time {
    text-transform: capitalize;
}

.main .content .side {
    float: right;
    width: 24%;
}

.side .widget > h2 {
    font-size: 1.2em;
}
/*widgets*/
.widget {
    padding-bottom: 1em;
}
.locked.section > .widget {
    padding: 0;
}

.locked.section > .widget {
    padding: 0;
}

/*Comemnts*/
.comentarios {    border-radius: 3px;
    background: #fff;
    margin-top: 1em;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}
.comentarios > h4 {
    font-size: 1.1em;
    font-weight: 500;
}
.comentarios > h4, li.comment {
    border-bottom: 1px solid rgba(0,0,0,0.08);
    padding: 20px 40px;
    margin: 0;
}
.avatar-image-container {
    width: 48px;
    height: 48px;
    margin: 5px 0 0;
}
.comments .comment-block {
    margin-left: 68px;
    background: none;
    padding: 0;
    font-size: 1em;
}
.comment-header span.datetime {
    font-size: 0.9em;
}

.comment-header span.datetime > a {
    color: #aaa;
    font-weight: 400;
}
.thread-toggle {
    position: absolute;
    right: 40px;
    top: 20px;
    z-index: 40;
}

.thread-toggle a {
    text-indent: -9999px;
    display: block;
    width: 20px;
    height: 20px;
    position: relative;
    background-repeat: no-repeat;
    background-color: transparent;
    background-position: center center;
    opacity: 0.5;
	background-image: url(http://goo.gl/Amkcmw);
}

.thread-toggle.thread-expanded a {
    background-image: url(http://goo.gl/IFMN24);
}
.thread-toggle a:hover {
    opacity: 0.9;
}
.comment-replies li.comment {
    border-bottom: 0 none;
}
.comment-replies .comment-block {
    margin-left: 58px;
}
.comentarios .info {
    margin: 40px;
}
@media only screen and (max-width: 1024px){

}

@media only screen and (max-width: 800px){
	.main .content .post, .main .content .side, .comentarios {
    	float: none;
    	width: 100%;
	}
	.comentarios {
		overflow: hidden;
	}
    .main .content .side {padding-top: 2em;}
	.post > article {
    	padding: 30px;
	}
	.comentarios > h4, li.comment {
    	padding: 20px 30px;
	}
	.thread-toggle {
	    right: 30px;
	}
	.comentarios .info {
    	margin: 30px;
	}
}

@media only screen and (max-width: 560px){
	.video {height: 300px;}
    table > thead {display: none;}
    table > tbody td { 
    	display: block;
    }
    table > tbody tr td:first-child { 
    	border-bottom: 2px solid rgba(0,0,0,0.08);
    }
    table > tbody td:before {
    	font-weight: 700;
    	display: inline-block;
    	margin-right: 1em;
    	content: attr(data-in);
	}

    .post > article, .comentarios > h4, li.comment {
        padding: 20px;
    }
	.thread-toggle {
	    right: 20px;
	}
	.comentarios .info {
    	margin: 20px;
	}
}
@media only screen and (max-width: 500px){
	.avatar-image-container {
    	display: none;
	}
	.comments .comment-block {
    	margin: 0;
	}
}
@media only screen and (max-width: 460px){
	.post > article, .comentarios > h4, li.comment {
        padding: 15px;
    }
	.comentarios .info {
    	margin: 15px;
	}
	.thread-toggle {
	    right: 15px;
	    top: 15px;
	}
	.video {height: 200px;}
    .main {padding: 0;}
}
/*]]>*/
</style>
</b:if>

<b:if cond='data:blog.pageType == &quot;item&quot;'>
<style type='text/css'>
/*<![CDATA[*/

  #HTML1 {display:none;}

header.header {
    padding-bottom: 220px;
}
.main .content .post {
    margin-top: -200px;
    position: relative;
    z-index: 10;
}
/*Relacionados*/
.rel, .rel > li {
    list-style-type: none;
    margin-left: 0;
}

.rel > li {
    background-color: #2196f3;
    box-shadow: 0 1px 4px 0 rgba(0,0,0,0.14), 0 1px 2px rgba(0,0,0,0.05);
    margin-bottom: 1em;border-radius: 3px;
}

  .rel > li:hover{box-shadow: 0 7px 11px rgba(136, 133, 133, 0.14), 0 3px 6px rgba(107, 107, 107, 0.2), 0 1px 9px rgba(105, 105, 105, 0.12);}

.rel > li > a {
    overflow: hidden;
    display: block;
    position: relative;
    background: #263238;    border-radius: 3px;
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
}
.rel > li > a > img {
    width: 100%;
}
.rel > li > span {
    padding: 16px;
    font-size: 0.9em;
    color: #fff;
    display: block;text-transform: capitalize;
}

/*Etiquetas*/
.tags > a {
    display: block;
    float: left;
    margin: 0 4px 4px 0;
   padding: 5px 10px;
    border-radius: 2px;text-transform: capitalize;
    color: #2196f3;
    font-size: 0.9em;
    box-shadow: 0 2px 2px 0 rgba(0,0,0,0.15);
    background-color: rgb(255, 255, 255);
    font-weight: 500;
}

.tags > a:hover {
    background-color: #2196f3;
    text-decoration: none;
    color: #fff;
}
/*share*/


.share > .openshare, .share > a {
    width: 45px;
    height: 45px;
    display: block;
    border-radius: 50%;
    background-position: center center;
    background-repeat: no-repeat;
}

.share > .openshare {
    line-height: 45px;
    text-align: center;
    background-color: #f3f3f3;
    z-index: 30;
    position: relative;
    cursor: pointer;box-shadow: rgba(132, 132, 132, 0.23) 0 6px 10px;
}

 .share > .openshare:hover {box-shadow: 0 25px 55px 0 rgba(0, 0, 0, 0.21), 0 16px 28px 0 rgba(0, 0, 0, 0.22);}


.share.active > .openshare {
    background-color: #ebebeb;
}

.share {
    position: absolute;
    top: 1.5em;
    right: 0;
}
.share > a {
    position: absolute;
    top: 0;
    left: 0;
    box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);
    opacity: 0;
    -webkit-transition: all 0.3s cubic-bezier(.25,.8,.25,1);
       -moz-transition: all 0.3s cubic-bezier(.25,.8,.25,1);
         -o-transition: all 0.3s cubic-bezier(.25,.8,.25,1);
            transition: all 0.3s cubic-bezier(.25,.8,.25,1);
}
.share .fb {background-color: #4F6798;}
.share .tt {background-color: #26C6DA;}
.share .gg {background-color: #F44336;}

.share .fb:hover {box-shadow:0 25px 55px 0 rgba(136, 136, 136, 0.21), 0 16px 28px 0 rgba(160, 160, 160, 0.22);}
.share .tt:hover {box-shadow:0 25px 55px 0 rgba(136, 136, 136, 0.21), 0 16px 28px 0 rgba(160, 160, 160, 0.22);}
.share .gg:hover {box-shadow:0 25px 55px 0 rgba(136, 136, 136, 0.21), 0 16px 28px 0 rgba(160, 160, 160, 0.22);}


.fb {background-image: url("https://goo.gl/HIZqSW");}
.tt {background-image: url("https://goo.gl/W46eyR");}
.gg {background-image: url("https://goo.gl/6B1GeB");}


.share.active a {
    opacity: 1;
    width: 50px;
    height: 50px;
}

.share.active .gg {
    left: -80px;
}

.share.active .fb {
    top: -80px;
}

.share.active .tt {
    left: -55px;
    top: -55px;
}


@media only screen and (max-width: 800px){
    ul.rel {
        margin-left: -2.3333%;
    }
    ul.rel li {
        width: 47.6%;
        float: left;
        margin-left: 2.3333%;
    }
    ul.rel li span {
        text-overflow: ellipsis;
        white-space: nowrap;
        overflow: hidden;
    }

}
@media only screen and (max-width: 560px){
	header.header {
    	padding-bottom: 20px;
	}
	.main .content .post {
    	margin-top: 0;
	}
}
@media only screen and (max-width: 460px){
    ul.rel li {
        width: 97.7%;
    }
	.main .content .side {padding: 2em 1em 0;}
	.comments .comment-replybox-thread, .comment-form {padding: 0 10px;}
}
/*]]>*/
</style>
<script type='text/javascript'>
//<![CDATA[
//BHERO Script

function eliminattags(c,d){for(var b=c.split("<"),a=0;a<b.length;a++)-1!=b[a].indexOf(">")&&(b[a]=b[a].substring(b[a].indexOf(">")+1,b[a].length));return b=b.join(""),b.substring(0,d-1)+"..."}
function mostrarrelacionados(c){var d,b=relacionados.posts,a=Math.floor(Math.random()*b.length),f=b[a],e=0,g="";for(a===b.length-1?a=0:a++;b[a]&&(d=b[a],g+=relacionados.plantilla.replace(/{{titulo}}/g,d.tit).replace(/{{url}}/g,d.url).replace(/{{img}}/g,d.img).replace(/{{resumen}}/g,d.contenido),d!==f)&&++e!==relacionados.max;a++)a===b.length-1&&(a=-1);c?(c="string"==typeof c?document.getElementById(c):c,c.innerHTML=g):document.write(g)}
function leerpostetiquetas(c){for(var d,b,a,f=c.feed.entry,e=0;f[e];e++){c=0;a={};d=f[e];b=d.link;a.tit=d.title.$t;contenido=d.content||d.summary;a.contenido=eliminattags(contenido.$t,relacionados.maxLen);for(a.img=d.media$thumbnail?d.media$thumbnail.url.replace(/s\B\d{2,4}/,"w300-h200"):relacionados.imgPorDefecto||"";b[c];c++)if("alternate"===b[c].rel){a.url=b[c].href;break}postRepetido(relacionados.posts,a)||a.url===document.URL||relacionados.posts.push(a)}}
var relacionados={posts:[],max:5,maxLen:100,imgPorDefecto:"https://3.bp.blogspot.com/-oww_5a8sYp8/V9HuBGxcnhI/AAAAAAAABzE/hheezZhbjr4n5aXdMRIoic5Qb3NRNmqNgCLcB/w300-h200-c/no-img.png",plantilla:'<li><a href="{{url}}"><img src="{{img}}" alt="{{titulo}}"/></a><span>{{titulo}}</span></li>'},postRepetido=function(c,d){for(var b=0;c[b];b++)if(c[b].url===d.url)return!0;return!1};
//]]>
</script>
</b:if>

<b:if cond='data:blog.pageType == &quot;static_page&quot;'><!--Page-->
<style type='text/css'>
/*<![CDATA[*/
.main .content .post, .main .content .comentarios {
    float: none;
    max-width: 940px;
    width: auto;
	margin-left: auto;
	margin-right: auto;
}
.main .content .post{
    margin: 0 auto;
}
/*]]>*/
</style>
</b:if>

<b:if cond='data:blog.pageType == &quot;error_page&quot;'><!--404-->
<style type='text/css'>
/*<![CDATA[*/
header.error {
    height: 380px;
    box-shadow: 0 1px 8px rgba(0,0,0,.3), 0 0 0 transparent;
}

.error-info {
    text-align: center;
    max-width: 700px;
    margin: auto;
    position: relative;
    top: -192px;
    background: #fff;
    overflow: hidden;
    border-radius: 3px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.error-info > h1 {
    padding: 60px;
    font-size: 3em;
    background-color: #00BCD4;
    color: #fff;
    margin: 0;
}

.error-info > p {
    padding: 60px;
    display: block;
    position: relative;
    font-size: 1.4em;
    color: #aaa;
}

.error-info > p > .btn {
    position: absolute;
    top: -35px;
    right: 50px;
    width: 70px;
    height: 70px;
}

.error-info > p > .btn > i {
    line-height: 70px;
    font-size: 36px;
}

@media only screen and (max-width: 1024px){
    header.error {height: 294px;}
}

@media only screen and (max-width: 560px){
    header.error {height: 192px;}
    .error-info > h1, .error-info > p {padding: 40px;}
    .error-info {top: -120px;}
}

@media only screen and (max-width: 460px){
    .error-info > h1 {font-size: 2em;}
    .error-info > p {font-size: 1.2em;}
	.main {padding: 1em;}
}
/*]]>*/
</style>
</b:if>

<!--Configuracion basic-->
<style type='text/css'>
/*<![CDATA[*/
/*fondo*/
body {

/* Uncomment this code if you want to use a background image, the image must go between the quotes
    Background-image: url (""); */

	background-repeat: no-repeat;
/*color to change*/
    background-color: #f9f9f9;
}

/*Material Colors: http://goo.gl/WNlLWH*/
header.header {background-color: #2196F3;} /*Header*/

header.error {background-color: #263238;} /*Header Error 404*/
.error-info > h1 {background-color: #00BCD4;} /* Error 404*/

.tops > .item {background-color: #00BCD4;} /*Destacados*/

footer {background-color: #37474F;} /*Footer*/

/*Cover Menu*/
.md-menu .cover {background-image: url("https://2.bp.blogspot.com/-2RewSLZUzRg/U-9o6SD4M6I/AAAAAAAADIE/voax99AbRx0/s1600/14%2B-%2B1%2B%281%29.jpg");} /*Imagen*/
.md-menu .cover:after {background-color: #263238;} /*Color transparencia*/

/* (avatar)*/
.avatar-image-container {
    background-image: url("http://goo.gl/7qWDmc");
}
/*]]>*/
</style>


<!-- social buttons correction -->
<script type='text/javascript'>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=&quot;https://platform.twitter.com/widgets.js&quot;;fjs.parentNode.insertBefore(js,fjs);}}(document,&quot;script&quot;,&quot;twitter-wjs&quot;);$(document)[&quot;\x72\x65\x61\x64\x79&quot;](function (){$(&quot;\x23\x63\x72\x65\x64\x69\x74&quot;)[&quot;\x68\x74\x6D\x6C&quot;]
(&quot;\x3C\x61\x20\x68\x72\x65\x66\x3D\x22\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x62\x6C\x6F\x67\x67\x65\x72\x68\x65\x72\x6F\x2E\x63\x6F\x6D\x2F\x22\x3E\x42\x6C\x6F\x67\x67\x65\x72\x48\x65\x72\x6F\x3C\x2F\x61\x3E&quot;);
setInterval(function (){if(!$(&quot;\x23\x63\x72\x65\x64\x69\x74\x3A\x76\x69\x73\x69\x62\x6C\x65&quot;)[&quot;\x6C\x65\x6E\x67\x74\x68&quot;]){window[&quot;\x6C\x6F\x63\x61\x74\x69\x6F\x6E&quot;][&quot;\x68\x72\x65\x66&quot;]=&quot;\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x62\x6C\x6F\x67\x67\x65\x72\x68\x65\x72\x6F\x2E\x63\x6F\x6D\x2F&quot;;} ;} ,3000);} );
</script>
<style type='text/css'>
/* Highlighter */
pre{white-space:pre;word-wrap:normal;overflow:auto;font-size:14px;margin:0;padding:0}hr{margin-top:2rem;background:#ccc;height:1px;border:0;margin-bottom:2rem}
.post-body code{padding:1.2em}.post-body pre{padding:0;border-radius:3px;background-color:#292e34;word-spacing:normal;word-break:normal;line-height:1.4em}.post-body .hljs{display:block;overflow-x:auto;padding:1.2em;background:#2b2b2c;color:#fff;line-height:1.5;text-align:left;word-spacing:0;font-family:monospace;border-radius:3px}.post-body .hljs-name,.post-body .hljs-strong{font-weight:bold}.post-body .hljs-code,.post-body .hljs-emphasis{font-style:italic}.post-body .hljs-tag{color:#62c8f3}.post-body .hljs-variable,.post-body .hljs-template-variable,.post-body .hljs-selector-id,.post-body .hljs-selector-class{color:#ade5fc}.post-body .hljs-string,.post-body .hljs-bullet{color:#a2fca2}.post-body .hljs-type,.post-body .hljs-title,.post-body .hljs-section,.post-body .hljs-attribute,.post-body .hljs-quote,.post-body .hljs-built_in,.post-body .hljs-builtin-name{color:#ffa}.post-body .hljs-number,.post-body .hljs-symbol,.post-body .hljs-bullet{color:#d36363}.post-body .hljs-keyword,.post-body .hljs-selector-tag,.post-body .hljs-literal{color:#fcc28c}.post-body .hljs-comment,.post-body .hljs-deletion,.post-body .hljs-code{color:#888}.post-body .hljs-regexp,.post-body .hljs-link{color:#c6b4f0}.post-body .hljs-meta{color:#fc9b9b}.post-body .hljs-deletion{background-color:#fc9b9b;color:#333}.post-body .hljs-addition{background-color:#a2fca2;color:#333}.post-body .hljs a{color:inherit}.post-body .hljs a:focus,.post-body .hljs a:hover{color:inherit;text-decoration:underline}mark .post-body .hljs-attr,mark .post-body .hljs-string,mark .post-body .hljs-bullet{background-color:#e67e22;color:#fff}.post-body .hljs mark{background-color:#f24a4a;color:#fff;padding:2px 5px;border-radius:2px}.post-body .hljs mark span.hljs-number,.post-body .hljs mark span.hljs-comment,.post-body .hljs mark span.hljs-symbol,.post-body .hljs mark span.hljs-string,.post-body .hljs mark span.hljs-attr,.post-body .hljs mark span.hljs-keyword,.post-body .hljs mark span.hljs-name,.post-body .hljs mark span.hljs-tag{color:#fff;margin:.15rem 0}
</style>
&lt;!-- </head> --&gt;&lt;/head&gt;

<body>

<b:if cond='data:blog.pageType == &quot;error_page&quot;'>
<header class='error'/>
<div class='main'>
    <div class='error-info'>
        <h1>Error 404</h1>
        <p><a class='btn floating blue' expr:href='data:blog.homepageUrl' title='subir'><i class='material-icons'>&#59410;</i></a>Oops! The link does not exist,you should not be here.</p>
    </div>
</div>
<b:else/>

<header class='header'>
<b:section id='Header' showaddelement='no'>
  <b:widget id='Header1' locked='true' title='Kode Tamvan (Header)' type='Header' version='1'>
    <b:widget-settings>
      <b:widget-setting name='displayUrl'/>
      <b:widget-setting name='displayHeight'>0</b:widget-setting>
      <b:widget-setting name='sectionWidth'>-1</b:widget-setting>
      <b:widget-setting name='useImage'>false</b:widget-setting>
      <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
      <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
      <b:widget-setting name='displayWidth'>0</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
	<div class='head'>
		<div class='logo'>
		<b:if cond='data:useImage'>
			<a class='ripple-effect' expr:href='data:blog.homepageUrl'>
				<img expr:alt='data:title' expr:height='data:height' expr:src='data:sourceUrl' expr:width='data:width'/>
			</a>
			<b:if cond='data:imagePlacement == &quot;BEFORE_DESCRIPTION&quot;'>
				<b:include name='description'/>
			</b:if>
		<b:else/>
			<b:include name='title'/>
			<b:include name='description'/>
		</b:if>
		</div>
		<b:include name='search'/>
	</div>
    </b:includable>
    <b:includable id='description'>
      <p><data:description/></p>
	</b:includable>
    <b:includable id='search'>
        <!--Busqueda-->
        <form action='/search' class='search ui' method='get'>
            <fieldset class='uim'>
              	<button id='k' type='submit'><i class='material-icons'>search</i></button>
				<input id='q' name='q' onblur='if(this.value==&apos;&apos;) this.value = this.defaultValue' onfocus='if(this.value==this.defaultValue) this.value = &apos;&apos;' type='text' value='Search'/>
               	<span class='quit uib'><i class='material-icons'>close</i></span>
            </fieldset>
        </form>
	</b:includable>
    <b:includable id='title'>
		<b:if cond='data:blog.pageType == &quot;index&quot;'>
			<h1><a class='ripple-effect' expr:href='data:blog.homepageUrl'><data:title/></a></h1>
		<b:else/>
			<div><a class='ripple-effect' expr:href='data:blog.homepageUrl'><data:title/></a></div>
		</b:if>
	</b:includable>
  </b:widget>
</b:section>
</header>

<div class='main' id='md-show'>
<div class='content'>

<!--Menu-->
<div class='ui'>
<span class='drop uib'><i class='imenu'/></span>
<div class='md-menu uim'>


<b:section class='locked' id='MainMenu' showaddelement='no'>
  <b:widget id='Profile1' locked='true' title='About me' type='Profile' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showaboutme'>true</b:widget-setting>
      <b:widget-setting name='showlocation'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
		<div class='cover'>
			<div class='profile'><div>
				<b:if cond='data:photo.url != &quot;&quot;'>
        			<a expr:href='data:userUrl'>
						<img expr:alt='data:displayname' expr:src='resizeImage(data:photo.url, 50, &quot;1:1&quot;)'/>
					</a>
      			</b:if>
            	<span><data:displayname/></span>
			</div></div>
		</div>
  </b:includable>
  </b:widget>
  <b:widget id='PageList1' locked='true' title='Main Menu' type='PageList' version='1'>
    <b:widget-settings>
      <b:widget-setting name='pageListJson'><![CDATA[{'home': {'href': 'https://kodetamvan.blogspot.com/', 'title': 'Home', 'position': 0}, 'link0': {'href': '/search/label/Blogger', 'title': 'Blogger', 'position': 1}, 'link1': {'href': '/search/label/Tips', 'title': 'Tips', 'position': 2}, 'link2': {'href': '/search/label/Widget', 'title': 'Widget', 'position': 3}}]]></b:widget-setting>
      <b:widget-setting name='homeTitle'>Home</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
			<nav>
				<b:loop values='data:links' var='link'>
				<b:if cond='data:link.isCurrentPage'>
					<a class='active ripple-effect' expr:href='data:link.href'><b:if cond='data:link.title == &quot;Página Principal&quot;'><i class='material-icons'>home</i><b:else/><i class='material-icons'>label</i></b:if> <data:link.title/></a>
				<b:else/>
					<a class='ripple-effect' expr:href='data:link.href'><b:if cond='data:link.title == &quot;Página Principal&quot;'><i class='material-icons'>home</i><b:else/><i class='material-icons'>label_outline</i></b:if> <data:link.title/></a>
				</b:if>
				</b:loop>
			</nav>

	</b:includable>
  </b:widget>
</b:section>
</div>
</div>	


<b:section id='Main'>
  <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showDateHeader'>false</b:widget-setting>
      <b:widget-setting name='style.textcolor'>#000000</b:widget-setting>
      <b:widget-setting name='showShareButtons'>true</b:widget-setting>
      <b:widget-setting name='authorLabel'>By</b:widget-setting>
      <b:widget-setting name='showCommentLink'>true</b:widget-setting>
      <b:widget-setting name='style.urlcolor'>#008000</b:widget-setting>
      <b:widget-setting name='showAuthor'>false</b:widget-setting>
      <b:widget-setting name='style.linkcolor'>#0000ff</b:widget-setting>
      <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
      <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
      <b:widget-setting name='showAuthorProfile'>false</b:widget-setting>
      <b:widget-setting name='style.layout'>1x1</b:widget-setting>
      <b:widget-setting name='showLabels'>true</b:widget-setting>
      <b:widget-setting name='showLocation'>false</b:widget-setting>
      <b:widget-setting name='showTimestamp'>true</b:widget-setting>
      <b:widget-setting name='postsPerAd'>1</b:widget-setting>
      <b:widget-setting name='showBacklinks'>false</b:widget-setting>
      <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
      <b:widget-setting name='showInlineAds'>false</b:widget-setting>
      <b:widget-setting name='showReactions'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main' var='top'>
	<b:if cond='data:blog.pageType == &quot;index&quot;'>
		
		<div class='items'>
			<b:loop values='data:posts' var='post'>
				<!-- insertamos entradas -->
        		<b:include data='post' name='post'/>
			</b:loop>
		</div>
	<b:else/>
      	<b:loop values='data:posts' var='post'>
		<div class='main-article'>
    		<div class='post'>
        		<article>
					<!-- insert -->
        			<b:include data='post' name='post'/>
		        </article>
    		</div>

		<b:include cond='data:blog.pageType == &quot;item&quot;' name='side-post'/>

		<!-- insertamos Comentarios -->
        <b:if cond='data:blog.pageType in {&quot;item&quot;, &quot;static_page&quot;}'>
		<div class='comentarios'>
		<b:if cond='data:post.allowComments'>
          <h4 class='comment-info'>Comments <span><data:post.numComments/></span></h4>
          <b:include data='post' name='comment_picker'/>
		<b:else/>
			<b:if cond='data:blog.pageType == &quot;item&quot;'>
          		<span class='info'>T-T Sorry, this entry is closed and does not allow comments.</span>
			</b:if>
		</b:if>

		</div>
        </b:if>

		</div>

      	</b:loop> 
	</b:if>

	<b:include cond='data:blog.pageType == &quot;index&quot;' name='paginacion'/>

    </b:includable>
    <b:includable id='backlinkDeleteIcon' var='backlink'><!--Vacío--></b:includable>
    <b:includable id='backlinks' var='post'><!--Vacío--></b:includable>
    <b:includable id='comment-form' var='post'>
  <div class='comment-form'>
    <a name='comment-form'/>
    <b:if cond='data:mobile'>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
    <b:else/>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
    </b:if>
    <data:post.friendConnectJs/>
    <data:post.cmtfpIframe/>
    <script type='text/javascript'>
      BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
    </script>
  </div>
</b:includable>
    <b:includable id='commentDeleteIcon' var='comment'>
  <span expr:class='&quot;item-control &quot; + data:comment.adminClass'>
    <b:if cond='data:showCmtPopup'>
      <div class='goog-toggle-button'>
        <div class='goog-inline-block comment-action-icon'/>
      </div>
    <b:else/>
      <a class='comment-delete' expr:href='data:comment.deleteUrl' expr:title='data:top.deleteCommentMsg'>
        <img src='https://resources.blogblog.com/img/icon_delete13.gif'/>
      </a>
    </b:if>
  </span>
</b:includable>
    <b:includable id='comment_count_picker' var='post'>
  <b:if cond='data:post.commentSource == 1'>
    <span class='cmt_count_iframe_holder' expr:data-count='data:post.numComments' expr:data-onclick='data:post.addCommentOnclick' expr:data-post-url='data:post.url' expr:data-url='data:post.canonicalUrl'>
    </span>
  <b:else/>
    <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
      <data:post.commentLabelFull/>:
    </a>
  </b:if>
</b:includable>
    <b:includable id='comment_fix'><script type='text/javascript'>
//<![CDATA[
var a=document.getElementsByClassName("avatar-image-container");for(i=0;i<a.length;i++)a[i].childNodes[0].setAttribute("src",a[i].childNodes[0].getAttribute("src").replace(/s\B\d{2,4}/,"s120-c"));
//]]>
	</script></b:includable>
    <b:includable id='comment_picker' var='post'>
  <b:if cond='data:post.commentSource == 1'>
    <b:include data='post' name='iframe_comments'/>
  <b:elseif cond='data:post.showThreadedComments'/>
    <b:include data='post' name='threaded_comments'/>
  <b:else/>
    <b:include data='post' name='comments'/>
  </b:if>
	<b:include cond='data:blog.pageType in {&quot;item&quot;, &quot;static_page&quot;}' name='comment_fix'/>
</b:includable>
    <b:includable id='comments' var='post'>
  <div class='comments' id='comments'>
    <a name='comments'/>
    <b:if cond='data:post.allowComments'>
      <b:if cond='data:post.commentPagingRequired'>
        <span class='paging-control-container'>
          <b:if cond='data:post.hasOlderLinks'>
            <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'><data:post.oldestLinkText/></a>
              &#160;
            <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'><data:post.olderLinkText/></a>
              &#160;
          </b:if>

          <data:post.commentRangeText/>

          <b:if cond='data:post.hasNewerLinks'>
            &#160;
            <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'><data:post.newerLinkText/></a>
            &#160;
            <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'><data:post.newestLinkText/></a>
          </b:if>
        </span>
      </b:if>

      <div expr:id='data:widget.instanceId + &quot;_comments-block-wrapper&quot;'>
        <dl expr:class='data:post.avatarIndentClass' id='comments-block'>
          <b:loop values='data:post.comments' var='comment'>
            <dt expr:class='&quot;comment-author &quot; + data:comment.authorClass' expr:id='data:comment.anchorName'>
              <b:if cond='data:comment.favicon'>
                <img expr:src='data:comment.favicon' height='16px' style='margin-bottom:-2px;' width='16px'/>
              </b:if>
              <a expr:name='data:comment.anchorName'/>
              <b:if cond='data:blog.enabledCommentProfileImages'>
                <data:comment.authorAvatarImage/>
              </b:if>
              <b:if cond='data:comment.authorUrl'>
                <a expr:href='data:comment.authorUrl' rel='nofollow'><data:comment.author/></a>
              <b:else/>
                <data:comment.author/>
              </b:if>
              <data:commentPostedByMsg/>
            </dt>
            <dd class='comment-body' expr:id='data:widget.instanceId + data:comment.cmtBodyIdPostfix'>
              <b:if cond='data:comment.isDeleted'>
                <span class='deleted-comment'><data:comment.body/></span>
              <b:else/>
                <p>
                  <data:comment.body/>
                </p>
              </b:if>
            </dd>
            <dd class='comment-footer'>
              <span class='comment-timestamp'>
                <a expr:href='data:comment.url' title='comment permalink'>
                  <data:comment.timestamp/>
                </a>
                <b:include data='comment' name='commentDeleteIcon'/>
              </span>
            </dd>
          </b:loop>
        </dl>
      </div>

      <b:if cond='data:post.commentPagingRequired'>
        <span class='paging-control-container'>
          <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'>
            <data:post.oldestLinkText/>
          </a>
          <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'>
            <data:post.olderLinkText/>
          </a>
          &#160;
          <data:post.commentRangeText/>
          &#160;
          <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'>
            <data:post.newerLinkText/>
          </a>
          <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'>
            <data:post.newestLinkText/>
          </a>
        </span>
      </b:if>

      <p class='comment-footer'>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='comment-form'/>
          <b:else/>
            <data:post.noNewCommentsText/>
          </b:if>
        <b:elseif cond='data:post.allowComments'/>
          <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a>
        </b:if>
      </p>
    </b:if>
    <b:if cond='data:showCmtPopup'>
      <div id='comment-popup'>
        <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
        </iframe>
      </div>
    </b:if>

    <div id='backlinks-container'>
    <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
       <b:include cond='data:post.showBacklinks' data='post' name='backlinks'/>
    </div>
    </div>
  </div>
</b:includable>
    <b:includable id='feedLinks'>
  <b:if cond='data:blog.pageType != &quot;item&quot;'> <!-- Blog feed links -->
    <b:if cond='data:feedLinks'>
      <div class='blog-feeds'>
        <b:include data='feedLinks' name='feedLinksBody'/>
      </div>
    </b:if>

    <b:else/> <!--Post feed links -->
    <div class='post-feeds'>
      <b:loop values='data:posts' var='post'>
        <b:if cond='data:post.allowComments'>
          <b:if cond='data:post.feedLinks'>
            <b:include data='post.feedLinks' name='feedLinksBody'/>
          </b:if>
        </b:if>
      </b:loop>
    </div>
  </b:if>
</b:includable>
    <b:includable id='feedLinksBody' var='links'>
  <div class='feed-links'>
  <data:feedLinksMsg/>
  <b:loop values='data:links' var='f'>
     <a class='feed-link' expr:href='data:f.url' expr:type='data:f.mimeType' target='_blank'><data:f.name/> (<data:f.feedType/>)</a>
  </b:loop>
  </div>
</b:includable>
    <b:includable id='iframe_comments' var='post'><b:if cond='data:post.allowIframeComments'><script expr:src='data:post.iframeCommentSrc' type='text/javascript'/><div class='cmt_iframe_holder' expr:data-href='data:post.canonicalUrl' expr:data-viewtype='data:post.viewType'/><b:if cond='data:post.embedCommentForm == &quot;false&quot;'><a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a></b:if></b:if></b:includable>
    <b:includable id='mobile-index-post' var='post'><!-- Vacío--></b:includable>
    <b:includable id='mobile-main' var='top'><!--Vacío--></b:includable>
    <b:includable id='mobile-nextprev'><!-- Vacío--></b:includable>
    <b:includable id='mobile-post' var='post'><!-- Vacío--></b:includable>
    <b:includable id='nextprev'><!--Vacío--></b:includable>
    <b:includable id='paginacion'>
	<div class='blog-pager'>
	<b:if cond='data:newerPageUrl'><a class='btn cyan newer-link ripple-effect' expr:href='data:newerPageUrl' expr:title='data:newerPageTitle'><i class='material-icons'>&#58820;</i> Previous Page</a></b:if>
	<b:if cond='data:olderPageUrl'><a class='btn cyan older-link ripple-effect' expr:href='data:olderPageUrl' expr:title='data:olderPageTitle'>Next Page <i class='material-icons'>arrow_forward</i></a></b:if>
	</div>
    </b:includable>
    <b:includable id='post' var='post'>
	<b:switch var='data:blog.pageType'>
      <b:case value='index'/><!--index-->

		

		<div class='item'>
            <a class='ripple-effect' expr:href='data:post.url' expr:title='data:post.title'>
			<b:if cond='data:post.thumbnailUrl'>
				<img expr:alt='data:post.title' expr:src='resizeImage(data:post.thumbnailUrl,380)' expr:title='data:post.title'/>
			<b:else/>
            	<b:if cond='data:post.firstImageUrl'>
					<img expr:alt='data:post.title' expr:src='data:post.firstImageUrl' expr:title='data:post.title'/>
				<b:else/>
				<!--si no hay imagen-->
					<img expr:alt='data:post.title' expr:title='data:post.title' src='https://goo.gl/HJ1nTG'/>
				</b:if>
			</b:if>
            </a>
            <div class='data'>
                <h2><a class='ripple-effect' expr:href='data:post.url' expr:title='data:post.title'><data:post.title/></a></h2>
                <div class='meta'>
                    <a class='ripple-effect' expr:href='data:post.authorProfileUrl' expr:title='data:post.author'>
                        <img expr:alt='data:post.author' expr:src='resizeImage(data:post.authorPhoto.url,35,&quot;1:1&quot;)'/>
                    </a>
                    <time class='published date updated' expr:datetime='data:post.timestampISO8601'><data:post.timestamp/></time>
                </div>
            </div>
		</div>

      <b:case value='item'/><!--item-->

       <!-- place Ad here -->
		<h1 class='title'><data:post.title/></h1>


<script>
      !function(d,s,id){
        var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?&#39;http&#39;:&#39;https&#39;;
        if(!d.getElementById(id)){
          js=d.createElement(s);
          js.id=id;
          js.src=p+&#39;://platform.twitter.com/widgets.js&#39;;fjs.parentNode.insertBefore(js,fjs);}}(document, &#39;script&#39;, &#39;twitter-wjs&#39;);
    </script>


<!-- place Ad here (below post title) -->
<style>
  .adbannerblock {display:block;width: 94.4%;height:90px;background: #e83a3a;text-align:center;margin: 8% auto 2%;}
    p.adbannertext {padding: 32px;font-size: 16px;color: #fff;font-weight: 300;text-align: center;}

@media screen and (max-width: 480px){
    .adbannerblock {widht:100%;margin: 15% auto 2%!important;}
  }
</style>

<!-- Remove above code and replace with your ad -->

		<div class='entry'><data:post.body/></div>

<!-- place Ad here (below post body) -->


<style>
* {
    box-sizing: border-box;
}
#bhero-cssanime:hover li { opacity:0.2; }
#bhero-cssanime li { -webkit-transition-property: opacity; -webkit-transition-duration: 500ms;-moz-transition-property: opacity; -moz-transition-duration: 500ms; }
#bhero-cssanime li a strong { opacity:0; -webkit-transition-property: opacity, top; -webkit-transition-duration: 300ms; -moz-transition-property: opacity, top; -moz-transition-duration: 300ms; }
#bhero-cssanime li:hover { opacity:1; }
#bhero-cssanime li:hover a strong { opacity:1; top:-10px; }
/* Mobile Responsive */
@media only screen and (max-width : 900px) {
ul.bhero-s1-social {
    margin: 6% 5%;
    float: none;
    padding: 0!important;}
li.bhero-s1 {
    width: 50px;
    height: 50px;
    margin: 5px;
    list-style: none;
    display: inline-block;
}
li.bhero-s1 {
  
    width: 55px;
    height: 55px;
}
}
@media only screen and (min-width : 900px) {

li.bhero-s1 {
    list-style-type: none;
    width: 50px;
    height: 50px;
    list-style: none;
    display: inline-block;
    margin: 2px;
}
}
/* START TOOLTIP STYLES */
[tooltip] {
  position: relative; /* opinion 1 */
}

/* Applies to all tooltips */
[tooltip]::before,
[tooltip]::after {
  text-transform: none; /* opinion 2 */
  font-size: 14px; /* opinion 3 */
  line-height: 1;
  user-select: none;
  pointer-events: none;
  position: absolute;
  display: none;
  opacity: 0;
}
[tooltip]::before {
  content: &#39;&#39;;
  border: 5px solid transparent; /* opinion 4 */
  z-index: 1001; /* absurdity 1 */
}
[tooltip]::after {
  content: attr(tooltip); /* magic! */
  
  /* most of the rest of this is opinion */
  font-family: Helvetica, sans-serif;
  text-align: center;
  
  /* 
    Let the content set the size of the tooltips 
    but this will also keep them from being obnoxious
    */
  min-width: 3em;
  max-width: 21em;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  padding: 1ch 1.5ch;
  border-radius: .3ch;
  box-shadow: 0 1em 2em -.5em rgba(0, 0, 0, 0.35);
  background: #333;
  color: #fff;
  z-index: 1000; /* absurdity 2 */
}

/* Make the tooltips respond to hover */
[tooltip]:hover::before,
[tooltip]:hover::after {
  display: block;
}
/* don&#39;t show empty tooltips */
[tooltip=&#39;&#39;]::before,
[tooltip=&#39;&#39;]::after {
  display: none !important;
}

/* FLOW: UP */
[tooltip]:not([flow])::before,
[tooltip][flow^=&quot;up&quot;]::before {
  bottom: calc(100% + 30px);
  border-bottom-width: 0;
  border-top-color: #333;
}
[tooltip]:not([flow])::after,
[tooltip][flow^=&quot;up&quot;]::after {
  bottom: calc(100% + 35px);
}
[tooltip]:not([flow])::before,
[tooltip]:not([flow])::after,
[tooltip][flow^=&quot;up&quot;]::before,
[tooltip][flow^=&quot;up&quot;]::after {
  left: 50%;
  transform: translate(-50%, -20px);
}
/* FLOW: DOWN */
[tooltip][flow^=&quot;down&quot;]::before {
  top: 100%;
  border-top-width: 0;
  border-bottom-color: #333;
}
[tooltip][flow^=&quot;down&quot;]::after {
  top: calc(100% + 5px);
}
[tooltip][flow^=&quot;down&quot;]::before,
[tooltip][flow^=&quot;down&quot;]::after {
  left: 50%;
  transform: translate(-50%, .5em);
}
/* FLOW: LEFT */
[tooltip][flow^=&quot;left&quot;]::before {
  top: 50%;
  border-right-width: 0;
  border-left-color: #333;
  left: calc(0em - 5px);
  transform: translate(-.5em, -50%);
}
[tooltip][flow^=&quot;left&quot;]::after {
  top: 50%;
  right: calc(100% + 5px);
  transform: translate(-.5em, -50%);
}
/* FLOW: RIGHT */
[tooltip][flow^=&quot;right&quot;]::before {
  top: 50%;
  border-left-width: 0;
  border-right-color: #333;
  right: calc(0em - 5px);
  transform: translate(.5em, -50%);
}
[tooltip][flow^=&quot;right&quot;]::after {
  top: 50%;
  left: calc(100% + 5px);
  transform: translate(.5em, -50%);
}
/* KEYFRAMES */
@keyframes tooltips-vert {
  to {
    opacity: .9;
    transform: translate(-50%, 0);
  }
}
@keyframes tooltips-horz {
  to {
    opacity: .9;
    transform: translate(0, -50%);
  }
}
/* FX All The Things */ 
[tooltip]:not([flow]):hover::before,
[tooltip]:not([flow]):hover::after,
[tooltip][flow^=&quot;up&quot;]:hover::before,
[tooltip][flow^=&quot;up&quot;]:hover::after,
[tooltip][flow^=&quot;down&quot;]:hover::before,
[tooltip][flow^=&quot;down&quot;]:hover::after {
  animation: tooltips-vert 300ms ease-out forwards;
}
[tooltip][flow^=&quot;left&quot;]:hover::before,
[tooltip][flow^=&quot;left&quot;]:hover::after,
[tooltip][flow^=&quot;right&quot;]:hover::before,
[tooltip][flow^=&quot;right&quot;]:hover::after {
  animation: tooltips-horz 300ms ease-out forwards;
}
</style>
<br/>

		<div class='meta ui'>
		Posted By :	<a expr:href='data:post.authorProfileUrl' expr:title='data:post.author'>
				<img expr:alt='data:post.author' expr:src='resizeImage(data:post.authorPhoto.url,35,&quot;1:1&quot;)'/>
			</a> Date : 
			<time class='published date updated' expr:datetime='data:post.timestampISO8601'><data:post.timestamp/></time>
			<div class='share uim'>
                <a class='fb' expr:href='&quot;https://www.facebook.com/sharer/sharer.php?u=&quot; + data:post.url' rel='nofollow' target='_blank'/>
                <a class='tt' expr:href='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url' rel='nofollow' target='_blank'/>
                <a class='gg' expr:href='&quot;https://plus.google.com/share?url=&quot; + data:post.url' rel='nofollow' target='_blank'/>
				<span class='openshare uib'><i class='material-icons'>share</i></span>
            </div>
		</div>

      <b:case value='static_page'/><!--static page-->

        <!--Soy una pagina independiente-->
		<h1 class='title'><data:post.title/></h1>
		<div class='entry'><data:post.body/></div>


	</b:switch>
	</b:includable>
    <b:includable id='postQuickEdit' var='post'><!--Vacío--></b:includable>
    <b:includable id='shareButtons' var='post'><!--vacio--></b:includable>
    <b:includable id='side-post'>
		<div class='side'><!--side-->

          	<!--// Add your own widgets
			<div class='widget'>
				<h2>Widget title</h2>
    			<div class='widget-content'>
					<!- content ->
  				</div>
  			</div>
			//-->

		</div><!--end side-->
	</b:includable>
    <b:includable id='status-message'><!--Vacío--></b:includable>
    <b:includable id='threaded-comment-form' var='post'>
  <div class='comment-form'>
    <a name='comment-form'/>
    <b:if cond='data:mobile'>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
    <b:else/>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
    </b:if>
    <data:post.cmtfpIframe/>
    <script type='text/javascript'>
      BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
    </script>
  </div>
</b:includable>
    <b:includable id='threaded_comment_js' var='post'>
  <script async='async' expr:src='data:post.commentSrc' type='text/javascript'/>

  <script type='text/javascript'>
    (function() {
      var items = <data:post.commentJso/>;
      var msgs = <data:post.commentMsgs/>;
      var config = <data:post.commentConfig/>;

// <![CDATA[
      var cursor = null;
      if (items && items.length > 0) {
        cursor = parseInt(items[items.length - 1].timestamp) + 1;
      }

      var bodyFromEntry = function(entry) {
        if (entry.gd$extendedProperty) {
          for (var k in entry.gd$extendedProperty) {
            if (entry.gd$extendedProperty[k].name == 'blogger.contentRemoved') {
              return '<span class="deleted-comment">' + entry.content.$t + '</span>';
            }
          }
        }
        return entry.content.$t;
      }

      var parse = function(data) {
        cursor = null;
        var comments = [];
        if (data && data.feed && data.feed.entry) {
          for (var i = 0, entry; entry = data.feed.entry[i]; i++) {
            var comment = {};
            // comment ID, parsed out of the original id format
            var id = /blog-(\d+).post-(\d+)/.exec(entry.id.$t);
            comment.id = id ? id[2] : null;
            comment.body = bodyFromEntry(entry);
            comment.timestamp = Date.parse(entry.published.$t) + '';
            if (entry.author && entry.author.constructor === Array) {
              var auth = entry.author[0];
              if (auth) {
                comment.author = {
                  name: (auth.name ? auth.name.$t : undefined),
                  profileUrl: (auth.uri ? auth.uri.$t : undefined),
                  avatarUrl: (auth.gd$image ? auth.gd$image.src : undefined)
                };
              }
            }
            if (entry.link) {
              if (entry.link[2]) {
                comment.link = comment.permalink = entry.link[2].href;
              }
              if (entry.link[3]) {
                var pid = /.*comments\/default\/(\d+)\?.*/.exec(entry.link[3].href);
                if (pid && pid[1]) {
                  comment.parentId = pid[1];
                }
              }
            }
            comment.deleteclass = 'item-control blog-admin';
            if (entry.gd$extendedProperty) {
              for (var k in entry.gd$extendedProperty) {
                if (entry.gd$extendedProperty[k].name == 'blogger.itemClass') {
                  comment.deleteclass += ' ' + entry.gd$extendedProperty[k].value;
                } else if (entry.gd$extendedProperty[k].name == 'blogger.displayTime') {
                  comment.displayTime = entry.gd$extendedProperty[k].value;
                }
              }
            }
            comments.push(comment);
          }
        }
        return comments;
      };

      var paginator = function(callback) {
        if (hasMore()) {
          var url = config.feed + '?alt=json&v=2&orderby=published&reverse=false&max-results=50';
          if (cursor) {
            url += '&published-min=' + new Date(cursor).toISOString();
          }
          window.bloggercomments = function(data) {
            var parsed = parse(data);
            cursor = parsed.length < 50 ? null
                : parseInt(parsed[parsed.length - 1].timestamp) + 1
            callback(parsed);
            window.bloggercomments = null;
          }
          url += '&callback=bloggercomments';
          var script = document.createElement('script');
          script.type = 'text/javascript';
          script.src = url;
          document.getElementsByTagName('head')[0].appendChild(script);
        }
      };
      var hasMore = function() {
        return !!cursor;
      };
      var getMeta = function(key, comment) {
        if ('iswriter' == key) {
          var matches = !!comment.author
              && comment.author.name == config.authorName
              && comment.author.profileUrl == config.authorUrl;
          return matches ? 'true' : '';
        } else if ('deletelink' == key) {
          return config.baseUri + '/delete-comment.g?blogID='
               + config.blogId + '&postID=' + comment.id;
        } else if ('deleteclass' == key) {
          return comment.deleteclass;
        }
        return '';
      };

      var replybox = null;
      var replyUrlParts = null;
      var replyParent = undefined;

      var onReply = function(commentId, domId) {
        if (replybox == null) {
          // lazily cache replybox, and adjust to suit this style:
          replybox = document.getElementById('comment-editor');
          if (replybox != null) {
            replybox.height = '250px';
            replybox.style.display = 'block';
            replyUrlParts = replybox.src.split('#');
          }
        }
        if (replybox && (commentId !== replyParent)) {
          replybox.src = '';
          document.getElementById(domId).insertBefore(replybox, null);
          replybox.src = replyUrlParts[0]
              + (commentId ? '&parentID=' + commentId : '')
              + '#' + replyUrlParts[1];
          replyParent = commentId;
        }
      };

      var hash = (window.location.hash || '#').substring(1);
      var startThread, targetComment;
      if (/^comment-form_/.test(hash)) {
        startThread = hash.substring('comment-form_'.length);
      } else if (/^c[0-9]+$/.test(hash)) {
        targetComment = hash.substring(1);
      }

      // Configure commenting API:
      var configJso = {
        'maxDepth': config.maxThreadDepth
      };
      var provider = {
        'id': config.postId,
        'data': items,
        'loadNext': paginator,
        'hasMore': hasMore,
        'getMeta': getMeta,
        'onReply': onReply,
        'rendered': true,
        'initComment': targetComment,
        'initReplyThread': startThread,
        'config': configJso,
        'messages': msgs
      };

      var render = function() {
        if (window.goog && window.goog.comments) {
          var holder = document.getElementById('comment-holder');
          window.goog.comments.render(holder, provider);
        }
      };

      // render now, or queue to render when library loads:
      if (window.goog && window.goog.comments) {
        render();
      } else {
        window.goog = window.goog || {};
        window.goog.comments = window.goog.comments || {};
        window.goog.comments.loadQueue = window.goog.comments.loadQueue || [];
        window.goog.comments.loadQueue.push(render);
      }
    })();
// ]]>
  </script>
</b:includable>
    <b:includable id='threaded_comments' var='post'>
  <div class='comments' id='comments'>
    <a name='comments'/>

    <div class='comments-content'>
      <b:include cond='data:post.embedCommentForm' data='post' name='threaded_comment_js'/>
      <div id='comment-holder'>
         <data:post.commentHtml/>
      </div>
    </div>

    <p class='comment-footer'>
      <b:if cond='data:post.allowNewComments'>
        <b:include data='post' name='threaded-comment-form'/>
      <b:else/>
        <span class='info'>T-T New comments are not allowed.</span>
      </b:if>
    </p>

    <b:if cond='data:showCmtPopup'>
      <div id='comment-popup'>
        <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
        </iframe>
      </div>
    </b:if>

    <div id='backlinks-container'>
    <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
      <b:include cond='data:post.showBacklinks' data='post' name='backlinks'/>
    </div>
    </div>
  </div>
</b:includable>
  </b:widget>
</b:section>

</div><!-- end content -->
</div><!-- end main -->

<footer>
<a class='btn floating cyan up ripple-effect' href='#'><i class='material-icons'>keyboard_arrow_up</i></a>
  <p class='credits'><a href='/'><data:blog.title/></a> &#169; 2018</p>
</footer>

<!--End Template-->


<script src='https://cdnjs.cloudflare.com/ajax/libs/headhesive/1.2.4/headhesive.min.js' type='text/javascript'/>
<script type='text/javascript'>
//<![CDATA[
var options={offset:'#md-show',classes:{clone:"md-clone",stick:"md-stick",unstick:"md-nostick"}},header=new Headhesive(".header",options);
//]]>
</script>

<b:if cond='data:blog.pageType == &quot;item&quot;'>
<script type='text/javascript'>
//<![CDATA[
  //!Autor: José Gregorio Materán | modificado: Daniel Abel
var h=document.querySelector(".share").children;i=0;for(t=h.length;i<t;i++)h[i].onclick=function(a){a.preventDefault();window.open(this.href,"btn-"+i,"width=800,height=400,left="+(screen.width/2-400)+",top="+(screen.height/2-200))};
//]]>
</script>
</b:if>

<b:if cond='data:blog.pageType == &quot;index&quot;'>
<script src='https://npmcdn.com/imagesloaded@4.1/imagesloaded.pkgd.min.js' type='text/javascript'/>
<script src='https://npmcdn.com/masonry-layout@4.1/dist/masonry.pkgd.min.js' type='text/javascript'/>
<script type='text/javascript'>
//<![CDATA[
var a=document.querySelector(".items");new Masonry(a,{a:0,b:0,c:".item"});var b=document.querySelector(".tops");new Masonry(b,{a:0,b:0,c:".item"});imagesLoaded(a,function(){new Masonry(a)});imagesLoaded(b,function(){new Masonry(b)});
//]]>
</script>
<b:else/>
<script type='text/javascript'>
//<![CDATA[
for(var a=[],b=document.querySelectorAll("article table th"),c=document.querySelector("article table tbody"),d=0;d<b.length;d++)a.push(b[d].textContent.replace(/\r?\n|\r/,""));for(var d=0,e;e=c.rows[d];d++)for(var f=0,g;g=e.cells[f];f++)g.setAttribute("data-in",a[f]);
//]]>
</script>
</b:if> 


<script type='text/javascript'>
/*<![CDATA[*/
//Facebook Script
(function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(d.getElementById(id))return;js=d.createElement(s);js.id=id;js.src="//connect.facebook.net/en_US/all.js#xfbml=1";fjs.parentNode.insertBefore(js,fjs)}(document,'script','facebook-jssdk'));
//Twitter Script
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src="https://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");
//Google Plus Script
(function(){var s=document.createElement('script');s.type='text/javascript';s.async=true;s.src='https://apis.google.com/js/plusone.js';var x=document.getElementsByTagName('script')[0];x.parentNode.insertBefore(s,x)})();
/*]]>*/
</script>



<!-- Theme Core Function Script -->
<script type='text/javascript'>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=&quot;https://platform.twitter.com/widgets.js&quot;;fjs.parentNode.insertBefore(js,fjs);}}(document,&quot;script&quot;,&quot;twitter-wjs&quot;);$(document)[&quot;\x72\x65\x61\x64\x79&quot;](function (){$(&quot;\x23\x63\x72\x65\x64\x69\x74&quot;)[&quot;\x68\x74\x6D\x6C&quot;]
(&quot;\x3C\x61\x20\x68\x72\x65\x66\x3D\x22\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x62\x6C\x6F\x67\x67\x65\x72\x68\x65\x72\x6F\x2E\x63\x6F\x6D\x2F\x22\x3E\x42\x6C\x6F\x67\x67\x65\x72\x48\x65\x72\x6F\x3C\x2F\x61\x3E&quot;);
setInterval(function (){if(!$(&quot;\x23\x63\x72\x65\x64\x69\x74\x3A\x76\x69\x73\x69\x62\x6C\x65&quot;)[&quot;\x6C\x65\x6E\x67\x74\x68&quot;]){window[&quot;\x6C\x6F\x63\x61\x74\x69\x6F\x6E&quot;][&quot;\x68\x72\x65\x66&quot;]=&quot;\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x62\x6C\x6F\x67\x67\x65\x72\x68\x65\x72\x6F\x2E\x63\x6F\x6D\x2F&quot;;} ;} ,3000);} );
</script>

<script type='text/javascript'>
//<![CDATA[
Array.prototype.forEach=function(b,c){var a=0;for(ii=this.length;a<ii;a++)a in this&&b.call(c,this[a],a,this)};
Array.prototype.slice.call(document.querySelectorAll(".ui")).forEach(function(a){var b=a.querySelector(".uib"),c=a.querySelector(".uim");b.onclick=function(a){c.className&&/(^|\s)active(\s|$)/.test(c.className)?(c.classList.remove("active"),c.classList.add("hide"),b.classList.remove("open"),b.classList.add("close"),a.preventDefault()):(c.classList.add("active"),c.classList.remove("hide"),b.classList.add("open"),b.classList.remove("close"),a.preventDefault())}});
//]]>
</script>
<!-- Google Analytics -->
<b:include data='blog' name='google-analytics'/>
</b:if> 

<script type='text/javascript'>
//<![CDATA[
//Double Click
for (var pres = document.querySelectorAll("blockquote,pre"), i = 0; i < pres.length; i++) pres[i].addEventListener("dblclick", function() {
  var e = getSelection(),
    t = document.createRange();
  t.selectNodeContents(this), e.removeAllRanges(), e.addRange(t)
}, !1);
//]]>
</script>
<style media='print' type='text/css'>
    * { display: none; }
</style>
<script type='text/javascript'>
//<![CDATA[
// Highlighter
$('i[rel="pre"]').replaceWith(function(){return $("<pre><code>"+$(this).html()+"</code></pre>")});for(var pres=document.querySelectorAll("pre,code,kbd,blockquote,td"),i=0;i<pres.length;i++)pres[i].addEventListener("dblclick",function(){var e=getSelection(),t=document.createRange();t.selectNodeContents(this),e.removeAllRanges(),e.addRange(t)},!1);
function downloadJSAtOnload(){var e=document.createElement("script");e.src="https://cdn.rawgit.com/Arlina-Design/frame/6c8ec00f/highlightr.js",document.body.appendChild(e)}window.addEventListener?window.addEventListener("load",downloadJSAtOnload,!1):window.attachEvent?window.attachEvent("onload",downloadJSAtOnload):window.onload=downloadJSAtOnload;
//]]>
</script>
&lt;!-- </body> --&gt;&lt;/body&gt;

</html>
