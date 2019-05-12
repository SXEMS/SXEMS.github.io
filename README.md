# SXEMS.github.io
<！DOCTYPE html>
<html xmlns =“http://www.w3.org/1999/xhtml”lang =“en”>
	<HEAD>
		<meta charset =“utf-8”/>
		<meta name =“description”content =“cmsmasters网站模板”/>
		<meta name =“keywords”content =“html，css，template”/>
		<link rel =“快捷图标”href =“images / favicon.png”type =“image / png”/>
		<link rel =“stylesheet”href =“css / style.css”type =“text / css”media =“screen”/>
		<link rel =“stylesheet”href =“css / styles / prettyPhoto.css”type =“text / css”media =“screen”/>
		<link id =“gFontName”rel =“stylesheet”href =“http://fonts.googleapis.com/css?family=Cuprum:regular,italic,bold,bolditalic”type =“text / css”/>
		<！ -  [if lt IE 9]>
			<link rel =“stylesheet”href =“css / styles / ie.css”type =“text / css”/>
		<！[ENDIF]  - >
		<TITLE>次元时光 - 轻刻年轮 - 记磊</ TITLE>
	<！ - 在MafiaShare.net上分享 - > <！ - 在MafiaShare.net上共享 - > </ head>
	<body class =“standard simple”>
		<script type =“text / javascript”> if（window.jQuery == undefined）document.write（unescape（'％3Cscript src =“js / jquery-1.6.4.min.js”type =“text / javascript” ％3E％3C / script％3E'））; </ SCRIPT>
		<script src =“js / jquery.prettyPhoto.js”type =“text / javascript”> </ script>
		<script src =“js / script.js”type =“text / javascript”> </ script>
		<script type =“text / javascript”>
			jQuery的（文件）。就绪（函数（）{
				if（jQuery.browser.msie && jQuery.browser.version <9）{
					var $ windowWidth = jQuery（window）.width（）+ 17;
					var $ windowHeight = jQuery（window）.height（）+ 17;
				} else {
					var $ windowWidth = window.innerWidth;
					var $ windowHeight = window.innerHeight;
				}
				
				jQuery（'body'）。append（'<div id =“preloaderMotion”/>'）;
				jQuery的（ 'a.header_arrow'）addClass（ '隐藏'）。
				
				var $ slider ='＃sliderMotion';
				var $ preloader ='＃preloaderMotion';
				var $ images = jQuery（$ slider +'li img'）;
				var $ max = $ images.length;
				
				$ images.each（函数（）{
					var img = new Image（）;
					
					img.src = jQuery（this）.attr（'src'）;
					
					var intervalId = setInterval（function（）{
						if（img.complete）{
							clearInterval（intervalId）;
							
							$ max--;
							
							jQuery（$ preloader）.append（'<img id =“nMotion'+ $ max +'”src =“'+ img.src +'”width =“60”height =“35”alt =“”/>'）;
							jQuery（$ preloader）.find（'img #nMotion'+ $ max）.animate（{opacity：1}，500）;
							
							if（$ max == 0）{
								LoadImageStart（jQuery的（$滑块））;
								jQuery（$ preloader）.fadeOut（500，function（）{
									jQuery的（本）的CSS（{显示： '无'}）;
									showHideContent（）;
								}）;
							}
						}
					}，50）;
				}）;
				
				function LoadImageStart（slider）{
					slider.cmsmsMotionSlider（{
						sliderWidth：$ WINDOWWIDTH，
						sliderHeight：$ WINDOWHEIGHT，
						pauseOnHover：假的，
						showPause：假
					}）;
					
					jQuery（'a [rel =“prettyPhoto [bgSlider]”]'）。prettyPhoto（{animationSpeed：'normal'，deeplinking：false，social_tools：false}）;
				}
				
				jQuery的（窗口）.resize（函数（）{
					if（jQuery.browser.msie && jQuery.browser.version <9）{
						var $ windowWidth = jQuery（window）.width（）+ 17;
						var $ windowHeight = jQuery（window）.height（）;
					} else {
						var $ windowWidth = window.innerWidth;
						var $ windowHeight = window.innerHeight;
					}
					
					jQuery（'。cmsmsMotionSliderContainer，.cmsmsMotionSlides，.cmsmsMotionSlides canvas，.cmsmsMotionSlides img，.cmsmsMotionSlides iframe'）。css（{width：$ windowWidth +'px'，height：$ windowHeight +'px'}）;
					。jQuery的（ 'cmsmsMotionControl '）的CSS（{高度：$ WINDOWHEIGHT +' 像素'}）;
					jQuery（'。cmsmsMotionNavigation'）。css（{height：parseInt（$ windowHeight  -  195）+'px'}）;
				}）;
			}）;
		</ SCRIPT>

<！ -  _________________________开始滑动__________________________  - >
		<ul id =“sliderMotion”>
			<li data-thumb =“images / slider / thumbs / img1.jpg”data-start =“左上角”data-finish =“右下角”data-zoom =“out”data-animation =“10”>
				<img src =“images / slider / img1.jpg”alt =“横幅图1”/>
                <div class =“cmsmsSlideCaption”data-top =“50”>
					<H2>次元时光导航</ H2>
					<p>记磊博客成立于2017年六一儿童节，目标是<不忘初心的个人博客>，并在为此努力的路上。我们分享来自全球的热门资源，无门槛下载资源给你最佳的体验。</ p>
					<a href="https://www.ly522.com/ class="button btn_1">点击进入记磊博客</a>
				</ DIV>
			</ LI>
			<li data-thumb =“images / slider / thumbs / img2.jpg”data-start =“bottom center”data-finish =“center center”data-zoom =“in”data-animation =“15”>
				<a class="video autostop hd"> <img src =“images / slider / img2.jpg”alt =“Banner Image 2”/>
					
			</ LI>
			<li data-thumb =“images / slider / thumbs / img3.jpg”data-start =“右下角”data-finish =“左下角”data-zoom =“out”>
				<img src =“images / slider / img3.jpg”alt =“Banner Image 3”/>
				
					
			</ LI>
			<li data-thumb =“images / slider / thumbs / img4.jpg”data-start =“center center”data-finish =“center center”data-zoom =“in”>
				<a class="video autostop hd"> <img src =“images / slider / img4.jpg”alt =“Banner Image 4”/> </a>
			
					
            </ LI>
			<li data-thumb =“images / slider / thumbs / img5.jpg”data-start =“center left”data-finish =“top right”data-zoom =“out”data-animation =“15”>
				<img src =“images / slider / img5.jpg”alt =“Banner Image 5”/>
                
			</ LI>
		</ UL>
<！ -  _________________________完成滑块__________________________  - >


<！ -  _________________________首页___________________________  - >
		<div id =“page”class =“hideContent”>

<！ -  _________________________开始标题_________________________  - >
			<div class =“header_wrap”>
				<div id =“header”>
					<div class =“header_inner”>
						<a class="logo" title="Pacifico" href="index.html">
							<img alt =“Pacifico”src =“images / logo.png”/>
							
                            <audio autoplay =“autoplay”> <source src =“/ mengzhan.mp3”type =“audio / mpeg”/> </ audio>

						</A>
						
<！ -  _________________________开始导航_____________________  - >
						<div class =“navigation_wrap”>
							<ul id =“navigation”>
                            点击
                            点击
								<li> <a href="about.html">关于<span>关于</ span> </a> </ li>
								<li> <a href="https://www.ly522.com/">进入博客<span>博客</ span> </a>
									
								</ LI>
								<li> <a href="https://img.ly522.com">次元图床<span> pic moe </ span> </a>
									
								</ LI>
								<li> <a href="https://web.ly522.com">导航网<span> web </ span> </a>
								
								</ LI>
								<li> <a href="http://wpa.qq.com/msgrd?v=3&uin=68213803&site=qq&menu=yes">联系笨站长<span>爱我</ span> </a> </ LI>
							</ UL>
                        </ DIV>
<！ -  _________________________完成导航____________________  - >

					</ DIV>
					<div class =“header_arrow_wrap”>
						<a href="#" class="header_arrow"> <span>＆nbsp; </ span> </a>
					</ DIV>
				</ DIV>
			</ DIV>
<！ -  _________________________完成标题________________________  - >

		</ DIV>
<！ -  _________________________完成页面__________________________  - >

	</ BODY>
</ HTML>
