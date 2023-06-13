<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:version='2' class='v2' expr:dir='data:blog.languageDirection' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>

    <!--Title-->
    <b:if cond='data:blog.pageType == &quot;index&quot;'>
      <title><data:blog.pageTitle/></title>
      <b:else/>
      <b:if cond='data:blog.pageType != &quot;error_page&quot;'>
        <title><data:blog.pageName/> - <data:blog.title/></title>
      </b:if></b:if>
    <b:if cond='data:blog.pageType == &quot;error_page&quot;'>
      <title>Page Not Found - <data:blog.title/></title>
    </b:if>

    <!--META-->
    <meta charset='utf-8'/>
    <meta content='width' name='MobileOptimized'/>
    <meta content='true' name='HandheldFriendly'/>
    <meta content='yes' name='apple-mobile-web-app-capable'/>
    <meta content='index,nofollow' name='robots'/>
    <meta content='width=device-width, initial-scale=1, maximum-scale=1' name='viewport'/>

    <!-- Blogger main head data and meta -->
    <b:include data='blog' name='all-head-content'/>

    <!-- BOOTSTRAP -->
    <link href='https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css' rel='stylesheet'/>
    <link crossorigin='anonymous' href='https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta/css/bootstrap.min.css' integrity='sha384-/Y6pD6FV/Vv2HJnA6t+vslU6fwYXjCFtcEpHbNJ0lyAFsXTsjBbfaDjzALeQsN6M' rel='stylesheet'/>

    <b:skin><![CDATA[
/* Variable definitions
====================

<Group description="Shutter Theme Basic" selector="body">

<Variable name="body.background" description="Dark Color" type="color" default="#222222" value="#222222"/>
<Variable name="body.text.color" description="Text Color" type="color" default="#ffffff" value="#ffffff"/>
<Variable name="body.link.color" description="Primary Color" type="color" default="#0275c6" value="#0275c6"/>
</Group>

*/

/* GLOBAL */
html,body{color:$(body.text.color);font-family: 'Raleway', sans-serif;}
body, body > .wrapper{background:$(body.background);}
body.hidescroll{background:#ccc}
a{color:$(body.text.color);}
a:hover{color:$(body.link.color);}
aside{max-width: 330px;margin:0 auto;}
img{max-width: 100%;}
a:hover{text-decoration: none}
.post-body{font-size:14px;letter-spacing:.2px;}
.post-body blockquote{background: $(body.link.color);padding:20px 25px;font-weight:400;position:relative;color:$(body.text.color);margin:10px 0px;opacity:1;}
.post-body ul{list-style-type: square;}
.post-body{line-height: 1.5;letter-spacing:0.3px;margin-bottom:15px;}
.post-body img{padding: 5px 0px;}
.post-body code a{color:$(body.background)}
hr{border-color: rgba(255,255,255,0.5);}

/* Layout */
.topmenu{display: none;}
.content-area{box-sizing: border-box;padding-left: 320px;}
.nav-sidebar-area{position: fixed;width: 320px; border-right: 1px solid $(body.link.color);/*rgba(255,255,255,0.1)*/;z-index: 999;bottom: 0;top:0;left: 0;background:$(body.background);}
.nav-sidebar-area .nav-sbar-inner .nav-outer-table{display: table;width: 100%;height: 100%;box-sizing: border-box;padding: 10px;}
.nav-sidebar-area .nav-sbar-inner .nav-inner-cell{display: table-cell;vertical-align: middle;}
.nav-sidebar-area .nav-sbar-inner{position: absolute;top:0px;width: 100%;bottom: 0px;left: 0px;}
h1.title{text-align: center;font-weight: 700;text-transform: uppercase;position:relative;border-bottom:2px solid transperent;}
h1.title:after{content: "";height:2px;width: 80%;background:$(body.link.color);bottom:0px;margin: 10px auto;display:table;}
#tilting{min-height:100vh}
#right-sidebar-area .column-right-outer{z-index: 1}
#left-sidebar-area .column-left-outer{z-index: 1}
.addpad{padding-top:30px;}
.Header img{max-height: 150px;max-width:180px;}
.topmenu .Header img{max-height:50px;max-width:180px;}
.nav-sidebar-area .Header img{margin: 0 auto;border-bottom:2px solid $(body.link.color);margin-bottom:10px;}

/*Nav Menu*/
#navmenu ul{list-style-type: none;padding: 0px;text-align: right}
#navmenu > ul{margin-right: 10%;}
#navmenu ul li{padding: 0px;position:relative;}
#navmenu ul li a{font-size:14px;padding:5px 0px;display: block;text-transform: uppercase;font-weight: 700;}
#navmenu ul ul{position:absolute;left:100%;width:100%;background:$(body.text.color);color:$(body.background);display: table;padding: 10px 20px;margin-left:20px;top:0px}
#navmenu ul ul a{text-align: left;color: $(body.background);}
#navmenu ul li > a.sf-with-ul:after{content: "";font-family: "Ionicons";padding:0px 19px;position: absolute;}
#navmenu ul  ul li > a.sf-with-ul:after{content: "\f10b";font-family: "Ionicons";padding:0px 4px;position: absolute;right: 0px;}
/* #navmenu ul ul:before{content: "";display: table;position: absolute;background: $(body.link.color);left: 0px;width: 2px;top:0px;bottom:0px;height: 100%;}*/
#navmenu > ul > li:hover a{color: $(body.text.color);text-decoration:none;}
#navmenu > ul > li:after{content: "";position: absolute;right: -2px;background: $(body.link.color);width: 2px;display: block;height:0%;bottom:0px;margin:0 -6px;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
#navmenu > ul > li:hover:after{height: 100%;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
#navmenu > ul li:hover ul li a{color: $(body.background)}
#navmenu > ul li:hover ul li{color: $(body.background)}

/*responsive navigation*/
.responsive-nav ul{list-style-type: none;padding: 0px;margin: 0px;padding-left:20px;}
.responsive-nav ul li{padding: 0px;}
.responsive-nav ul li a{font-weight: 700;font-size:12px;padding:3px 0px;display:block;text-transform: uppercase;}
.responsive-nav ul li ul li a:before{content:"\f10b";font-family: "Ionicons";font-size:15px;padding-right: 10px;}
.responsive-nav ul ul{padding-left: 15px;}
.responsive-nav{display: none}
.nav-sidebar-area.open{transform: translateX(0px);transition:.3s all ease-in-out;-moz-transition:.3s all ease-in-out;-o-transition:.3s all ease-in-out;-ms-transition:.3s all ease-in-out;-webkit-transition:.3s all ease-in-out;}
.nav-sidebar-area.open a.search-button{display: none}
.nav-sidebar-area.open a.toggle-button{display: block !important;position: absolute;top: 0px;right: 0px;width: 30px;height: 30px;text-align: center;line-height: 30px;font-size: 20px;background: $(body.link.color);}
.nav-sidebar-area{transition:.3s all ease-in-out;-moz-transition:.3s all ease-in-out;-o-transition:.3s all ease-in-out;-ms-transition:.3s all ease-in-out;-webkit-transition:.3s all ease-in-out;}

/*MEGA MENU*/
.shutter-mega-list{position: static !important;}
#navmenu ul .shutter-mega-list ul.mega-list{position: absolute;top: 0px;height: 100%;left:100%;display:none;margin-left:0px !important;padding:0px !important}
.nlink .LinkList{position: static !important;}
.shutter-mega-list:after{display: none !important;}
.upnav,.downnav{width:100%;text-align:center !important;background:$(body.link.color);color:$(body.text.color) !important;height:30px;opacity:0.8;}
.upnav:hover, .downnav:hover{opacity:1;}
.upnav{position: absolute;top:0px;left:0px;}
.downnav{position: absolute;bottom: 0px;left: 0px;}
.mega-list li{position: relative;height: 100%;display:table;width:100%;}
.mega-list{max-width: 260px;display:none}
.nav-disable{background: #ddd !important;}
.items-shutter {box-sizing: border-box;padding:30px 0px;height:100%;display:table;width: 100%;overflow-y: scroll}
.item-shutter-table{display: table-cell;vertical-align: middle;text-align: center}
.shutter-m-thumb{display: table;height: 100%;width: 100%;background-size:cover !important;background-position:center center !important;}
.mega-list .shutter-mega-item{height: 25%;display: table;width: 100%;position:relative;box-sizing:border-box;padding:0px 0px;}
.item-shutter-cell{display: table;height: 100%;width: 100%;}
.shutter-mega-item a{display: table;height: 100%;width: 100%;}
.shutter-text{position: absolute;bottom:20px;left:10px;}
.shutter-text a{color: $(body.text.color) !important;font-size:14px !important;text-transform: initial !important;font-weight: 600 !important;}
.shutter-mega-item{overflow:hidden;}
.shutter-mega-item .shutter-m-thumb{transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.shutter-mega-item:hover .shutter-m-thumb{transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.shutter-m-thumb::after{content: "";position: absolute;top: 0px;bottom: 0px;left: 0px;right: 0px;background: #000;opacity: 0;}
.shutter-mega-item:hover .shutter-m-thumb::after{opacity: 0.5}
.shutter-text{filter: blur(10px);opacity: 0;transition:all .6s ease;-moz-transition:all .6s ease;-o-transition:all .6s ease;-webkit-transition:all .6s ease;-ms-transition:all .6s ease;}
.shutter-mega-item:hover .shutter-text{filter: blur(0px);opacity: 1}

/*Mega Menu Loading Effect*/
.shutter-mega-loadingwrapper{top:0px;bottom:0px;background:$(body.text.color);left:0px;right:0px;height:100%;width:100%;display:table;}
.shutter-loading-table{display: table-cell;width: 100%;height: 100%;vertical-align: middle;}
.shutter-loading{background:rgb(255,255,255);color:rgb(2,116,198);font:28px "Helvetica Neue", sans-serif;line-height:175px;margin:175px auto;text-align:center;position:relative;width:100%;display:block;height:25px;position:relative;width:25px;}
.shutter-loading::before, .shutter-loading::after{position:absolute;font-smoothing:none;-o-font-smoothing:none;-ms-font-smoothing:none;-webkit-font-smoothing:none;-moz-font-smoothing:none;}
.shutter-loading::before{animation:cssload-spin 1.15s linear infinite;-o-animation:cssload-spin 1.15s linear infinite;-ms-animation:cssload-spin 1.15s linear infinite;-webkit-animation:cssload-spin 1.15s linear infinite;-moz-animation:cssload-spin 1.15s linear infinite;animation-direction:alternate;box-shadow:0 0 0 2px rgb(2,116,198);color:rgb(255,255,255);content:"+";font-size:186px;height:46px;line-height:0;left:0;top:0;text-indent:-30px;transform-origin:50% 50%;-o-transform-origin:50% 50%;-ms-transform-origin:50% 50%;-webkit-transform-origin:50% 50%;-moz-transform-origin:50% 50%;width:46px;}
.shutter-loading::after{content:"";background:rgb(2,116,198);height:25px;width:25px;position:absolute;top:11px;left:11px;}
@keyframes cssload-spin{0%{transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{transform:scale(1) rotate(270deg) translateZ(0);}
}
@-o-keyframes cssload-spin{0%{-o-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-o-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-o-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-o-transform:scale(1) rotate(270deg) translateZ(0);}
}
@-ms-keyframes cssload-spin{0%{-ms-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-ms-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-ms-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-ms-transform:scale(1) rotate(270deg) translateZ(0);}
}
@-webkit-keyframes cssload-spin{0%{-webkit-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-webkit-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-webkit-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-webkit-transform:scale(1) rotate(270deg) translateZ(0);}
}
@-moz-keyframes cssload-spin{0%{-moz-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-moz-transform:scale(1.4) rotate(-90deg) translateZ(0);}
30%, 45%{-moz-transform:scale(1.4) rotate(-270deg) translateZ(0);}
55%, 100%{-moz-transform:scale(1) rotate(-3600deg) translateZ(0);}
}

/* Nav Social */
.nav-social ul{list-style-type: none;margin-right:10%;margin-top:20px;}
.nav-social ul li{float: right;}
.nav-social ul li a{font-size:12px;border:1px solid $(body.text.color);margin:0px 4px;display: table;width: 30px;height: 25px;text-align: center;line-height: 25px;}
.nav-social ul li a:hover{color: $(body.text.color);background: $(body.link.color);border:1px solid $(body.link.color)}

/* search*/
.search-button{position: absolute;top:0px;right: 0px;width: 30px;height: 30px;text-align: center;line-height: 30px;font-size:20px;background: $(body.link.color);}
.search-button:hover{color: $(body.text.color);}
#tilting.searchopen{transform: perspective(1000px) translate3d(0,15%,0) rotate3d(1,0,0,30deg);transition:.4s all ease-in-out;-moz-transition:.4s all ease-in-out;-o-transition:.4s all ease-in-out;-ms-transition:.4s all ease-in-out;-webkit-transition:.4s all ease-in-out;}
#tilting{transition:.4s all ease-in-out;-moz-transition:.4s all ease-in-out;-o-transition:.4s all ease-in-out;-ms-transition:.4s all ease-in-out;-webkit-transition:.4s all ease-in-out;}
body > .wrapper{background: $(body.background)}
.hidescroll{overflow: hidden}
#btn-search-close svg{width: 30px;height: 30px;font-size: 20px;}
#btn-search-close{position: fixed;right: 10px;top:10px;background: transparent}
.search__form{text-align: center;}
.search__form input{font-size: 30px;background: transparent;border: 0px;color: $(body.background);font-weight: 600;padding: 10px;margin-top:40px;border-bottom: 2px solid $(body.background);width: 60%;}
.search__form .search__info{clear: left;width: 60%;padding:10px 0px;text-align:right;display:table;margin-left: 20%;color:$(body.background);text-transform: uppercase;}
/*.hidescroll #tilting{display: none;}*/
.hidescroll{position:fixed;transition:.4s all ease-in-out;-moz-transition:.4s all ease-in-out;-o-transition:.4s all ease-in-out;-ms-transition:.4s all ease-in-out;-webkit-transition:.4s all ease-in-out;}

/*GRID FIX*/
.column-left-outer{margin-left:0px !important;}
#left-sidebar-area >  div,#right-sidebar-area > div{margin: 0 auto !important;float: none !important}
body{font-size:12px;transition:.4s all ease-in-out;-moz-transition:.4s all ease-in-out;-o-transition:.4s all ease-in-out;-ms-transition:.4s all ease-in-out;-webkit-transition:.4s all ease-in-out;}

/*owl slider*/
/** * Owl Carousel v2.2.1 * Copyright 2013-2017 David Deutsch * Licensed under () *//* * Owl Carousel - Core */.owl-carousel{display:none;width:100%;-webkit-tap-highlight-color:transparent;position:relative;z-index:1;}
.owl-carousel .owl-stage{position:relative;-ms-touch-action:pan-Y;-moz-backface-visibility:hidden;}
.owl-carousel .owl-stage:after{content:".";display:block;clear:both;visibility:hidden;line-height:0;height:0;}
.owl-carousel .owl-stage-outer{position:relative;overflow:hidden;-webkit-transform:translate3d(0px, 0px, 0px);}
.owl-carousel .owl-wrapper, .owl-carousel .owl-item{-webkit-backface-visibility:hidden;-moz-backface-visibility:hidden;-ms-backface-visibility:hidden;-webkit-transform:translate3d(0, 0, 0);-moz-transform:translate3d(0, 0, 0);-ms-transform:translate3d(0, 0, 0);}
.owl-carousel .owl-item{position:relative;min-height:1px;float:left;-webkit-backface-visibility:hidden;-webkit-tap-highlight-color:transparent;-webkit-touch-callout:none;}
.owl-carousel .owl-item img{display:block;width:100%;}
.owl-carousel .owl-nav.disabled, .owl-carousel .owl-dots.disabled{display:none;}
.owl-carousel .owl-nav .owl-prev, .owl-carousel .owl-nav .owl-next, .owl-carousel .owl-dot{cursor:pointer;cursor:hand;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}
.owl-carousel.owl-loaded{display:block;}
.owl-carousel.owl-loading{opacity:0;display:block;}
.owl-carousel.owl-hidden{opacity:0;}
.owl-carousel.owl-refresh .owl-item{visibility:hidden;}
.owl-carousel.owl-drag .owl-item{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}
.owl-carousel.owl-grab{cursor:move;cursor:grab;}
.owl-carousel.owl-rtl{direction:rtl;}
.owl-carousel.owl-rtl .owl-item{float:right;}
.no-js .owl-carousel{display:block;}
/* * Owl Carousel - Animate Plugin */.owl-carousel .animated{animation-duration:1000ms;animation-fill-mode:both;}
.owl-carousel .owl-animated-in{z-index:0;}
.owl-carousel .owl-animated-out{z-index:1;}
.owl-carousel .fadeOut{animation-name:fadeOut;}
@keyframes fadeOut{0%{opacity:1;}
100%{opacity:0;}
}
/* * Owl Carousel - Auto Height Plugin */.owl-height{transition:height 500ms ease-in-out;}
/* * Owl Carousel - Lazy Load Plugin */.owl-carousel .owl-item .owl-lazy{opacity:0;transition:opacity 400ms ease;}
.owl-carousel .owl-item img.owl-lazy{transform-style:preserve-3d;}
/* * Owl Carousel - Video Plugin */.owl-carousel .owl-video-wrapper{position:relative;height:100%;background:#000;}
.owl-carousel .owl-video-play-icon{position:absolute;height:80px;width:80px;left:50%;top:50%;margin-left:-40px;margin-top:-40px;background:url("owl.video.play.png") no-repeat;cursor:pointer;z-index:1;-webkit-backface-visibility:hidden;transition:transform 100ms ease;}
.owl-carousel .owl-video-play-icon:hover{-ms-transform:scale(1.3, 1.3);transform:scale(1.3, 1.3);}
.owl-carousel .owl-video-playing .owl-video-tn,.owl-carousel .owl-video-playing .owl-video-play-icon{display:none;}
.owl-carousel .owl-video-tn{opacity:0;height:100%;background-position:center center;background-repeat:no-repeat;background-size:contain;transition:opacity 400ms ease;}
.owl-carousel .owl-video-frame{position:relative;z-index:1;height:100%;width:100%;}


/*slider*/
.hidepad{padding:0px !important}
.slide .slide-wrapper{height: 100%;width: 100%;background-size: cover !important;background-position: center center !important;}
.slide-inner{height: 100%;width: 100%;display: table;}
.slide-box{position:absolute;left:40px;bottom:10%;}
.slide{position: relative;}
.slidebox-inner, .slide-title ,.slide-title h3, .slide-meta {display: block !important;}
.slidebox-inner{box-sizing: border-box;padding: 20px 25px;background: $(body.link.color);}
.slider-wrapper{margin-bottom: 30px;}
.slide-title h3{font-size: 35px;font-weight:700;}
.owl-nav > div{position: absolute;top:40%}
.owl-nav .owl-prev{left: 0px;}
.owl-nav .owl-next{right: 0px;}
.owl-nav i{font-size:30px;display: table;height: 40px;width: 40px;border: 1px solid $(body.text.color);line-height: 40px;text-align: center;opacity: 0.6;position:absolute;left:20px;top:50%}
.owl-nav > div > div:hover i{background: $(body.link.color);border: $(body.link.color);opacity: 1;}
.owl-nav .prev-slider-shutter{box-sizing: border-box;padding-top: 50px;padding-left: 30px;padding-bottom: 50px;padding-right: 90px;position:relative;cursor:none}
.owl-nav .next-slider-shutter{box-sizing: border-box;padding-top: 50px;padding-left: 130px;padding-bottom: 50px;padding-right: 30px;position:relative;cursor:none}
.slide h3 a:hover{color: $(body.text.color)}
.slide .slide-box{max-width: 40%;}
.slide-category a{text-transform: uppercase;border:1px solid $(body.text.color);padding: 4px 6px;margin-bottom: 10px;display: inline-block}
.slide-category a:hover{background: $(body.text.color);border-color:$(body.text.color);text-decoration: none}

/*Packery*/
.shutter-two-sidebar .grid-sizer, .shutter-two-sidebar .grid-item{width:50%;position:relative;}
.shutter-one-sidebar .grid-item{width:33.33%;position:relative;}
.shutter-no-sidebar .grid-item{width:25%;position:relative;}

/*Post Deafult*/
.grid-item .dlayout .item-content{position: absolute;top:50%;left: 50%;-moz-transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);-webkit-transform: translate(-50%, -50%);-o-transform: translate(-50%, -50%);transform: translate(-50%, -50%);width: 80% !important;filter: blur(10px);transition: all .6s ease;-moz-transition: all .6s ease;-o-transition: all .6s ease;-webkit-transition: all .6s ease;-ms-transition: all .6s ease;text-align: center;opacity:0}
.grid-item:hover .dlayout .item-content{filter:blur(0px);opacity:1}
.grid-item .cover:after{content: "";position: absolute;top:0px;left: 0px;background:$(body.background);opacity: 0.5;right: 0px;bottom:0px;height: 100%;width: 100%;display: block}
.grid-item .cover{display: block;height: 100%;width: 100%;position: absolute;left: 0px;right: 0px; opacity:0}
.grid-item:hover .cover{opacity: 1}
.grid-item h3 {border-bottom: 1px solid rgba(255,255,255,0.1);padding-bottom: 5px;}
.grid-item h3 a:hover{color: $(body.text.color);}
.grid-item{box-sizing: border-box;padding: 10px;opacity:0}
.grid-item.inline-ad{padding: 0px !important;margin: 0px !important;}
.ad-content > * {margin: 0 auto;padding: 10px;box-sizing: border-box;}
.grid-item img{max-width: 100%;min-width: 100%;}
a.linkmask{position: absolute;display: block;left:0px;top:0px;height: 100%;width: 100%;z-index:10}

/*.noapply{opacity:0}*/
.visible{opacity:1}
/*Sidebars*/
.widget > h2{text-align: ;margin: 0px 0px;padding: 0px 0px;font-size:22px;font-weight:600;}
.widget > h2:after{content: "";height: 2px;width: 100%;background: $(body.link.color);bottom: 0px;margin: 10px 0;display: table}

/*Featured Post*/
.FeaturedPost.widget{padding: 0px;}
.FeaturedPost img{display: none}
.FeaturedPost .post-summary{background-size: cover;box-sizing: border-box;padding:20px 30px;background-position: center center; position:relative;background-color:#151515}
.FeaturedPost .post-summary h3{padding-top:80%;z-index:2;position: relative;}
.FeaturedPost .post-summary p{z-index:2;position: relative;}
.FeaturedPost .post-summary a,.FeaturedPost .post-summary {color:$(body.text.color);}
.FeaturedPost a:hover{color:#ccc}
.FeaturedPost .overlay{position: absolute;left: 0px;top:0px;height: 100%;width: 100%;background: rgba(0,0,0,0.2);z-index: 1;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.FeaturedPost:hover .overlay{position: absolute;left: 0px;top:0px;height: 100%;width: 100%;background: rgba(0,0,0,0.5);z-index: 1;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.FeaturedPost h2.title{margin-bottom: 0px !important;}
.FeaturedPost > h2:after{margin-bottom: 0px !important;}

/*Navigation*/
.feed-links{display: none}

/*Arrow Navigation*/
.shutter-pager.arrow{text-align:center;margin:20px 20px;}
.shutter-pager.arrow #shutter-new{float: left;display:table;}
.shutter-pager.arrow #shutter-old{float: right;display: table;}
.shutter-pager.arrow a{border:1px solid $(body.text.color);padding: 10px 17px;color:$(body.text.color)}
.shutter-pager.arrow #shutter-new a{float: left;display:table;}
.shutter-pager.arrow #shutter-old a{float: right;display: table;}
.shutter-pager.arrow .shutter-home{display: table;margin: 0px auto;}
.shutter-pager.arrow a:hover{background:$(body.link.color);border-color:$(body.link.color);color:$(body.text.color)}
.shutter-pager.arrow a i{font-size:16px;}

/*number nav*/
#shutter-pager span{float: left}
#shutter-pager{display:block;padding:5px 0;margin-top:20px;}
.showpage a, .pagenumber a, .current{position:relative;display:inline-block;padding:5px 11px !important;line-height:21px;margin:0 2px;border:1px solid #dcdcdc;color:$(body.text.color);font-size:16px;transition:.3s all ease-in-out;-moz-transition:.3s all ease-in-out;-o-transition:.3s all ease-in-out;-ms-transition:.3s all ease-in-out;-webkit-transition:.3s all ease-in-out;;min-width:33px;text-align:center;}
.showpage a:hover, .pagenumber a:hover, .current{background:$(body.link.color);border:1px solid $(body.link.color);color:$(body.text.color)fff;text-decoration:none;}
.current{color:$(body.text.color);background:$(body.link.color);border-color:$(body.link.color);}
#shutter-pager .totalpages{text-align:left;float:right;padding:5px 11px;display:inline-block;font-size:16px;font-weight:500;color:$(body.text.color);line-height:21px;}

/*infinite loading*/
.shutter-loadmore a{margin:20px auto;text-align:center;border:1px solid $(body.text.color);padding:10px 30px;font-weight:700;font-size:20px;display:inline-block;min-width:300px;max-width:300px;}
.shutter-loadmore{text-align:center;}
.shutter-loadmore a:hover{text-decoration:none;color:$(body.text.color);border-color:$(body.link.color);background-color:$(body.link.color)}
.shutter-loadmore a:active,.shutter-loadmore a:visited, .shutter-loadmore a:link{color: $(body.text.color);text-decoration: none}
.shutter-infinite-loading{display:block;width:100%;position:relative;}
.shutter-infinite-loading .shttr-thecube{padding:0px !important;margin:0px auto !important;background:$(body.text.color);display:inline-block;position:relative;overflow:hidden;width:40%;min-width:300px;max-width:300px;}
.shutter-loadmore a.disable:hover{background: transparent;border-color:$(body.text.color) }
.shttr-cube.shttr-c1{background:rgb(255,255,255);color:rgb(2,116,198);font:16px "Helvetica Neue", sans-serif;line-height:97px;margin:20px auto;text-align:center;position:relative;width:100%;display:block;height:14px;position:relative;width:14px;}
.shttr-cube.shttr-c1::before, .shttr-cube.shttr-c1::after{position:absolute;font-smoothing:none;-o-font-smoothing:none;-ms-font-smoothing:none;-webkit-font-smoothing:none;-moz-font-smoothing:none;}
.shttr-cube.shttr-c1::before{animation:cssload-spin 1.15s linear infinite;-o-animation:cssload-spin 1.15s linear infinite;-ms-animation:cssload-spin 1.15s linear infinite;-webkit-animation:cssload-spin 1.15s linear infinite;-moz-animation:cssload-spin 1.15s linear infinite;box-shadow:0 0 0 1px rgb(2,116,198);color:rgb(255,255,255);content:"+";font-size:103px;height:25px;line-height:0;left:0;top:0;text-indent:-17px;transform-origin:50% 50%;-o-transform-origin:50% 50%;-ms-transform-origin:50% 50%;-webkit-transform-origin:50% 50%;-moz-transform-origin:50% 50%;width:25px;}
.shttr-cube.shttr-c1::after{content:"";background:rgb(2,116,198);height:14px;width:14px;position:absolute;top:6px;left:6px;}
@keyframes cssload-spin{0%{transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{transform:scale(1) rotate(270deg) translateZ(0);}
}
@-o-keyframes cssload-spin{0%{-o-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-o-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-o-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-o-transform:scale(1) rotate(270deg) translateZ(0);}
}
@-ms-keyframes cssload-spin{0%{-ms-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-ms-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-ms-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-ms-transform:scale(1) rotate(270deg) translateZ(0);}
}
@-webkit-keyframes cssload-spin{0%{-webkit-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-webkit-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-webkit-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-webkit-transform:scale(1) rotate(270deg) translateZ(0);}
}
@-moz-keyframes cssload-spin{0%{-moz-transform:scale(1) rotate(0deg) translateZ(0);}
10%, 20%{-moz-transform:scale(1.4) rotate(90deg) translateZ(0);}
30%, 45%{-moz-transform:scale(1.4) rotate(180deg) translateZ(0);}
55%, 100%{-moz-transform:scale(1) rotate(270deg) translateZ(0);}
}

/*instagram feed*/
.insta-pic .insta-thumb{display:table;width:100%;height:250px;background-size:cover !important;background-position:center center !important;}
.insta-pic .insta-thumb:after{content:"";position:absolute;background:#000;top:0px;left:0px;height:100%;width:100%;display:table;opacity:0;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.insta-pic:hover .insta-thumb:after{opacity:0.5;}
.insta-pic{padding:0px !important;position:relative;}
.insta-pic .insta-likes{position:absolute;top:50%;left:50%;-moz-transform:translate(-50%, -50%);-ms-transform:translate(-50%, -50%);-webkit-transform:translate(-50%, -50%);-o-transform:translate(-50%, -50%);}
.insta-pic i{font-size:90px;position:relative;color:$(body.text.color);filter:blur(10px);opacity:0;transition: all .6s ease;-moz-transition: all .6s ease;-o-transition: all .6s ease;-webkit-transition: all .6s ease;-ms-transition: all .6s ease;opacity:0}
.insta-pic i span{position:absolute;top:50%;left:50%;-moz-transform:translate(-50%, -50%);-ms-transform:translate(-50%, -50%);-webkit-transform:translate(-50%, -50%);-o-transform:translate(-50%, -50%);font-size:20px;color:$(body.background);font-family:"consolas";font-weight:700;}
.insta-pic:hover i{opacity:0.5;filter:blur(0px);}
#instafeed{margin-top:30px;}
#instafeed .button-follow{position: absolute;top: 50%;left: 50%;-moz-transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);-webkit-transform: translate(-50%, -50%);-o-transform: translate(-50%, -50%);z-index: 5;}
#instafeed .button-follow a{color: $(body.background);padding: 10px 15px;display: block;background: $(body.text.color);font-weight: 700;text-transform: uppercase;font-size:15px;}
#instafeed .button-follow a:hover{color: $(body.text.color);background:$(body.link.color);text-decoration:none;}
#instafeed .button-follow a:link{text-decoration:none}
#instafeed .button-follow a i{font-size:18px;margin-bottom: -5px;display: inline-block;}

/* Subscribe Widget */
.FollowByEmail h2.title{margin-bottom:0px !important;}
.FollowByEmail td{clear: left;display: block;width: 100% !important;}
.FollowByEmail form{margin: 0px !important;box-sizing: border-box;}
.FollowByEmail table td:nth-child(1):before{content: "Enter your email address below to subscribe to our newsletter";box-sizing: border-box;font-weight: 300;color:$(body.text.color);font-size:14px;}
.FollowByEmail table,.FollowByEmail form{box-sizing: border-box;padding: 10px 0px!important;margin-bottom: 0px}
.FollowByEmail table td:nth-child(1) input:nth-child(1){margin-top:10px;margin-bottom: 0px;width: 100% !important}
.FollowByEmail table td:nth-child(2) input:nth-child(1){margin-top:0px;margin-bottom: 0px;width: 100% !important}
.FollowByEmail table td:nth-child(2) input:nth-child(1):hover{background: $(body.text.color);color: #000}
.FollowByEmail table .follow-by-email-address{height:40px !important;padding:10px 20px;line-height: 30px;font-size:15px !important;font-family:'Raleway', sans-serif;font-weight:400;border:1px solid rgba(255,255,255,0.6) !important;color: $(body.background);background: rgba(0,0,0,0);color:$(body.text.color);)}
.FollowByEmail table .follow-by-email-submit{margin: 0px !important;padding: 0px !important;border-radius: 0px !important;margin-top:10px !important;background: $(body.text.color) !important;color:$(body.background) !important;font-weight: 700;font-family:'Raleway', sans-serif !important;font-weight:500 !important;;height: 40px !important;font-size:15px !important; text-transform: uppercase;border:1px solid $(body.text.color) !important;}
.FollowByEmail table .follow-by-email-submit:hover{color:$(body.background) !important;}

/* Popular Posts */
.PopularPosts ul{list-style-type: none;padding: 0px;}
.PopularPosts ul li .item-thumbnail{position: relative;overflow: hidden;}
.PopularPosts ul li.item-thumbnail img{transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.PopularPosts ul li:hover .item-thumbnail img{transform: scale(1.1,1.1);transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.PopularPosts ul li .item-snippet{font-size: 12px;color: rgba(255,255,255,0.6);font-family: 'Raleway',arial,sans-serif;margin-top: 0px;}
.PopularPosts ul li .item-title a{font-weight: 700;font-size:14px;}

/* Labels */
.Label ul{list-style-type: none;padding: 0px;}
.Label li{float: left;}
.Label li a{padding: 5px 8px;border: 1px solid #ccc;display: table;margin:0px 3px;font-size:13px;color:$(body.text.color);line-height: 18px;display: inline-block;text-transform: uppercase;opacity: 0.6;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.fwrapper .Label li a{padding: 5px 8px !important;display: block !important;color: rgba(255,255,255,1);border-color:rgba(255,255,255,0.1)}
.Label li a:hover{color: $(body.text.color);border-color: rgba(255,255,255,1);text-decoration: none;opacity:1}

/* Blog Archive */
.BlogArchive select{color:$(body.text.color);background:transparent;width:100%;border:1px solid rgba(255,255,255,0.3);box-sizing:border-box;padding:10px 20px;}
.BlogArchive select option{color:$(body.background);}

/* Page layout */
.grid-item.inline-ad .ad-content{display: block !important;overflow: hidden !important;width: 100% !important;}

/* Footer */
footer .tfoot{background: $(body.link.color);}
footer a:hover{color: $(body.text.color);text-decoration: underline;}
footer .widget > h2:after{background: rgba(255,255,255,0.3)}
#credit-blsm {background: $(body.link.color);border-top: 1px solid rgba(255,255,255,0.1);box-sizing: border-box;padding: 15px 0px;font-size:14px;}
footer .shutter-columns-4 div.columns-cell {width: 25%;float: left;box-sizing: border-box}
footer .shutter-columns-3 div.columns-cell {width: 33.33%;float: left;box-sizing: border-box}
footer .shutter-columns-2 div.columns-cell {width: 50%;float: left;box-sizing: border-box}
footer .shutter-columns-1 div.columns-cell {width: 100%;box-sizing: border-box}
.tfoot{padding-bottom:20px;}

/*Post Header*/
#shutter_post_header {position: relative;margin-bottom: 30px;}
#shutter_post_header .shutter_wrap{background-size: cover !important;background-position: center center !important;padding:0px !important;}
#shutter_post_header .shutter_wrap:after{content: "";position: absolute;left: 0px;right:0px;top:0px;width:100%;height: 100%;background:#000;opacity:0;display: flex;flex-wrap: wrap}
#shutter_post_header .shutter_meta{position: absolute;top: 50%;left: 50%;-moz-transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);-webkit-transform: translate(-50%, -50%);-o-transform: translate(-50%, -50%);transform: translate(-50%, -50%);z-index: 5;max-width: 700px;  width: 100%;  text-align: center;}
#shutter_post_header .shutter_meta h1{font-size:40px;}
#shutter_post_header .post-tags a{text-transform: uppercase; border:1px solid rgba(255,255,255,0.8);opacity:0.8;padding:6px 4px;display: inline-block;margin:4px 4px;transition: .2s all ease-in-out;border-radius: 0px;}
#shutter_post_header .post-tags a:hover{opacity: 1;border-color: rgba(255,255,255,1);}
#shutter_post_header .post-details{opacity: 0.8;}
#shutter_post_header .post-title{padding:7px 0px;}
#shutter_post_header .meta-box{box-sizing: border-box;padding: 30px;background: rgba(0,0,0,0.4)}

/*Post Footer*/
.shutter-left-tags{float: left};
.shutter-right-share{float: right;text-align: right;}
.post-footer{padding:10px 0px;}
.shutter-right-share ul li{float: right;}
.shutter-right-share ul li a {display: inline-block;color: $(body.text.color);text-align: center;font-size: 12px;}
.shutter-right-share .share-links .social-item {padding: 4px 10px;box-shadow: 0 1px 1px rgba(0, 0, 0, 0.1);cursor: pointer;margin-left: 5px;text-align: center;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.shutter-right-share .share-links .social-item.facebook {background: #3b5998;}
.shutter-right-share .share-links .social-item.twitter {background: #00aced;}
.shutter-right-share .share-links .social-item.google {background: #dd4b39;}
.shutter-left-tags{font-weight: 500;font-family: 'Open Sans', sans-serif;}
.shutter-left-tags a{text-decoration: none;font-weight: 100;font-family: 'Open Sans', sans-serif;border:1px solid rgba(255,255,255,0.6);opacity:0.8;padding:2px 4px;margin:4px 3px;text-transform: uppercase;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.shutter-left-tags a:hover{opacity: 1;border-collapse: rgba(255,255,255,1);color:$(body.text.color)}

/* Comments */
#comments .comment .comment-block{border:0px;padding-bottom:15px;position:relative;}
.comments .comments-content .comment-content{font-size: 14px;background: rgba(255,255,255,0.1);color: $(body.text.color);line-height: 24px;width: 100%;  display: border-box;  padding: 20px;}
.comments .comment-actions{position: absolute;width: auto;right: 0px;top:-10px;}
.comments .comment-actions a{background: #transparent !important;color:$(body.text.color) !important;border: 1px solid #eaeaf1 !important;transition: .2s all ease-in-out !important;opacity:0.5;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.comments .comment-actions a:hover{background: #transparent !important;color: $(body.text.color) !important;border-color: $(body.text.color) !important;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;text-decoration:none !important;opacity:1}
.comments .comments-content .comment-header{border-bottom: 0px !important;}
.comments h4{border-bottom: 1px solid rgba(255,255,255,0.4);text-align: left;color: $(body.text.color);font-weight: 500;font-size: 18px;}
.comments h4:after{display: none;}
.comments .comment-actions a{margin:5px;display: inline-block;font-size:12px;padding:4px 8px;}
.comments .user a{font-weight: 700;font-size:15px;}
.comments .datetime a{color: #c3c3c3;font-size:11px;clear: left;display:block;margin-top:-10px;}
.comments .icon.user.blog-author:before{content:"\f3fe";font-family: "Ionicons";color:$(body.link.color);font-size:17px;}
.comments .continue a{width: 100% !important;text-align: center;border:1px solid #ccc;color:$(body.text.color);font-weight: 300;opacity:0.7;}
.comments .continue a:hover{color:$(body.text.color);border-color:$(body.text.color);opacity:1;}
.comments h4{border-bottom: 0;font-size: 18px;font-weight: 700;margin-bottom: 30px;margin-top: 2px;text-transform: uppercase;border-bottom: 2px solid #ecede7;padding-bottom: 10px;margin-bottom: 10px;position: relative;}
.comments h4:after{content: "";position: absolute;left: 0px;bottom: -2px;background: $(body.link.color);width: 100%;display: table;height: 2px;}
h4#comment-post-message{text-align:center;border:1px solid rgba(255,255,255,0.5);padding:18px 0px;box-sizing:border-box;color:$(body.text.color);font-size:16px;display:table;width:100%;}
h4#comment-post-message:after{display: none}

/*Post Author*/
.shutter-author{box-sizing: border-box;padding: 10px 10px;border:1px solid $(body.link.color);margin:20px 0px;background:$(body.link.color)}
.shutter-author .box-author .post-author{display: table;width:100%;}
.shutter-author .author-img{padding-right: 20px;display: table;float: left}
.shutter-author .author-content{padding-left: 130px;vertical-align: top;}
.top-author a{font-size:16px;line-height: 18px;font-weight: 600;}
#shutter-author-post-desc-place{color: $(body.text.color);opacity:0.7;font-size:12px;letter-spacing: 0.5px;line-height: 1.6;}
.shutter-author #shttr-link-place ul{padding: 0px;}
.shutter-author #shttr-link-place ul li{float: left;padding: 0px 3px;list-style-type: none;}
.breadcrumbs{width: 100%;overflow: hidden;}
.shutter-author .content-social-author a i{width: 25px;height: 25px;line-height: 25px;text-align: center;}
.shutter-author .content-social-author a:hover{color: $(body.text.color);}
.shutter-author .fa-facebook{background:#3b5999}
.shutter-author .fa-twitter{background: #55acee}
.shutter-author .fa-linkedin{background:#0077B5}
.shutter-author .fa-skype{background: #00AFF0}
.shutter-author .fa-dropbox{background: #007ee5}
.shutter-author .fa-wordpress{background: #21759b}
.shutter-author .fa-vimeo, .shutter-author .fa-vimeo-square{background: #1ab7ea}
.shutter-author .fa-slideshare{background: #0077b5}
.shutter-author .fa-vk{background:#4c75a3}
.shutter-author .fa-tumblr, .shutter-author .fa-tumblr-square{background: #34465d}
.shutter-author .fa-yahoo{background: #410093}
.shutter-author .fa-google-plus,.shutter-author .fa-google-plus-square,.shutter-author .fa-google-plus-official{background: #dd4b39}
.shutter-author .fa-pinterest-p,.shutter-author .fa-pinterest-square, .shutter-author .fa-pinterest{background: #bd081c}
.shutter-author .fa-youtube, .shutter-author .fa-youtube-play, .shutter-author .fa-youtube-square{background: #cd201f}
.shutter-author .fa-stumbleupon, .shutter-author .fa-stumbleupon-circle{background:#eb4924}
.shutter-author .fa-reddit-alien, .shutter-author .fa-reddit-square, .shutter-author .fa-reddit{background: #ff5700}
.shutter-author .fa-quora{background:#b92b27}
.shutter-author .fa-yelp{background: #af0606}
.shutter-author .fa-weibo{background:#df2029}
.shutter-author .fa-product-hunt{background: #da552f}
.shutter-author .fa-hacker-news{background: #ff6600}
.shutter-author .fa-soundcloud{background: #ff3300}
.shutter-author .fa-rss, .shutter-author .fa-rss-square{background: #f57d00}
.shutter-author .fa-whatsapp{background:#25D366}
.shutter-author .fa-weixin{background: #09b83e}
.shutter-author .fa-medium{background: #02b875}
.shutter-author .fa-vine{background: #00b489}
.shutter-author .fa-slack{background: #3aaf85}
.shutter-author .fa-instagram{background: #e4405f}
.shutter-author .fa-dribbble{background: #ea4c89}
.shutter-author .fa-flickr{background: #ff0084}
.shutter-author .fa-foursquare{background: #f94877}
.shutter-author .fa-behance-square, .shutter-author .fa-behance{background: #131418}
.shutter-author .fa-snapchat, .shutter-author .fa-snapchat-square, .shutter-author .fa-snapchat-ghost{background:$(body.text.color)C00}
.shutter-author .fa-codepen{background: $(body.background)}
.shutter-author .fa-stack-overflow{background: #f57d00}
.shutter-author .fa-digg{background:#131418}
.shutter-author .fa-delicious{background:#0084ff}

/*advertisement */
.btm-advertisement, #place-advert.bottom-advert, .top-advertisement {text-align: center;display: table;max-width: 100%;width: 100%; position: relative;overflow: hidden}

/* Error Page */
.error_msg{position: fixed;left: 320px;top:0px;right: 0px;bottom: 0px;z-index: 15;}
.error_msg .error-content{text-align: center;position: absolute;top:50%;left:50%;-moz-transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);-webkit-transform: translate(-50%, -50%);-o-transform: translate(-50%, -50%);transform: translate(-50%, -50%);
background:rgba(0,0,0,0.6);box-sizing:border-box;padding:30px;width:100%;max-width:550px;}
.error_msg .error-content h1{font-size:60px;margin-bottom:20px;font-weight:700;}
.error_msg .error-content h2{font-size: 30px;font-weight:700;}
.error_msg .error-content a.gohome{display: inline-block;margin: 10px;padding: 5px 10px;box-sizing: border-box;border:1px solid $(body.text.color);font-size:15px;text-transform: uppercase;transition:.2s all ease-in-out;-moz-transition:.2s all ease-in-out;-o-transition:.2s all ease-in-out;-ms-transition:.2s all ease-in-out;-webkit-transition:.2s all ease-in-out;}
.error_msg .error-content a:hover{background: $(body.text.color);color: $(body.background)}

/*meida queries*/
@media only screen and (max-width:1700px){
.shutter-one-sidebar .grid-item{width: 50%;}
.insta-pic .insta-thumb{height: 220px;}
.insta-pic i{font-size:60px;}
.insta-pic i span{font-size:16px;}
}
@media only screen and (max-width: 1500px){
.insta-pic .insta-thumb{height: 180px;}
.insta-pic i{font-size:60px;}
.insta-pic i span{font-size:16px;}
}
@media only screen and (max-width:1400px){
.shutter-two-sidebar .grid-item{width: 100%;padding:5px;}
.slide .slide-box{max-width:60%}
}
@media only screen and (max-width:1200px){
#navmenu{display: none}
#nav-responsive{display: block;}
.nav-sidebar-area{transform:translateX(-280px);max-width: 280px;}
.content-area{padding-left: 0px;}
.slide .slide-box{max-width:60%}
.slide-category a {padding: 2px 3px;margin-bottom: 5px;font-size:12px;}
.slide h3{font-size:25px;}
.slide .slidebox-inner{padding: 15px 18px;}
body{font-size:12px;}
.shutter-one-sidebar .grid-item{width: 50%;padding:5px;}
.insta-pic .insta-thumb{height: 180px;}
.insta-pic i{font-size:60px;}
.insta-pic i span{font-size:16px;}
.topmenu.hidden{display: block !important;border-bottom: 1px solid rgba(255,255,255,0.2)}
.topmenu{text-align: center;}
.topmenu.hidden h1, .topmenu .titlewrapper, .topmenu #header-inner, .topmenu #headercopy{display: inline-block;}
.topmenu .Header{margin: 0px;padding: 0px;display: inline;}
.topmenu > div.toogle_menu_button{position: absolute;left: 0px;top:0;cursor: pointer}
.topmenu > .toogle_search_button{position: absolute;right: 0px;top:0;cursor: pointer}
.topmenu h1:after{display: none;}
.topmenu.hidden h1{line-height:50px;}
.topmenu{position: fixed;top:0px;left: 0px;display: table;width: 100%;height: 50px;z-index: 999;background: $(body.background);}
.topmenu > div > a{line-height: 50px;width: 50px;text-align: center;display: table;font-size:20px;z-index:9099;}
.topmenu > div.toogle_menu_button a{border-right: 1px solid rgba(255,255,255,0.2);cursor: pointer}
.topmenu > div.toogle_search_button a{border-left: 1px solid rgba(255,255,255,0.2);cursor: pointer}
.topmenu > div > a:hover{color: $(body.text.color)}
.shutter-no-sidebar .grid-item{width: 33.33%;padding:5px;}
.error_msg{left:0px}
.error_msg .error-content{max-width: 400px;}
.content-area{margin-top:50px};
}
@media only screen and (max-width:1000px){
.insta-pic .insta-thumb{height: 160px;}
.insta-pic i{font-size:60px;}
.insta-pic i span{font-size:16px;}
}
@media only screen and (max-width: 991px){
.shutter-two-sidebar .grid-item{width: 33.33%;padding:5px;}
body.shutter-two-sidebar .addpad .col-lg-3{margin-top:30px}
}
@media only screen and (max-width: 900px){
.insta-pic .insta-thumb{height: 150px;}
.insta-pic i{font-size:60px;}
.insta-pic i span{font-size:16px}
aside .section{margin: 0px !important;}
#right-sidebar-area{padding-left: 0px;}
}
@media only screen and (max-width: 800px){
.col-sm-2.insta-pic{max-width: 33.33%;width:33.33% !important;min-width:33.33% !important;}
.insta-pic .insta-thumb{height: 250px;}
.shutter-one-sidebar .grid-item{width: 100%;}
.slide .slide-meta{display: none !important}
.shutter-no-sidebar .grid-item{width: 50%}
.shutter-two-sidebar .grid-item{width: 50%;padding:5px;}
#shutter_post_header .shutter_meta h1{font-size:30px;}
#shutter_post_header .shutter_meta {max-width: 400px}
.Label li a{font-size:11px;padding:4px 5px;}
}
@media only screen and (max-width: 767px){
footer .shutter-columns-4 div.columns-cell {width: 100%;float: left;box-sizing: border-box}
footer .shutter-columns-3 div.columns-cell {width: 100%;float: left;box-sizing: border-box}
.shutter-one-sidebar .grid-item{width: 50%;padding: 5px;}
.owl-nav{display:none}
body.shutter-one-sidebar .addpad .col-md-4{margin-top:30px}
}
@media only screen and (max-width:600px){
.insta-pic .insta-thumb{height: 200px;}
.shutter-author .author-img{float: none;width: 100%;text-align: center;}
.shutter-author .author-content{padding-left: 0px; text-align: center;}
.shutter-author .content-social-author{display: block;text-align: center;width: 100%;}
.shutter-author .content-social-author ul{text-align: center;display: inline-block;}
.post-footer > div{float:none;display:table;width:100%;text-align:center;}
.post-footer .social-icons:after{content: "";clear: both;}
.post-footer .social.share-links .count-share ul{display:inline-block;} 
.shutter-left-tags a{display: inline-block;}
.post-footer .social-icons{padding: 0px}
}
@media only screen and (max-width: 550px){
.shutter-one-sidebar .grid-item, .shutter-two-sidebar .grid-item, .shutter-no-sidebar .grid-item{width: 100%;}
.slide .slide-box{max-width: 80%;width:100%;text-align: center;}
.slide-box{position: absolute;left: 50%;top:75%;-moz-transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);-webkit-transform: translate(-50%, -50%);-o-transform: translate(-50%, -50%);transform: translate(-50%, -50%);}
.slide-box h3{font-size:22px;}
.slide-box .slide-category a{font-size:10px;}
footer .shutter-columns-2 div.columns-cell{width: 100%;}
.insta-pic .insta-thumb{height: 180px;}
.error_msg .error-content{max-width: 280px;}
.search__form input.search__input{width: 90%;box-sizing: border-box;}
.search__form .search__info{margin: 0px;padding: 20px 20px;width:100%;box-sizing: border-box;}

}
@media only screen and (max-width:450px){
.insta-pic .insta-thumb{height: 150px;}
#right-sidebar-area {padding-left: 15px}
}
@media only screen and (max-width: 350px){
.insta-pic .insta-thumb{height: 120px;}
.insta-pic i{font-size: 50px}
.insta-pic i span{font-size:12px;}
}
@media only screen and (max-width: 300px){
.shutter-loading, .shutter-loadmore a{max-width: 90%; min-width: 60%; font-size: 18px;}
.insta-pic .insta-thumb{height: 100px;}
}
]]></b:skin>


    <b:template-skin>
      <b:variable default='960px' name='content.width' type='length' value='860px'/>
      <b:variable default='0' name='main.column.left.width' type='length' value='0px'/>
      <b:variable default='310px' name='main.column.right.width' type='length' value='260px'/>

      <![CDATA[
body#layout{min-width:$(content.width);width:1100px;max-width:1100px;}
body#layout .hidden{display:block !important;}
body#layout .content-outer,body#layout .content-fauxcolumn-outer,body#layout .region-inner{min-width:$(content.width);}
body#layout .main-inner .columns{padding-left:$(main.column.left.width);padding-right:$(main.column.right.width);}
body#layout .main-inner .fauxcolumn-center-outer{left:$(main.column.left.width);right:$(main.column.right.width);_width:expression(this.parentNode.offsetWidth -parseInt("$(main.column.left.width)") -parseInt("$(main.column.right.width)") + 'px');}
body#layout .nav-sidebar-area{position:relative !important;}
body#layout footer{position:relative;display:table;width:100%;}
body#layout .footer-inner{width:100%;display:table;max-width:100% !important;}
body#layout .shutter-columns-3 .columns-cell{float:left;width:30%;}
body#layout .shutter-columns-2 .columns-cell{float:left;width:48%;}
body#layout .shutter-columns-4 .columns-cell{float:left;width:22%;}
body#layout #content-area{width:40%;float:left;}
body#layout .nav-sbar-inner{position:relative !important;width:260px;float:left;}
body#layout #left-sidebar-area{float:left;}
body#layout #right-sidebar-area{float:left;}
body#layout .main-inner .fauxcolumn-left-outer{width:$(main.column.left.width);}
body#layout #left-sidebar-area{max-width:30%;}
body#layout #right-sidebar-area{max-width:30%;}
body#layout .main-inner .fauxcolumn-right-outer{width:$(main.column.right.width);}
body#layout .main-inner .column-left-outer{width:$(main.column.left.width);right:100%;margin-left:-$(main.column.left.width);}
body#layout .main-inner .column-right-outer{width:$(main.column.right.width);margin-right:-$(main.column.right.width);}
body#layout{min-width:0;}
body#layout .content-outer{min-width:0;width:800px;}
body#layout .footer-inner{width:100% !important;}
body#layout .region-inner{min-width:0;width:auto;}
body#layout aside{max-width:95%;}
body#layout div.add_widget{padding:8px;}
body#layout div.add_widget a{margin-left:32px;}
body#layout #content-area{margin-left:30%;}
body#layout #left-sidebar-area #column-left-outer{width:100%;}
body#layout .addpad{position:relative;}
body#layout #right-sidebar-area{width:30% !important;;}
body#layout .column-right-outer{width:100%;}
body#layout .column-left-outer{margin-left:0px !important;width:100%;}
body#layout #left-sidebar-area{width:30%;}
body#layout #left-sidebar-area{margin-left:-70%;}
body#layout #left-sidebar-area .shutter-columns-2 .columns-cell{width:50%;display:block;}
body#layout .column-left-inner aside > .section{display:inline-block;width:100%;}
body#layout #right-sidebar-area .shutter-columns-2 .columns-cell{width:50%;display:block;}
body#layout .column-right-inner aside > .section{display:inline-block;width:100%;}
body#layout .footer-inner{width:100% !important;}
body#layout .content-area{padding-left:265px;}
body#layout{margin-top:0px;padding-top:0px;}
body#layout .nav-sbar-inner{background:#5d4286;padding-top:160px;-webkit-box-shadow:0 5px 15px 0 rgba(196,113,245,1);box-shadow:0 5px 15px 0 rgba(196,113,245,1);}
body#layout .section{background:transparent !important;}
body#layout .nav-sbar-inner .section{border:0px solid #fff !important;}
body#layout{background:#fff !important;}
body#layout .nav-sbar-inner:before{content:url('https://4.bp.blogspot.com/-w_OcVSzp_cM/WgxYE78QWHI/AAAAAAAABBY/GmK-TwZj1bM7KPAIaCLj-l4Tr7WhJOxkgCLcBGAs/s1600/clg.png');position:absolute;left:20px;top:100px;width:230px;height:230px;display:table;}
body#layout .nav-sbar-inner .section > h4{color:#fff !important;margin-left:0px;width:100%;}
body#layout #instawidget h4:after{content:"You can obtain this details from the tool link provided in documentation.";color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc;display:table;width:100%;margin:0px 0px;padding:10px 10px;box-sizing:border-box;font-size:12px;font-weight:normal;letter-spacing:0.4px;}

]]>
    </b:template-skin>

    <!-- jQuery -->
    <script src='https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js' type='text/javascript'/>

    <!--Load Fonts-->
    <script>
      //<![CDATA[
      /* You can add more configuration options to webfontloader by previously defining the WebFontConfig with your options */
      if ( typeof WebFontConfig === "undefined" ) {
        WebFontConfig = new Object();
      }
      WebFontConfig['google'] = {families: ['Raleway:400,500,600,700&amp;subset=latin-ext']};

      (function() {
        var wf = document.createElement( 'script' );
        wf.src = 'https://ajax.googleapis.com/ajax/libs/webfont/1.5.3/webfont.js';
        wf.type = 'text/javascript';
        wf.async = 'true';
        var s = document.getElementsByTagName( 'script' )[0];
        s.parentNode.insertBefore( wf, s );
      })();
      //]]>
    </script>

    <!--Load Icons-->
    <script async='async' type='text/javascript'>
      //<![CDATA[
      function loadCSS(e,o,n){"use strict";var s=window.document.createElement("link"),t=o||window.document.getElementsByTagName("script")[0];s.rel="stylesheet",s.href=e,s.media="only x",t.parentNode.insertBefore(s,t),setTimeout(function(){s.media=n||"all"})}loadCSS("//maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"),loadCSS("//code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css");
      //]]>
    </script>

    <b:if cond='data:blog.pageType in {&quot;index&quot;,&quot;archive&quot;}'>
      <script type='text/javascript'>
        //<![CDATA[
       function post(a,i){i=i.toLowerCase();var e=$(a),t=(e.find(".snippet").text(),e.find(".title").text()),s=e.find(".time").text(),n=e.find(".image").text(),d=e.find(".postauthor").text(),r=(e.find(".authorimg").text(),e.find(".purl").text()),p=(e.find(".comment").text(),["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sept","Oct","Nov","Dec"]);switch(s=(s=s.split("T"))[0].split("-"),s=p[Number(s[1])-1]+" "+s[2]+", "+s[0],i){case"default":o='<div class="cover"></div><a class="linkmask" href="'+r+'"></a><img src="'+n+'"/><div class="item-content"><h3><a href="'+r+'">'+t+"</a></h3><span>"+d+" / "+s+"</span></div>";$(a).html(o),$(a).addClass("dlayout"),$(a).removeClass("hidden");break;case"grid-appending":var o='<div class="cover noapply"></div><a class="linkmask" href="'+r+'"></a><img src="'+n+'"/><div class="item-content"><h3><a href="'+r+'">'+t+"</a></h3><span>"+d+" / "+s+"</span></div>";$(a).html(o),$(a).addClass("dlayout");var l=$(a).parent(".grid-item"),h=$('<div class="grid-item noapply">'+l.html()+"</div>");$(a).parent(".grid-item").remove(),$(".grid-wrapper").append(function(){$(this);$(this).append(h),$(this).find(a).removeClass("hidden"),$(this).find(a).find(".cover.noapply").removeClass("noapply");var i=$(this).find(a).parent(".grid-item");i.imagesLoaded(function(){$(".grid-wrapper").packery("appended",h);var a=$(window).scrollTop();a+=$(window).height()/2;var e=i.offset().top-$(window).height()/2;i.height();a>=e&&!i.hasClass("run-anim")&&(i.hasClass("anim-done")||i.addClass("run-anim"))})})}}var $=jQuery;
        //]]>
      </script>
    </b:if>
    <b:include data='blog' name='google-analytics'/>
  </head>

  <body>

    <script>postlayout = &#39;default&#39;</script>
    <div class='wrapper' id='tilting'>
      <div class='topmenu hidden'>
        <div class='toogle_menu_button'><a class='linktoggle_menu' href='javascript:;'><i class='ion-navicon-round'/></a></div>
        <div class='placeheader' id='headercopy'/>
        <div class='toogle_search_button'><a class='toggle_search-button' href='javascript:;'><i class='ion-ios-search'/></a></div>
      </div>

      <div class='nav-sidebar-area'>
        <div class='nav-sbar-inner'>
          <div class='nav-outer-table'>
            <div class='nav-inner-cell'>
              <a class='search-button' href='javascript:;'><i class='ion-ios-search'/></a>
              <a class='toggle-button hidden' href='javascript:;'><i class='ion-close-round'/></a>
              <div class='logo-section'>
                <b:section class='Header' id='Header' maxwidgets='1' name='Header' preferred='no' showaddelement='no'>
                  <b:widget id='Header1' locked='true' title='Shutter (Header)' type='Header' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='displayUrl'/>
                      <b:widget-setting name='displayHeight'>0</b:widget-setting>
                      <b:widget-setting name='sectionWidth'>292</b:widget-setting>
                      <b:widget-setting name='useImage'>false</b:widget-setting>
                      <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                      <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
                      <b:widget-setting name='displayWidth'>0</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:useImage'>
                        <b:if cond='data:imagePlacement == &quot;BEHIND&quot;'>
                          <!--
Show image as background to text. You can't really calculate the width
reliably in JS because margins are not taken into account by any of
clientWidth, offsetWidth or scrollWidth, so we don't force a minimum
width if the user is using shrink to fit.
This results in a margin-width's worth of pixels being cropped. If the
user is not using shrink to fit then we expand the header.
-->
                          <b:if cond='data:mobile'>
                            <div id='header-inner'>
                              <div class='titlewrapper' style='background: transparent'>
                                <h1 class='title' style='background: transparent; border-width: 0px'>
                                  <b:include name='title'/>
                                </h1>
                              </div>
                              <b:include name='description'/>
                            </div>
                            <b:else/>
                            <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                      + &quot;background-position: &quot;                      + data:backgroundPositionStyleStr + &quot;; &quot;                      + data:widthStyleStr                      + &quot;min-height: &quot; + data:height                      + &quot;_height: &quot; + data:height                      + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
                              <div class='titlewrapper' style='background: transparent'>
                                <h1 class='title' style='background: transparent; border-width: 0px'>
                                  <b:include name='title'/>
                                </h1>
                              </div>
                              <b:include name='description'/>
                            </div>
                          </b:if>
                          <b:else/>
                          <!--Show the image only-->
                          <div id='header-inner'>
                            <a expr:href='data:blog.homepageUrl' style='display: block'>
                              <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' expr:width='data:width' style='display: block'/>
                            </a>
                            <!--Show the description-->
                            <b:if cond='data:imagePlacement == &quot;BEFORE_DESCRIPTION&quot;'>
                              <b:include name='description'/>
                            </b:if>
                          </div>
                        </b:if>
                        <b:else/>
                        <!--No header image -->
                        <div id='header-inner'>
                          <div class='titlewrapper'>
                            <h1 class='title'>
                              <b:include name='title'/>
                            </h1>
                          </div>
                          <b:include name='description'/>
                        </div>
                      </b:if>
                    </b:includable>
                    <b:includable id='description'>
                      <div class='descriptionwrapper'>
                        <p class='description'><span><data:description/></span></p>
                      </div>
                    </b:includable>
                    <b:includable id='title'>
                      <b:tag cond='data:blog.url != data:blog.homepageUrl' expr:href='data:blog.homepageUrl' name='a'>
                        <data:title/>
                      </b:tag>
                    </b:includable>
                  </b:widget>
                </b:section>
              </div>
              <div class='nav-links'>
                <b:section class='nlink' id='nlink' maxwidgets='1' name='Navigation Menu' preferred='no' showaddelement='no'>
                  <b:widget id='LinkList999' locked='false' title='Navigation Menu' type='LinkList' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='text-9'>About</b:widget-setting>
                      <b:widget-setting name='link-9'>javascript:;</b:widget-setting>
                      <b:widget-setting name='text-8'>Documentation</b:widget-setting>
                      <b:widget-setting name='link-7'>/404</b:widget-setting>
                      <b:widget-setting name='link-8'>/p/documentation.html</b:widget-setting>
                      <b:widget-setting name='link-5'>javascript:;</b:widget-setting>
                      <b:widget-setting name='link-6'>[mega menu]</b:widget-setting>
                      <b:widget-setting name='link-3'>javascript:;</b:widget-setting>
                      <b:widget-setting name='link-4'>javascript:;</b:widget-setting>
                      <b:widget-setting name='text-1'>Sub Menu</b:widget-setting>
                      <b:widget-setting name='text-0'>Home</b:widget-setting>
                      <b:widget-setting name='text-3'>_Sub Item</b:widget-setting>
                      <b:widget-setting name='text-2'>_Sub Item</b:widget-setting>
                      <b:widget-setting name='text-5'>__sub sub item</b:widget-setting>
                      <b:widget-setting name='text-4'>__sub sub item</b:widget-setting>
                      <b:widget-setting name='text-7'>404</b:widget-setting>
                      <b:widget-setting name='text-6'>Mega Menu</b:widget-setting>
                      <b:widget-setting name='sorting'>NONE</b:widget-setting>
                      <b:widget-setting name='link-1'>javascript:;</b:widget-setting>
                      <b:widget-setting name='link-2'>javascript:;</b:widget-setting>
                      <b:widget-setting name='link-0'>javascript:;</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>


                      <div class='widget-content' id='navmenu' itemscope='itemscope' itemtype='http://schema.org/SiteNavigationElement' role='navigation'>
                        <ul>
                          <b:loop values='data:links' var='link'>
                            <li itemprop='name'><a expr:href='data:link.target' itemprop='url'><data:link.name/></a></li>
                          </b:loop>
                        </ul>
                        <b:include name='quickedit'/>
                      </div>

                      <div class='responsive-nav' id='nav-responsive'>
                        <ul>
                          <b:loop values='data:links' var='link'>
                            <li><a expr:href='data:link.target'><data:link.name/></a></li>
                          </b:loop>
                        </ul>
                      </div>

                    </b:includable>
                  </b:widget>
                </b:section>
              </div>
              <div class='nav-social'>
                <b:section class='nsocial' id='nsocial' maxwidgets='1' name='Social Links' preferred='no' showaddelement='no'>
                  <b:widget id='LinkList998' locked='false' title='Social Links' type='LinkList' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='sorting'>NONE</b:widget-setting>
                      <b:widget-setting name='text-1'><![CDATA[<i class="fa fa-facebook"></i>]]></b:widget-setting>
                      <b:widget-setting name='link-1'>http://facebook.com</b:widget-setting>
                      <b:widget-setting name='text-0'><![CDATA[<i class="fa fa-twitter"></i>]]></b:widget-setting>
                      <b:widget-setting name='link-0'>#</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>


                      <div class='social-nav' id='nav-social'>
                        <ul>
                          <b:loop values='data:links' var='link'>
                            <li><a expr:href='data:link.target'><data:link.name/></a></li>
                          </b:loop>
                        </ul>
                      </div>

                    </b:includable>
                  </b:widget>
                </b:section>
              </div>
              <div class='hidden'>
                <b:section class='hidden' id='adminpanel_options' maxwidgets='2' name='Author Widget' preferred='no' showaddelement='no'>
                  <b:widget id='HTML998' locked='false' title='About Author Description' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'>Hey there, We are Blossom Themes! We are trying to provide you the new way to look and use the blogger templates. Our designers are working hard and pushing the boundaries of possibilities to widen the horizon of the regular templates and provide high quality blogger templates to all hardworking bloggers!</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>


                      <div id='shutter-post-auth-desc'><data:content/></div>



                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                  <b:widget id='LinkList997' locked='false' title='Author Social Links' type='LinkList' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='link-3'>http://plus.google.com</b:widget-setting>
                      <b:widget-setting name='sorting'>NONE</b:widget-setting>
                      <b:widget-setting name='text-1'><![CDATA[<i class="fa fa-facebook"></i>]]></b:widget-setting>
                      <b:widget-setting name='link-1'>http://twitter.com</b:widget-setting>
                      <b:widget-setting name='text-0'><![CDATA[<i class="fa fa-twitter"></i>]]></b:widget-setting>
                      <b:widget-setting name='link-2'>http://instagram.com</b:widget-setting>
                      <b:widget-setting name='text-3'><![CDATA[<i class="fa fa-instagram"></i>]]></b:widget-setting>
                      <b:widget-setting name='link-0'>http://facebook.com</b:widget-setting>
                      <b:widget-setting name='text-2'><![CDATA[<i class="fa fa-google-plus"></i>]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <div id='shutter-author-links'>
                        <ul>
                          <b:loop values='data:links' var='link'>
                            <li><a expr:href='data:link.target'><data:link.name/></a></li>
                          </b:loop>
                        </ul>
                        <b:include name='quickedit'/>
                      </div>
                    </b:includable>
                  </b:widget>
                </b:section>
                <b:section class='hidden' id='error_page_option' maxwidgets='2' name='Error Page' preferred='no' showaddelement='no'>
                  <b:widget id='HTML995' locked='false' title='Error Page Background Image Url' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'><![CDATA[https://images.pexels.com/photos/532891/pexels-photo-532891.jpeg?w=1260&h=750&auto=compress&cs=tinysrgb]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:content'>
                        &lt;style&gt;.error_img{background: url(&#39;<data:content/>&#39;);background-color:#0275c6;background-position: center center !important;background-size: cover !important;}&lt;/style&gt;
                        <b:else/>

                        &lt;style&gt;.error_img{background: url(https://2.bp.blogspot.com/-xnNSwJfTEBw/WgKrGKlbWXI/AAAAAAAAA6o/-tyIFSFJS68nDb3XROWm7pF4pJbSnqTVACLcBGAs/s1600/6361491333701607071204999803_photography.jpg);background-color:#0275c6;background-position: center center !important;background-size: cover !important;}&lt;/style&gt;

                      </b:if>


                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>
                <b:section class='hidden' id='Post-Animation' maxwidgets='1' name='Post Animation' preferred='no' showaddelement='no'>
                  <b:widget id='HTML994' locked='false' title='Animation Type for Post' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'>slideup</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:content'>
                        <script>loadinganimation = &quot;<data:content/>&quot;</script>
                        <b:else/>

                        <script>loadinganimation = &quot;expand&quot;</script>

                      </b:if>


                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>

                <b:section class='hidden' id='instawidget' maxwidgets='2' name='Instagram Widget' preferred='no' showaddelement='no'>
                  <b:widget id='HTML993' locked='false' title='USER ID' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'>4087962651</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:content'>
                        <script>insta_userid = &quot;<data:content/>&quot;</script>
                        <b:else/>

                        <script>insta_userid = &quot;shutter-no-id&quot;</script>

                      </b:if>


                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                  <b:widget id='HTML992' locked='false' title='Access Token' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'>4087962651.6506e59.3dee099f0e3745cab94be871b35ff7d3</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:content'>
                        <script>insta_token = &quot;<data:content/>&quot;</script>
                        <b:else/>

                        <script>insta_token = &quot;shutter-no-token&quot;</script>

                      </b:if>


                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>

                <b:section class='hidden' id='Pagenaveropt' maxwidgets='2' name='Page Navigation' preferred='no' showaddelement='no'>
                  <b:widget id='HTML991' locked='false' title='Ppost per page' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'>8</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:content'>
                        <script>perpage = &quot;<data:content/>&quot;</script>
                        <b:else/>

                        <script>perpage = &quot;7&quot;</script>

                      </b:if>


                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                  <b:widget id='HTML990' locked='false' title='Navigation Type' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'>infinite</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>

                      <b:if cond='data:content'>
                        <script>pagit = &quot;<data:content/>&quot;</script>
                        <b:else/>

                        <script>pagit = &quot;infinite&quot;</script>

                      </b:if>


                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>
              </div>
            </div><!--/cell-->
          </div><!--/table-->
        </div>
      </div>
      <div class='content-area'>
        <div class='container-fluid'>
          <div class='row fullheight'>
            <div class='hidden'>
              <b:section class='slider-widget' id='slider-widget' maxwidgets='1' preferred='no' title='Featured Slider'>
                <b:widget id='HTML999' locked='false' title='Main Slider' type='HTML' version='1'>
                  <b:widget-settings>
                    <b:widget-setting name='content'><![CDATA[<object class="shutter-slider" data-label="travel" data-slidenumber="5"></object>]]></b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
                    <b:if cond='data:blog.homepageUrl == data:blog.url'>
                      <b:if cond='data:content'>
                        <data:content/>

                        <script type='text/javascript'>
                          //<![CDATA[
                          $(document).ready(function(){$(".shutter-slider").map(function(){var e=$(this),t=e.attr("data-label"),s=e.attr("data-slidenumber"),i="";$.ajax({url:"/feeds/posts/default/-/"+t+"?alt=json-in-script&max-results="+s,type:"get",dataType:"jsonp",success:function(e){if(e.feed.entry){for(var t=0;t<e.feed.entry.length;t++){var s=e.feed.entry[t];if(s.media$thumbnail)-1!==(r=s.media$thumbnail.url).indexOf("/s72-c")&&(r=r.replace("/s72-c","/s1600")),-1!==r.indexOf("img.youtube.com")&&(r=r.replace("/default.jpg","/maxresdefault.jpg"));else var r="https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/s1600/notfound.png";for(var a=s.category[0].term,l='<a href="/search/label/'+a+"?&max-results="+perpage+'" title="Show all posts in '+a+'">'+a+"</a>",d=function(e,t){return e.replace(/<.*?>/gi,"").split(/\s+/).slice(0,t-1).join(" ")}(s.content.$t,25),o=s.title.$t,n=0;n<s.link.length;n++)if("alternate"==s.link[n].rel)var c=s.link[n].href;i=i+'<div class="slide"><div class="slide-wrapper" style="background:url(\''+r+'\')"><div class="slide-inner"><div class="slide-box"><div class="slidebox-inner"><div class="slide-category">'+l+'</div><div class="slide-title"><h3><a href="'+c+'">'+o+'</a></h3></div><div class="slide-meta"><span>'+d+" [..]</span></div>                        </div>                        </div>                        </div>                        </div>                        </div>"}$("#slider").html(i),$("#sldr").removeClass("hidden"),$("#slider .slide").map(function(){var e=$(window).height();$(this).css("height",e)}),$(window).resize(function(){$("#slider .slide").map(function(){var e=$(window).height();$(this).css("height",e)})}),$(".owl-carousel").owlCarousel({items:1,autoplay:!0,loop:!0,nav:!0,navText:["<div class='prev-slider-shutter'><i class='ion-android-arrow-back'></i></div>","<div class='next-slider-shutter'><i class='ion-android-arrow-forward'></i></div>"]}),$(window).mousemove(function(e){var t=$(".prev-slider-shutter").offset(),s=$(".prev-slider-shutter").outerWidth(),i=$(".prev-slider-shutter").outerHeight(),r=e.pageX,a=e.pageY;if(r>t.left&&r<t.left+s&&a>t.top&&a<t.top+i){var l=r-t.left,d=a-t.top;$(".ion-android-arrow-back").css("top",d).css("left",l)}}),$(window).mousemove(function(e){var t=$(".next-slider-shutter").offset(),s=$(".next-slider-shutter").outerWidth(),i=$(".next-slider-shutter").outerHeight(),r=e.pageX,a=e.pageY;if(r>t.left&&r<t.left+s-40&&a>t.top&&a<t.top+i){var l=r-t.left,d=a-t.top;$(".ion-android-arrow-forward").css("top",d).css("left",l)}})}}})})});
                          //]]>

                        </script>
                      </b:if>
                    </b:if>

                    <b:include name='quickedit'/>
                  </b:includable>
                </b:widget>
              </b:section>
            </div>
            <div class='col-sm-12 hidepad hidden' id='sldr'>
              <div class='slider-wrapper owl-carousel' id='slider'>
              </div>
            </div>
          </div> <!--// row slider //-->

          <b:if cond='data:blog.pageType in {&quot;error_page&quot;}'>
            <div class='error_msg error_img'>
              <div class='error-content'>
                <h1>404</h1>
                <h2>Page Not Found!</h2>
                <a class='gohome' expr:href='data:blog.homepageUrl'>Go to home</a>
              </div>
            </div>
            <style>html,body{overflow:hidden;}</style>
          </b:if>
          <b:if cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}'>
            <div class='proccessed_header hidden' id='shutter_post_header'/>
          </b:if>


          <div class='row addpad'>
            <div class='col-md-8' id='content-area'>
              <div class='column-center-outer'>
                <div class='column-center-inner'>

                  <div class='top-advertisement'>
                    <b:section class='top-advert-section' id='top-advert-widget' maxwidgets='1' preferred='no' title='Top Advertisement'>
                      <b:widget id='HTML997' locked='false' title='Top Advertisement' type='HTML' version='1'>
                        <b:widget-settings>
                          <b:widget-setting name='content'><![CDATA[<style type="text/css">.advertisement_banner_demo{display:block;width:100%;height:90px;border:1px solid rgba(255,255,255,0.5);background:rgba(255,255,255,0.4);overflow:hidden;}.advertisement_banner_demo:hover{color:#fff}.advertisement_banner_demo:after{content:"Advertisement Responsive";font-weight:700;font-family:"Raleway";position:absolute;left:50%;top:50%;-moz-transform:translate(-50%, -50%);-ms-transform:translate(-50%, -50%);-webkit-transform:translate(-50%, -50%);-o-transform:translate(-50%, -50%);transform:translate(-50%, -50%);font-size:20px;}</style><a href="javascript:;" class="advertisement_banner_demo"></a>]]></b:widget-setting>
                        </b:widget-settings>
                        <b:includable id='main'>
                          <data:content/>
                          <b:include name='quickedit'/>
                        </b:includable>
                      </b:widget>
                    </b:section>
                  </div>

                  <b:section class='main' id='main' name='Main' showaddelement='yes'>
                    <b:widget id='Blog1' locked='false' title='Blog Posts' type='Blog' version='1'>
                      <b:widget-settings>
                        <b:widget-setting name='showDateHeader'>true</b:widget-setting>
                        <b:widget-setting name='style.textcolor'>#222222</b:widget-setting>
                        <b:widget-setting name='showShareButtons'>true</b:widget-setting>
                        <b:widget-setting name='authorLabel'>By</b:widget-setting>
                        <b:widget-setting name='showCommentLink'>true</b:widget-setting>
                        <b:widget-setting name='style.urlcolor'>#666666</b:widget-setting>
                        <b:widget-setting name='showAuthor'>false</b:widget-setting>
                        <b:widget-setting name='style.linkcolor'>#cc6611</b:widget-setting>
                        <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
                        <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
                        <b:widget-setting name='showAuthorProfile'>false</b:widget-setting>
                        <b:widget-setting name='style.layout'>1x1</b:widget-setting>
                        <b:widget-setting name='showLabels'>true</b:widget-setting>
                        <b:widget-setting name='showLocation'>true</b:widget-setting>
                        <b:widget-setting name='showTimestamp'>true</b:widget-setting>
                        <b:widget-setting name='postsPerAd'>3</b:widget-setting>
                        <b:widget-setting name='showBacklinks'>false</b:widget-setting>
                        <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
                        <b:widget-setting name='showInlineAds'>true</b:widget-setting>
                        <b:widget-setting name='showReactions'>true</b:widget-setting>
                      </b:widget-settings>
                      <b:includable id='main' var='top'>
                        <b:if cond='!data:mobile'>
                          <!-- posts -->


                          <b:include data='top' name='status-message'/>

                          <b:if cond='data:blog.pageType in {&quot;index&quot;,&quot;archive&quot;}'>
                            &lt;div class=&#39;grid-wrapper&#39;&gt;
                            &lt;div class=&#39;grid-sizer&#39;&gt;&lt;/div&gt;

                          </b:if>
                          <b:loop values='data:posts' var='post'>

                            <b:if cond='data:blog.pageType in {&quot;index&quot;,&quot;archive&quot;}'>
                              &lt;div class=&#39;grid-item&#39; style=&#39;opacity:0;&#39;&gt;
                              <b:else/>
                              &lt;div class=&#39;page-item&#39;&gt;
                            </b:if>
                            <b:include data='post' name='post'/>
                            <b:if cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}'>
                              <div class='shutter-comment'>
                                <b:include data='post' name='comment_picker'/>
                              </div>
                            </b:if>
                            &lt;/div&gt;

                            <!-- Ad -->
                            <b:if cond='data:post.includeAd'>
                              <div class='grid-item inline-ad' style='opacity:1 !important'>
                                <b:if cond='data:adCode'>
                                  <div class='ad-content'>
                                    <data:adCode/>

                                  </div>
                                </b:if>
                              </div>
                            </b:if>

                          </b:loop>
                          <b:if cond='data:blog.pageType in {&quot;index&quot;,&quot;archive&quot;}'>

                            &lt;/div&gt;

                          </b:if>
                          <!-- navigation -->
                          <b:include name='nextprev'/>

                          <!-- feed links -->
                          <b:include name='feedLinks'/>

                          <b:else/>
                          <b:include name='mobile-main'/>
                        </b:if>

                        <b:include cond='data:top.showPlusOne' name='googlePlusBootstrap'/>
                      </b:includable>
                      <b:includable id='backlinkDeleteIcon' var='backlink'>
                        <span expr:class='&quot;item-control &quot; + data:backlink.adminClass'>
                          <a expr:href='data:backlink.deleteUrl' expr:title='data:top.deleteBacklinkMsg'>
                            <img src='https://resources.blogblog.com/img/icon_delete13.gif'/>
                          </a>
                        </span>
                      </b:includable>
                      <b:includable id='backlinks' var='post'>
                        <a name='links'/><h4><data:post.backlinksLabel/></h4>
                        <b:if cond='data:post.numBacklinks != 0'>
                          <dl class='comments-block' id='comments-block'>
                            <b:loop values='data:post.backlinks' var='backlink'>
                              <div class='collapsed-backlink backlink-control'>
                                <dt class='comment-title'>
                                  <span class='backlink-toggle-zippy'>&#160;</span>
                                  <a expr:href='data:backlink.url' rel='nofollow'><data:backlink.title/></a>
                                  <b:include data='backlink' name='backlinkDeleteIcon'/>
                                </dt>
                                <dd class='comment-body collapseable'>
                                  <data:backlink.snippet/>
                                </dd>
                                <dd class='comment-footer collapseable'>
                                  <span class='comment-author'><data:post.authorLabel/> <data:backlink.author/></span>
                                  <span class='comment-timestamp'><data:post.timestampLabel/> <data:backlink.timestamp/></span>
                                </dd>
                              </div>
                            </b:loop>
                          </dl>
                        </b:if>
                        <p class='comment-footer'>
                          <a class='comment-link' expr:href='data:post.createLinkUrl' expr:id='data:widget.instanceId + &quot;_backlinks-create-link&quot;' target='_blank'><data:post.createLinkLabel/></a>
                        </p>
                      </b:includable>
                      <b:includable id='comment-form' var='post'>
                        <div class='comment-form'>
                          <a name='comment-form'/>
                          <b:if cond='data:mobile'>
                            <h4 id='comment-post-message'>
                              <a expr:id='data:widget.instanceId + &quot;_comment-editor-toggle-link&quot;' href='javascript:void(0)'><data:postCommentMsg/></a></h4>
                            <p><data:blogCommentMessage/></p>
                            <data:blogTeamBlogMessage/>
                            <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                            <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
                            <b:else/>
                            <h4 id='comment-post-message'><data:postCommentMsg/></h4>
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
                          <span class='cmt_count_iframe_holder' expr:data-count='data:post.numComments' expr:data-onclick='data:post.addCommentOnclick' expr:data-post-url='data:post.url' expr:data-url='data:post.url.canonical.http'>
                          </span>
                          <b:else/>
                          <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
                            <data:post.commentLabelFull/>:
                          </a>
                        </b:if>
                      </b:includable>
                      <b:includable id='comment_picker' var='post'>
                        <b:if cond='data:post.commentSource == 1'>
                          <b:include data='post' name='iframe_comments'/>
                          <b:elseif cond='data:post.showThreadedComments'/>
                          <b:include data='post' name='threaded_comments'/>
                          <b:else/>
                          <b:include data='post' name='comments'/>
                        </b:if>
                      </b:includable>
                      <b:includable id='comments' var='post'>
                        <div class='comments' id='comments'>
                          <a name='comments'/>
                          <b:if cond='data:post.allowComments'>
                            <h4><data:post.commentLabelFull/>:</h4>

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
                              <b:include cond='data:post.allowComments and data:post.feedLinks' data='post.feedLinks' name='feedLinksBody'/>
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
                      <b:includable id='iframe_comments' var='post'>

                        <b:if cond='data:post.allowIframeComments'>
                          <script expr:src='data:post.iframeCommentSrc' type='text/javascript'/>
                          <div class='cmt_iframe_holder' expr:data-href='data:post.url.canonical' expr:data-viewtype='data:post.viewType'/>

                          <b:if cond='data:post.embedCommentForm == &quot;false&quot;'>
                            <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a>
                          </b:if>
                        </b:if>
                      </b:includable>
                      <b:includable id='mobile-index-post' var='post'>
                        <div class='mobile-date-outer date-outer'>
                          <b:if cond='data:post.dateHeader'>
                            <div class='date-header'>
                              <span><data:post.dateHeader/></span>
                            </div>
                          </b:if>

                          <div class='mobile-post-outer'>
                            <a expr:href='data:post.url'>
                              <h3 class='mobile-index-title entry-title' itemprop='name'>
                                <data:post.title/>
                              </h3>

                              <div class='mobile-index-arrow'>&amp;rsaquo;</div>

                              <div class='mobile-index-contents'>
                                <b:if cond='data:post.thumbnailUrl'>
                                  <div class='mobile-index-thumbnail'>
                                    <div class='Image'>
                                      <img expr:src='data:post.thumbnailUrl'/>
                                    </div>
                                  </div>
                                </b:if>

                                <div class='post-body'>
                                  <b:if cond='data:post.snippet'><data:post.snippet/></b:if>
                                </div>
                              </div>

                              <div style='clear: both;'/>
                            </a>

                            <div class='mobile-index-comment'>
                              <b:include cond='data:blog.pageType != &quot;static_page&quot;                          and data:post.allowComments                          and data:post.numComments != 0' data='post' name='comment_count_picker'/>
                            </div>
                          </div>
                        </div>
                      </b:includable>
                      <b:includable id='mobile-main' var='top'>
                        <!-- posts -->
                        <div class='blog-posts hfeed'>

                          <b:include data='top' name='status-message'/>

                          <b:if cond='data:blog.pageType == &quot;index&quot;'>
                            <b:loop values='data:posts' var='post'>
                              <b:include data='post' name='mobile-index-post'/>
                            </b:loop>
                            <b:else/>
                            <b:loop values='data:posts' var='post'>
                              <b:include data='post' name='mobile-post'/>
                            </b:loop>
                          </b:if>
                        </div>

                        <b:include name='mobile-nextprev'/>
                      </b:includable>
                      <b:includable id='mobile-nextprev'>
                        <div class='blog-pager' id='blog-pager'>
                          <b:if cond='data:newerPageUrl'>
                            <div class='mobile-link-button' id='blog-pager-newer-link'>
                              <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'>&amp;lsaquo;</a>
                            </div>
                          </b:if>

                          <b:if cond='data:olderPageUrl'>
                            <div class='mobile-link-button' id='blog-pager-older-link'>
                              <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'>&amp;rsaquo;</a>
                            </div>
                          </b:if>

                          <div class='mobile-link-button' id='blog-pager-home-link'>
                            <a class='home-link' expr:href='data:blog.homepageUrl'><data:homeMsg/></a>
                          </div>

                          <div class='mobile-desktop-link'>
                            <a class='home-link' expr:href='data:desktopLinkUrl'><data:desktopLinkMsg/></a>
                          </div>

                        </div>
                        <div class='clear'/>
                      </b:includable>
                      <b:includable id='mobile-post' var='post'>
                        <div class='date-outer'>
                          <b:if cond='data:post.dateHeader'>
                            <h2 class='date-header'><span><data:post.dateHeader/></span></h2>
                          </b:if>
                          <div class='date-posts'>
                            <div class='post-outer'>

                              <div class='post hentry uncustomized-post-template' itemscope='itemscope' itemtype='http://schema.org/BlogPosting'>
                                <b:if cond='data:post.thumbnailUrl'>
                                  <meta expr:content='data:post.thumbnailUrl' itemprop='image_url'/>
                                </b:if>
                                <meta expr:content='data:blog.blogId' itemprop='blogId'/>
                                <meta expr:content='data:post.id' itemprop='postId'/>

                                <a expr:name='data:post.id'/>
                                <b:if cond='data:post.title'>
                                  <h3 class='post-title entry-title' itemprop='name'>
                                    <b:if cond='data:post.link'>
                                      <a expr:href='data:post.link'><data:post.title/></a>
                                      <b:elseif cond='data:post.url and data:blog.url != data:post.url'/>
                                      <a expr:href='data:post.url'><data:post.title/></a>
                                      <b:else/>
                                      <data:post.title/>
                                    </b:if>
                                  </h3>
                                </b:if>

                                <div class='post-header'>
                                  <div class='post-header-line-1'/>
                                </div>

                                <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id' itemprop='articleBody'>
                                  <data:post.body/>
                                  <div style='clear: both;'/> <!-- clear for photos floats -->
                                </div>

                                <div class='post-footer'>
                                  <div class='post-footer-line post-footer-line-1'>
                                    <span class='post-author vcard'>
                                      <b:if cond='data:top.showAuthor'>
                                        <b:if cond='data:post.authorProfileUrl'>
                                          <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                                            <meta expr:content='data:post.authorProfileUrl' itemprop='url'/>
                                            <a expr:href='data:post.authorProfileUrl' rel='author' title='author profile'>
                                              <span itemprop='name'><data:post.author/></span>
                                            </a>
                                          </span>
                                          <b:else/>
                                          <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                                            <span itemprop='name'><data:post.author/></span>
                                          </span>
                                        </b:if>
                                      </b:if>
                                    </span>

                                    <span class='post-timestamp'>
                                      <b:if cond='data:top.showTimestamp'>
                                        <data:top.timestampLabel/>
                                        <b:if cond='data:post.url'>
                                          <meta expr:content='data:post.url.canonical' itemprop='url'/>
                                          <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'><abbr class='published' expr:title='data:post.timestampISO8601' itemprop='datePublished'><data:post.timestamp/></abbr></a>
                                        </b:if>
                                      </b:if>
                                    </span>

                                    <span class='post-comment-link'>
                                      <b:include cond='data:blog.pageType not in {&quot;item&quot;,&quot;static_page&quot;}                                  and data:post.allowComments' data='post' name='comment_count_picker'/>
                                    </span>
                                  </div>

                                  <div class='post-footer-line post-footer-line-2'>
                                    <b:if cond='data:top.showMobileShare'>
                                      <div class='mobile-link-button goog-inline-block' id='mobile-share-button'>
                                        <a href='javascript:void(0);'><data:shareMsg/></a>
                                      </div>
                                    </b:if>
                                    <b:if cond='data:top.showDummy'>
                                      <div class='goog-inline-block dummy-container'><data:post.dummyTag/></div>
                                    </b:if>
                                  </div>

                                </div>
                              </div>

                              <b:include cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}' data='post' name='comment_picker'/>
                            </div>
                          </div>
                        </div>
                      </b:includable>
                      <b:includable id='nextprev'>
                        <div class='shutter-pager arrow' id='shutter-pager'>
                          <b:if cond='data:newerPageUrl'>
                            <div id='shutter-new'>
                              <a class='shutter-newer-link' expr:href='data:newerPageUrl' expr:title='data:newerPageTitle'><i class='ion-arrow-left-c'/></a>
                            </div>
                          </b:if>

                          <b:if cond='data:olderPageUrl'>
                            <div id='shutter-old'>
                              <a class='shutter-older-link' expr:href='data:olderPageUrl' expr:title='data:olderPageTitle'><i class='ion-arrow-right-c'/></a>
                            </div>
                          </b:if>

                          <a class='shutter-home' expr:href='data:blog.homepageUrl'><i class='ion-home'/></a>

                          <div class='shttr-pager-clear'/>
                        </div>
                        <div class='clear'/>
                      </b:includable>
                      <b:includable id='post' var='post'>

                        <b:if cond='data:blog.pageType in {&quot;index&quot;,&quot;archive&quot;}'>
                          <article expr:class='&quot;post hidden ajax_pickup hentry post_&quot; + data:post.id' expr:data-class='&quot;post_&quot; + data:post.id'>
                            <div class='snippet entry-content' itemprop='articleBody'><data:post.snippet/></div>
                            <div class='title entry-title'><data:post.title/></div>
                            <div class='time published' expr:title='data:post.timestampISO8601'><data:post.timestampISO8601/></div>
                            <div class='image'><b:if cond='data:post.firstImageUrl'><data:post.firstImageUrl/><b:else/>https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/s1600/notfound.png</b:if></div>
                            <div class='postauthor'><data:post.author/></div>
                            <div class='authorimg'><data:post.authorPhoto.url/></div>
                            <div class='purl'><data:post.url/></div>
                            <div class='comment'><data:post.numComments/></div>
                            <div class='vcard'>
                              <a class='url fn' expr:href='data:post.authorProfileUrl'><data:post.author/></a>
                            </div>
                            &lt;script&gt; post(&#39;.post_<data:post.id/>&#39;,postlayout); &lt;/script&gt;
                          </article>
                          <b:else/>


                          <div class='hidden' id='hpick'>
                            <b:if cond='data:post.firstImageUrl'>
                              <div class='shutter_wrap row' expr:style='&quot;background:url(&quot; + data:post.firstImageUrl + &quot;)&quot;'/>
                              <b:else/>
                              <div class='shutter_wrap row' style='background:url(https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/s1600/notfound.png)'/>
                            </b:if>
                            <div class='shutter_meta'>
                              <div class='meta-box'>
                                <div class='meta-box-inner'>
                                  <div class='post-tags'><b:if cond='data:top.showPostLabels and data:post.labels'><b:loop values='data:post.labels' var='label'><a class='label shutter-max-limit' expr:href='data:label.url'><data:label.name/></a><b:if cond='not data:label.isLast'/></b:loop></b:if> </div>
                                  <div class='post-title'><h1><data:post.title/></h1></div>
                                  <div class='post-details'><data:post.author/> / <time expr:data-pub='data:post.timestampISO8601'/></div>
                                </div>
                              </div>
                            </div>
                          </div>
                          <script type='text/javascript'>
                            //<![CDATA[
                            var $=jQuery;$("#hpick .shutter_wrap").css("min-height",$(window).height()),$("#shutter_post_header").html($("#hpick").html()).removeClass("hidden"),$("#hpick").remove(),$(window).resize(function(){$("#shutter_post_header .shutter_wrap").css("min-height",$(window).height())}),$("time").map(function(){var e=$(this).attr("data-pub"),t=["","January","February","March","April","May","June","July","August","September","October","November","December"][(e=(e=e.split("T"))[0].split("-"))[1]]+" "+e[2]+", "+e[0];$(this).after(t),$(this).remove()});
                            //]]>
                          </script>


                          <div class='post-body'>
                            <data:post.body/>
                          </div>

                          <div class='post-footer'>
                            <div class='shutter-left-tags'>
                              <div class='tags-wrap'>
                                <b:if cond='data:top.showPostLabels and data:post.labels'>&lt;span class=&quot;tags&quot;&gt;
                                  <b:loop values='data:post.labels' var='label'>
                                    <a expr:href='data:label.url' expr:title='&quot;View all posts in &quot; + data:label.name' rel='tag'>
                                      <data:label.name/>
                                    </a>
                                    <b:if cond='data:label.isLast'>&lt;/span&gt;</b:if>
                                  </b:loop>
                                </b:if>
                              </div>
                            </div>
                            <div class='shutter-right-share'>
                              <div class='social share-links clearfix'>
                                <div class='count-share'>
                                  <ul class='social-icons list-unstyled list-inline'>
                                    <li class='social-item facebook'>
                                      <a class='post_share_facebook facebook' expr:href='&quot;http://www.facebook.com/sharer.php?u=&quot; + data:post.url' onclick='javascript:window.open(this.href,&apos;&apos;, &apos;menubar=no,toolbar=no,resizable=yes,scrollbars=yes,height=220,width=600&apos;);return false;' title='facebook'>
                                        <i class='fa fa-facebook'>
                                        </i> facebook
                                      </a>
                                    </li>
                                    <li class='social-item twitter'>
                                      <a class='product_share_twitter twitter' expr:href='&quot;https://twitter.com/share?url=&quot; + data:post.url' onclick='javascript:window.open(this.href,&apos;&apos;, &apos;menubar=no,toolbar=no,resizable=yes,scrollbars=yes,height=260,width=600&apos;);return false;' title='twitter'>
                                        <i class='fa fa-twitter'>
                                        </i> twitter
                                      </a>
                                    </li>
                                    <li class='social-item google'>
                                      <a class='googleplus' expr:href='&quot;https://plus.google.com/share?url=&quot; + data:post.url' onclick='javascript:window.open(this.href,&apos;&apos;, &apos;menubar=no,toolbar=no,resizable=yes,scrollbars=yes,height=600,width=600&apos;);return false;' title='google +'>
                                        <i class='fa fa-google-plus'>
                                        </i> google+
                                      </a>
                                    </li>
                                  </ul>
                                </div>
                              </div>
                            </div>
                          </div>



                          <div class='bottom-advert' id='place-advert'/>

                          <div class='shutter-author'>
                            <div class='box box-author'>
                              <div class='post-author'>
                                <div class='author-img'> 
                                  <img class='avatar avatar-100 photo' expr:alt='data:post.author' expr:src='data:post.authorPhoto.url' height='100' width='100'/>
                                </div>
                                <div class='author-content'>
                                  <div class='top-author'>
                                    <h5>
                                      <a expr:href='data:post.authorUrl' expr:title='&quot;Posts by &quot; + data:post.author' rel='author'><data:post.author/>
                                      </a>
                                    </h5>
                                  </div>
                                  <p><span id='shutter-author-post-desc-place'><script>
                                    /*<![CDATA[*/
                                    $(document).ready(function(){
                                      $('#shutter-author-post-desc-place').html($('#shutter-post-auth-desc').html());
                                    });/*]]>*/
                                    </script></span>
                                  </p>
                                  <div class='content-social-author' id='shttr-link-place'> 
                                    <script>/*<![CDATA[*/
                                      $(document).ready(function(){
                                        $('#shttr-link-place').html($('#shutter-author-links').html());
                                      });/*]]>*/</script>
                                  </div>
                                </div>
                              </div>
                            </div>
                          </div>
                        </b:if>
                      </b:includable>
                      <b:includable id='postQuickEdit' var='post'>
                        <b:if cond='data:post.editUrl'>
                          <span expr:class='&quot;item-control &quot; + data:post.adminClass'>
                            <a expr:href='data:post.editUrl' expr:title='data:top.editPostMsg'>
                              <img alt='' class='icon-action' height='18' src='https://resources.blogblog.com/img/icon18_edit_allbkg.gif' width='18'/>
                            </a>
                          </span>
                        </b:if>
                      </b:includable>
                      <b:includable id='shareButtons' var='post'>
                        <b:if cond='data:top.showEmailButton'><a class='goog-inline-block share-button sb-email' expr:href='data:post.sharePostUrl + &quot;&amp;target=email&quot;' expr:title='data:top.emailThisMsg' target='_blank'><span class='share-button-link-text'><data:top.emailThisMsg/></span></a></b:if><b:if cond='data:top.showBlogThisButton'><a class='goog-inline-block share-button sb-blog' expr:href='data:post.sharePostUrl + &quot;&amp;target=blog&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=270,width=475\&quot;); return false;&quot;' expr:title='data:top.blogThisMsg' target='_blank'><span class='share-button-link-text'><data:top.blogThisMsg/></span></a></b:if><b:if cond='data:top.showTwitterButton'><a class='goog-inline-block share-button sb-twitter' expr:href='data:post.sharePostUrl + &quot;&amp;target=twitter&quot;' expr:title='data:top.shareToTwitterMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToTwitterMsg/></span></a></b:if><b:if cond='data:top.showFacebookButton'><a class='goog-inline-block share-button sb-facebook' expr:href='data:post.sharePostUrl + &quot;&amp;target=facebook&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=430,width=640\&quot;); return false;&quot;' expr:title='data:top.shareToFacebookMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToFacebookMsg/></span></a></b:if><b:if cond='data:top.showPinterestButton'><a class='goog-inline-block share-button sb-pinterest' expr:href='data:post.sharePostUrl + &quot;&amp;target=pinterest&quot;' expr:title='data:top.shareToPinterestMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToPinterestMsg/></span></a></b:if><b:if cond='data:top.showPlusOne'><div class='goog-inline-block google-plus-share-container'><data:post.googlePlusShareTag/></div></b:if>
                      </b:includable>
                      <b:includable id='status-message'>
                        <b:if cond='data:navMessage'>
                          <div class='status-msg-wrap'>
                            <div class='status-msg-body'>
                              <data:navMessage/>
                            </div>
                            <div class='status-msg-border'>
                              <div class='status-msg-bg'>
                                <div class='status-msg-hidden'><data:navMessage/></div>
                              </div>
                            </div>
                          </div>
                          <div style='clear: both;'/>
                        </b:if>
                      </b:includable>
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
                          <h4><data:post.commentLabelFull/>:</h4>

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
                              <data:post.noNewCommentsText/>
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


                  <div class='btm-advertisement'>
                    <b:section class='btm-advert-section' id='btm-advert-widget' maxwidgets='1' preferred='no' title='Bottom Advertisement'>
                      <b:widget id='HTML996' locked='false' title='Bottom Advertisement' type='HTML' version='1'>
                        <b:widget-settings>
                          <b:widget-setting name='content'><![CDATA[<style type="text/css">.advertisement_banner_demo{display:block;width:100%;height:90px;border:1px solid rgba(255,255,255,0.5);background:rgba(255,255,255,0.4);overflow:hidden;}.advertisement_banner_demo:hover{color:#fff}.advertisement_banner_demo:after{content:"Advertisement Responsive";font-weight:700;font-family:"Raleway";position:absolute;left:50%;top:50%;-moz-transform:translate(-50%, -50%);-ms-transform:translate(-50%, -50%);-webkit-transform:translate(-50%, -50%);-o-transform:translate(-50%, -50%);transform:translate(-50%, -50%);font-size:20px;}</style><a href="javascript:;" class="advertisement_banner_demo"></a>]]></b:widget-setting>
                        </b:widget-settings>
                        <b:includable id='main'>

                          <div class='pickup-bottom-advert'>
                            <data:content/>
                          </div>
                          <b:if cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}'>
                            <script type='text/javascript'>
                              //<![CDATA[
                              $(document).ready(function(){ 
                                $('#place-advert').html($('.pickup-bottom-advert').html());
                                $('.pickup-bottom-advert').remove();
                              });
                              //]]>
                            </script>
                          </b:if>
                          <b:include name='quickedit'/>
                        </b:includable>
                      </b:widget>
                    </b:section>
                  </div>

                </div>
              </div>
            </div>
            <div class='col-md-4' id='left-sidebar-area'>
              <div class='column-left-outer'>
                <div class='column-left-inner'>
                  <aside>
                    <macro:include id='main-column-left-sections' name='sections'>
                      <macro:param default='0' name='num' value='0'/>
                      <macro:param default='sidebar-left' name='idPrefix'/>
                      <macro:param default='sidebar' name='class'/>
                      <macro:param default='true' name='includeBottom'/>
                    </macro:include>
                  </aside>
                </div>
              </div><!--/leftouter-->
            </div>
            <div class='col-md-4' id='right-sidebar-area'>
              <div class='column-right-outer'>
                <div class='column-right-inner'>
                  <aside>
                    <macro:include id='main-column-right-sections' name='sections'>
                      <macro:param default='2' name='num' value='1'/>
                      <macro:param default='sidebar-right' name='idPrefix'/>
                      <macro:param default='sidebar' name='class'/>
                      <macro:param default='true' name='includeBottom'/>
                    </macro:include>
                  </aside>
                </div>
              </div>
              <!--/rightouter-->
            </div> 
          </div><!--// row //-->

          <footer class='row'>
            <div class='col-sm-12'>
              <div class='row instawidget'>
                <div class='col-sm-12'>
                  <div class='row nopadsinsta' id='instafeed'/>
                  <script type='text/javascript'>
                    //<![CDATA[
                    $(document).ready(function(){"shutter-no-token"!=insta_token&&"shutter-no-id"!=insta_userid&&new Instafeed({get:"user",userId:insta_userid,limit:6,sortBy:"random",accessToken:insta_token,template:'<div class="col-sm-2 insta-pic" data-username="{{uname}}"><a href="{{link}}" target="_blank"><div class="insta-thumb" style="background:url(\'{{image}}\')" ></div><div class="insta-likes"><div class="likes"><div class="heart-blink"><i class="fa fa-heart"><span>{{likes}}</span></i></div></div></div></a></div>',resolution:"standard_resolution"}).run()});
                    //]]>
                  </script>
                </div><!--/insta widget-->
              </div>
              <div class='row'>
                <div class='col-sm-12 tfoot'>
                  <div class='footer-outer'>
                    <div class='footer-cap-top cap-top'>
                      <div class='cap-left'/>
                      <div class='cap-right'/>
                    </div>
                    <div class='fauxborder-left footer-fauxborder-left'>
                      <div class='fauxborder-right footer-fauxborder-right'/>
                      <div class='region-inner footer-inner'>
                        <macro:include id='footer-sections' name='sections'>
                          <macro:param default='2' name='num' value='3'/>
                          <macro:param default='footer' name='idPrefix'/>
                          <macro:param default='foot' name='class'/>
                          <macro:param default='false' name='includeBottom'/>
                        </macro:include>
                        <!-- outside of the include in order to lock Attribution widget -->

                      </div>
                    </div>
                    <div class='footer-cap-bottom cap-bottom'>
                      <div class='cap-left'/>
                      <div class='cap-right'/>
                    </div>
                  </div>
                </div></div>
              <div class='row' id='creditlink'>
                <div class='col-sm-12 text-center' id='credit-blsm'>
                  (C) Copyright 2017, <a expr:href='data:blog.homepageUrl'><data:blog.title/></a> | Designed by <a href='https://colorlib.com'>Colorlib</a>.
                </div>
              </div>
            </div>
          </footer>

        </div>
      </div><!--/contentarea-->

    </div><!--content wrapper-->

    <svg class='hidden'>
      <defs>
        <symbol id='icon-arrow' viewBox='0 0 24 24'>
          <title>arrow</title>
          <polygon points='6.3,12.8 20.9,12.8 20.9,11.2 6.3,11.2 10.2,7.2 9,6 3.1,12 9,18 10.2,16.8 '/>
        </symbol>
        <symbol id='icon-drop' viewBox='0 0 24 24'>
          <title>drop</title>
          <path d='M12,21c-3.6,0-6.6-3-6.6-6.6C5.4,11,10.8,4,11.4,3.2C11.6,3.1,11.8,3,12,3s0.4,0.1,0.6,0.3c0.6,0.8,6.1,7.8,6.1,11.2C18.6,18.1,15.6,21,12,21zM12,4.8c-1.8,2.4-5.2,7.4-5.2,9.6c0,2.9,2.3,5.2,5.2,5.2s5.2-2.3,5.2-5.2C17.2,12.2,13.8,7.3,12,4.8z'/><path d='M12,18.2c-0.4,0-0.7-0.3-0.7-0.7s0.3-0.7,0.7-0.7c1.3,0,2.4-1.1,2.4-2.4c0-0.4,0.3-0.7,0.7-0.7c0.4,0,0.7,0.3,0.7,0.7C15.8,16.5,14.1,18.2,12,18.2z'/>
        </symbol>
        <symbol id='icon-search' viewBox='0 0 24 24'>
          <title>search</title>
          <path d='M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z'/>
        </symbol>
        <symbol id='icon-cross' viewBox='0 0 24 24'>
          <title>cross</title>
          <path d='M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z'/>
        </symbol>
      </defs>
    </svg>
    <div class='search search--open hidden' id='searchbox' style='position: fixed;top: 0px;left: 0px;width: 100%;'>
      <button aria-label='Close search form' class='btn btn--search-close' id='btn-search-close'><svg class='icon icon--cross'><use xlink:href='#icon-cross'/></svg></button>
      <form action='/search' class='search__form'>
        <input class='search__input' name='q' placeholder='Search' type='search'/><br/>

        <span class='search__info'>Hit enter to search..</span>
      </form>
    </div>

    <script type='text/javascript'>
      //<![CDATA[
      function msieversion(){return(window.navigator.userAgent.indexOf("MSIE ")>0||navigator.userAgent.match(/Trident.*rv\:11\./))&&jQuery("body").append("<style>.grid-item{opacity:1 !important}</style>"),!1}var $=jQuery;$("#headercopy").html($("#Header").html()),msieversion();
      //]]>
    </script>
    <script type='text/javascript'>
      //<![CDATA[
      /*
 * jQuery Superfish Menu Plugin
 * Copyright (c) 2013 Joel Birch
 *
 * Dual licensed under the MIT and GPL licenses:
 *	http://www.opensource.org/licenses/mit-license.php
 *	http://www.gnu.org/licenses/gpl.html
 */
      !function(e,s){"use strict";var n=function(){var n={bcClass:"sf-breadcrumb",menuClass:"sf-js-enabled",anchorClass:"sf-with-ul",menuArrowClass:"sf-arrows"},o=function(){var s=/^(?![\w\W]*Windows Phone)[\w\W]*(iPhone|iPad|iPod)/i.test(navigator.userAgent);return s&&e("html").css("cursor","pointer").on("click",e.noop),s}(),t=function(){var e=document.documentElement.style;return"behavior"in e&&"fill"in e&&/iemobile/i.test(navigator.userAgent)}(),i=!!s.PointerEvent,r=function(e,s,o){var t=n.menuClass;s.cssArrows&&(t+=" "+n.menuArrowClass),e[o?"addClass":"removeClass"](t)},a=function(s,o){return s.find("li."+o.pathClass).slice(0,o.pathLevels).addClass(o.hoverClass+" "+n.bcClass).filter(function(){return e(this).children(o.popUpSelector).hide().show().length}).removeClass(o.pathClass)},l=function(e,s){var o=s?"addClass":"removeClass";e.children("a")[o](n.anchorClass)},h=function(e){var s=e.css("ms-touch-action"),n=e.css("touch-action");n="pan-y"===(n=n||s)?"auto":"pan-y",e.css({"ms-touch-action":n,"touch-action":n})},u=function(e){return e.closest("."+n.menuClass)},p=function(e){return u(e).data("sfOptions")},c=function(){var s=e(this),n=p(s);clearTimeout(n.sfTimer),s.siblings().superfish("hide").end().superfish("show")},f=function(s){s.retainPath=e.inArray(this[0],s.$path)>-1,this.superfish("hide"),this.parents("."+s.hoverClass).length||(s.onIdle.call(u(this)),s.$path.length&&e.proxy(c,s.$path)())},d=function(){var s=e(this),n=p(s);o?e.proxy(f,s,n)():(clearTimeout(n.sfTimer),n.sfTimer=setTimeout(e.proxy(f,s,n),n.delay))},v=function(s){var n=e(this),o=p(n),t=n.siblings(s.data.popUpSelector);if(!1===o.onHandleTouch.call(t))return this;t.length>0&&t.is(":hidden")&&(n.one("click.superfish",!1),"MSPointerDown"===s.type||"pointerdown"===s.type?n.trigger("focus"):e.proxy(c,n.parent("li"))())},m=function(s,n){var r="li:has("+n.popUpSelector+")";e.fn.hoverIntent&&!n.disableHI?s.hoverIntent(c,d,r):s.on("mouseenter.superfish",r,c).on("mouseleave.superfish",r,d);var a="MSPointerDown.superfish";i&&(a="pointerdown.superfish"),o||(a+=" touchend.superfish"),t&&(a+=" mousedown.superfish"),s.on("focusin.superfish","li",c).on("focusout.superfish","li",d).on(a,"a",n,v)};return{hide:function(s){if(this.length){var n=this,o=p(n);if(!o)return this;var t=!0===o.retainPath?o.$path:"",i=n.find("li."+o.hoverClass).add(this).not(t).removeClass(o.hoverClass).children(o.popUpSelector),r=o.speedOut;if(s&&(i.show(),r=0),o.retainPath=!1,!1===o.onBeforeHide.call(i))return this;i.stop(!0,!0).animate(o.animationOut,r,function(){var s=e(this);o.onHide.call(s)})}return this},show:function(){var e=p(this);if(!e)return this;var s=this.addClass(e.hoverClass).children(e.popUpSelector);return!1===e.onBeforeShow.call(s)?this:(s.stop(!0,!0).animate(e.animation,e.speed,function(){e.onShow.call(s)}),this)},destroy:function(){return this.each(function(){var s,o=e(this),t=o.data("sfOptions");if(!t)return!1;s=o.find(t.popUpSelector).parent("li"),clearTimeout(t.sfTimer),r(o,t),l(s),h(o),o.off(".superfish").off(".hoverIntent"),s.children(t.popUpSelector).attr("style",function(e,s){if(void 0!==s)return s.replace(/display[^;]+;?/g,"")}),t.$path.removeClass(t.hoverClass+" "+n.bcClass).addClass(t.pathClass),o.find("."+t.hoverClass).removeClass(t.hoverClass),t.onDestroy.call(o),o.removeData("sfOptions")})},init:function(s){return this.each(function(){var o=e(this);if(o.data("sfOptions"))return!1;var t=e.extend({},e.fn.superfish.defaults,s),i=o.find(t.popUpSelector).parent("li");t.$path=a(o,t),o.data("sfOptions",t),r(o,t,!0),l(i,!0),h(o),m(o,t),i.not("."+n.bcClass).superfish("hide",!0),t.onInit.call(this)})}}}();e.fn.superfish=function(s,o){return n[s]?n[s].apply(this,Array.prototype.slice.call(arguments,1)):"object"!=typeof s&&s?e.error("Method "+s+" does not exist on jQuery.fn.superfish"):n.init.apply(this,arguments)},e.fn.superfish.defaults={popUpSelector:"ul,.sf-mega",hoverClass:"sfHover",pathClass:"overrideThisToUse",pathLevels:1,delay:800,animation:{opacity:"show"},animationOut:{opacity:"hide"},speed:"normal",speedOut:"fast",cssArrows:!0,disableHI:!1,onInit:e.noop,onBeforeShow:e.noop,onShow:e.noop,onBeforeHide:e.noop,onHide:e.noop,onIdle:e.noop,onDestroy:e.noop,onHandleTouch:e.noop}}(jQuery,window);
      /*
 Sticky-kit v1.1.2 | WTFPL | Leaf Corcoran 2015 | http://leafo.net
*/
      // Generated by CoffeeScript 1.9.2
      (function(){var b,f;b=this.jQuery||window.jQuery;f=b(window);b.fn.stick_in_parent=function(d){var A,w,J,n,B,K,p,q,k,E,t;null==d&&(d={});t=d.sticky_class;B=d.inner_scrolling;E=d.recalc_every;k=d.parent;q=d.offset_top;p=d.spacer;w=d.bottoming;null==q&&(q=0);null==k&&(k=void 0);null==B&&(B=!0);null==t&&(t="is_stuck");A=b(document);null==w&&(w=!0);J=function(a,d,n,C,F,u,r,G){var v,H,m,D,I,c,g,x,y,z,h,l;if(!a.data("sticky_kit")){a.data("sticky_kit",!0);I=A.height();g=a.parent();null!=k&&(g=g.closest(k));
                                                                                                                                                                                                                                                                                                                                                                                                                                                  if(!g.length)throw"failed to find stick parent";v=m=!1;(h=null!=p?p&&a.closest(p):b("<div />"))&&h.css("position",a.css("position"));x=function(){var c,f,e;if(!G&&(I=A.height(),c=parseInt(g.css("border-top-width"),10),f=parseInt(g.css("padding-top"),10),d=parseInt(g.css("padding-bottom"),10),n=g.offset().top+c+f,C=g.height(),m&&(v=m=!1,null==p&&(a.insertAfter(h),h.detach()),a.css({position:"",top:"",width:"",bottom:""}).removeClass(t),e=!0),F=a.offset().top-(parseInt(a.css("margin-top"),10)||0)-q,
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      u=a.outerHeight(!0),r=a.css("float"),h&&h.css({width:a.outerWidth(!0),height:u,display:a.css("display"),"vertical-align":a.css("vertical-align"),"float":r}),e))return l()};x();if(u!==C)return D=void 0,c=q,z=E,l=function(){var b,l,e,k;if(!G&&(e=!1,null!=z&&(--z,0>=z&&(z=E,x(),e=!0)),e||A.height()===I||x(),e=f.scrollTop(),null!=D&&(l=e-D),D=e,m?(w&&(k=e+u+c>C+n,v&&!k&&(v=!1,a.css({position:"fixed",bottom:"",top:c}).trigger("sticky_kit:unbottom"))),e<F&&(m=!1,c=q,null==p&&("left"!==r&&"right"!==r||a.insertAfter(h),
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 h.detach()),b={position:"",width:"",top:""},a.css(b).removeClass(t).trigger("sticky_kit:unstick")),B&&(b=f.height(),u+q>b&&!v&&(c-=l,c=Math.max(b-u,c),c=Math.min(q,c),m&&a.css({top:c+"px"})))):e>F&&(m=!0,b={position:"fixed",top:c},b.width="border-box"===a.css("box-sizing")?a.outerWidth()+"px":a.width()+"px",a.css(b).addClass(t),null==p&&(a.after(h),"left"!==r&&"right"!==r||h.append(a)),a.trigger("sticky_kit:stick")),m&&w&&(null==k&&(k=e+u+c>C+n),!v&&k)))return v=!0,"static"===g.css("position")&&g.css({position:"relative"}),
                                                                                                                                                                                                                                                                                                                                                                                                                                                    a.css({position:"absolute",bottom:d,top:"auto"}).trigger("sticky_kit:bottom")},y=function(){x();return l()},H=function(){G=!0;f.off("touchmove",l);f.off("scroll",l);f.off("resize",y);b(document.body).off("sticky_kit:recalc",y);a.off("sticky_kit:detach",H);a.removeData("sticky_kit");a.css({position:"",bottom:"",top:"",width:""});g.position("position","");if(m)return null==p&&("left"!==r&&"right"!==r||a.insertAfter(h),h.remove()),a.removeClass(t)},f.on("touchmove",l),f.on("scroll",l),f.on("resize",
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                y),b(document.body).on("sticky_kit:recalc",y),a.on("sticky_kit:detach",H),setTimeout(l,0)}};n=0;for(K=this.length;n<K;n++)d=this[n],J(b(d));return this}}).call(this);
      /**
 * Owl Carousel v2.2.1
 * Copyright 2013-2017 David Deutsch
 * Licensed under  ()
 */
      !function(a,b,c,d){function e(b,c){this.settings=null,this.options=a.extend({},e.Defaults,c),this.$element=a(b),this._handlers={},this._plugins={},this._supress={},this._current=null,this._speed=null,this._coordinates=[],this._breakpoint=null,this._width=null,this._items=[],this._clones=[],this._mergers=[],this._widths=[],this._invalidated={},this._pipe=[],this._drag={time:null,target:null,pointer:null,stage:{start:null,current:null},direction:null},this._states={current:{},tags:{initializing:["busy"],animating:["busy"],dragging:["interacting"]}},a.each(["onResize","onThrottledResize"],a.proxy(function(b,c){this._handlers[c]=a.proxy(this[c],this)},this)),a.each(e.Plugins,a.proxy(function(a,b){this._plugins[a.charAt(0).toLowerCase()+a.slice(1)]=new b(this)},this)),a.each(e.Workers,a.proxy(function(b,c){this._pipe.push({filter:c.filter,run:a.proxy(c.run,this)})},this)),this.setup(),this.initialize()}e.Defaults={items:3,loop:!1,center:!1,rewind:!1,mouseDrag:!0,touchDrag:!0,pullDrag:!0,freeDrag:!1,margin:0,stagePadding:0,merge:!1,mergeFit:!0,autoWidth:!1,startPosition:0,rtl:!1,smartSpeed:250,fluidSpeed:!1,dragEndSpeed:!1,responsive:{},responsiveRefreshRate:200,responsiveBaseElement:b,fallbackEasing:"swing",info:!1,nestedItemSelector:!1,itemElement:"div",stageElement:"div",refreshClass:"owl-refresh",loadedClass:"owl-loaded",loadingClass:"owl-loading",rtlClass:"owl-rtl",responsiveClass:"owl-responsive",dragClass:"owl-drag",itemClass:"owl-item",stageClass:"owl-stage",stageOuterClass:"owl-stage-outer",grabClass:"owl-grab"},e.Width={Default:"default",Inner:"inner",Outer:"outer"},e.Type={Event:"event",State:"state"},e.Plugins={},e.Workers=[{filter:["width","settings"],run:function(){this._width=this.$element.width()}},{filter:["width","items","settings"],run:function(a){a.current=this._items&&this._items[this.relative(this._current)]}},{filter:["items","settings"],run:function(){this.$stage.children(".cloned").remove()}},{filter:["width","items","settings"],run:function(a){var b=this.settings.margin||"",c=!this.settings.autoWidth,d=this.settings.rtl,e={width:"auto","margin-left":d?b:"","margin-right":d?"":b};!c&&this.$stage.children().css(e),a.css=e}},{filter:["width","items","settings"],run:function(a){var b=(this.width()/this.settings.items).toFixed(3)-this.settings.margin,c=null,d=this._items.length,e=!this.settings.autoWidth,f=[];for(a.items={merge:!1,width:b};d--;)c=this._mergers[d],c=this.settings.mergeFit&&Math.min(c,this.settings.items)||c,a.items.merge=c>1||a.items.merge,f[d]=e?b*c:this._items[d].width();this._widths=f}},{filter:["items","settings"],run:function(){var b=[],c=this._items,d=this.settings,e=Math.max(2*d.items,4),f=2*Math.ceil(c.length/2),g=d.loop&&c.length?d.rewind?e:Math.max(e,f):0,h="",i="";for(g/=2;g--;)b.push(this.normalize(b.length/2,!0)),h+=c[b[b.length-1]][0].outerHTML,b.push(this.normalize(c.length-1-(b.length-1)/2,!0)),i=c[b[b.length-1]][0].outerHTML+i;this._clones=b,a(h).addClass("cloned").appendTo(this.$stage),a(i).addClass("cloned").prependTo(this.$stage)}},{filter:["width","items","settings"],run:function(){for(var a=this.settings.rtl?1:-1,b=this._clones.length+this._items.length,c=-1,d=0,e=0,f=[];++c<b;)d=f[c-1]||0,e=this._widths[this.relative(c)]+this.settings.margin,f.push(d+e*a);this._coordinates=f}},{filter:["width","items","settings"],run:function(){var a=this.settings.stagePadding,b=this._coordinates,c={width:Math.ceil(Math.abs(b[b.length-1]))+2*a,"padding-left":a||"","padding-right":a||""};this.$stage.css(c)}},{filter:["width","items","settings"],run:function(a){var b=this._coordinates.length,c=!this.settings.autoWidth,d=this.$stage.children();if(c&&a.items.merge)for(;b--;)a.css.width=this._widths[this.relative(b)],d.eq(b).css(a.css);else c&&(a.css.width=a.items.width,d.css(a.css))}},{filter:["items"],run:function(){this._coordinates.length<1&&this.$stage.removeAttr("style")}},{filter:["width","items","settings"],run:function(a){a.current=a.current?this.$stage.children().index(a.current):0,a.current=Math.max(this.minimum(),Math.min(this.maximum(),a.current)),this.reset(a.current)}},{filter:["position"],run:function(){this.animate(this.coordinates(this._current))}},{filter:["width","position","items","settings"],run:function(){var a,b,c,d,e=this.settings.rtl?1:-1,f=2*this.settings.stagePadding,g=this.coordinates(this.current())+f,h=g+this.width()*e,i=[];for(c=0,d=this._coordinates.length;c<d;c++)a=this._coordinates[c-1]||0,b=Math.abs(this._coordinates[c])+f*e,(this.op(a,"<=",g)&&this.op(a,">",h)||this.op(b,"<",g)&&this.op(b,">",h))&&i.push(c);this.$stage.children(".active").removeClass("active"),this.$stage.children(":eq("+i.join("), :eq(")+")").addClass("active"),this.settings.center&&(this.$stage.children(".center").removeClass("center"),this.$stage.children().eq(this.current()).addClass("center"))}}],e.prototype.initialize=function(){if(this.enter("initializing"),this.trigger("initialize"),this.$element.toggleClass(this.settings.rtlClass,this.settings.rtl),this.settings.autoWidth&&!this.is("pre-loading")){var b,c,e;b=this.$element.find("img"),c=this.settings.nestedItemSelector?"."+this.settings.nestedItemSelector:d,e=this.$element.children(c).width(),b.length&&e<=0&&this.preloadAutoWidthImages(b)}this.$element.addClass(this.options.loadingClass),this.$stage=a("<"+this.settings.stageElement+' class="'+this.settings.stageClass+'"/>').wrap('<div class="'+this.settings.stageOuterClass+'"/>'),this.$element.append(this.$stage.parent()),this.replace(this.$element.children().not(this.$stage.parent())),this.$element.is(":visible")?this.refresh():this.invalidate("width"),this.$element.removeClass(this.options.loadingClass).addClass(this.options.loadedClass),this.registerEventHandlers(),this.leave("initializing"),this.trigger("initialized")},e.prototype.setup=function(){var b=this.viewport(),c=this.options.responsive,d=-1,e=null;c?(a.each(c,function(a){a<=b&&a>d&&(d=Number(a))}),e=a.extend({},this.options,c[d]),"function"==typeof e.stagePadding&&(e.stagePadding=e.stagePadding()),delete e.responsive,e.responsiveClass&&this.$element.attr("class",this.$element.attr("class").replace(new RegExp("("+this.options.responsiveClass+"-)\\S+\\s","g"),"$1"+d))):e=a.extend({},this.options),this.trigger("change",{property:{name:"settings",value:e}}),this._breakpoint=d,this.settings=e,this.invalidate("settings"),this.trigger("changed",{property:{name:"settings",value:this.settings}})},e.prototype.optionsLogic=function(){this.settings.autoWidth&&(this.settings.stagePadding=!1,this.settings.merge=!1)},e.prototype.prepare=function(b){var c=this.trigger("prepare",{content:b});return c.data||(c.data=a("<"+this.settings.itemElement+"/>").addClass(this.options.itemClass).append(b)),this.trigger("prepared",{content:c.data}),c.data},e.prototype.update=function(){for(var b=0,c=this._pipe.length,d=a.proxy(function(a){return this[a]},this._invalidated),e={};b<c;)(this._invalidated.all||a.grep(this._pipe[b].filter,d).length>0)&&this._pipe[b].run(e),b++;this._invalidated={},!this.is("valid")&&this.enter("valid")},e.prototype.width=function(a){switch(a=a||e.Width.Default){case e.Width.Inner:case e.Width.Outer:return this._width;default:return this._width-2*this.settings.stagePadding+this.settings.margin}},e.prototype.refresh=function(){this.enter("refreshing"),this.trigger("refresh"),this.setup(),this.optionsLogic(),this.$element.addClass(this.options.refreshClass),this.update(),this.$element.removeClass(this.options.refreshClass),this.leave("refreshing"),this.trigger("refreshed")},e.prototype.onThrottledResize=function(){b.clearTimeout(this.resizeTimer),this.resizeTimer=b.setTimeout(this._handlers.onResize,this.settings.responsiveRefreshRate)},e.prototype.onResize=function(){return!!this._items.length&&(this._width!==this.$element.width()&&(!!this.$element.is(":visible")&&(this.enter("resizing"),this.trigger("resize").isDefaultPrevented()?(this.leave("resizing"),!1):(this.invalidate("width"),this.refresh(),this.leave("resizing"),void this.trigger("resized")))))},e.prototype.registerEventHandlers=function(){a.support.transition&&this.$stage.on(a.support.transition.end+".owl.core",a.proxy(this.onTransitionEnd,this)),this.settings.responsive!==!1&&this.on(b,"resize",this._handlers.onThrottledResize),this.settings.mouseDrag&&(this.$element.addClass(this.options.dragClass),this.$stage.on("mousedown.owl.core",a.proxy(this.onDragStart,this)),this.$stage.on("dragstart.owl.core selectstart.owl.core",function(){return!1})),this.settings.touchDrag&&(this.$stage.on("touchstart.owl.core",a.proxy(this.onDragStart,this)),this.$stage.on("touchcancel.owl.core",a.proxy(this.onDragEnd,this)))},e.prototype.onDragStart=function(b){var d=null;3!==b.which&&(a.support.transform?(d=this.$stage.css("transform").replace(/.*\(|\)| /g,"").split(","),d={x:d[16===d.length?12:4],y:d[16===d.length?13:5]}):(d=this.$stage.position(),d={x:this.settings.rtl?d.left+this.$stage.width()-this.width()+this.settings.margin:d.left,y:d.top}),this.is("animating")&&(a.support.transform?this.animate(d.x):this.$stage.stop(),this.invalidate("position")),this.$element.toggleClass(this.options.grabClass,"mousedown"===b.type),this.speed(0),this._drag.time=(new Date).getTime(),this._drag.target=a(b.target),this._drag.stage.start=d,this._drag.stage.current=d,this._drag.pointer=this.pointer(b),a(c).on("mouseup.owl.core touchend.owl.core",a.proxy(this.onDragEnd,this)),a(c).one("mousemove.owl.core touchmove.owl.core",a.proxy(function(b){var d=this.difference(this._drag.pointer,this.pointer(b));a(c).on("mousemove.owl.core touchmove.owl.core",a.proxy(this.onDragMove,this)),Math.abs(d.x)<Math.abs(d.y)&&this.is("valid")||(b.preventDefault(),this.enter("dragging"),this.trigger("drag"))},this)))},e.prototype.onDragMove=function(a){var b=null,c=null,d=null,e=this.difference(this._drag.pointer,this.pointer(a)),f=this.difference(this._drag.stage.start,e);this.is("dragging")&&(a.preventDefault(),this.settings.loop?(b=this.coordinates(this.minimum()),c=this.coordinates(this.maximum()+1)-b,f.x=((f.x-b)%c+c)%c+b):(b=this.settings.rtl?this.coordinates(this.maximum()):this.coordinates(this.minimum()),c=this.settings.rtl?this.coordinates(this.minimum()):this.coordinates(this.maximum()),d=this.settings.pullDrag?-1*e.x/5:0,f.x=Math.max(Math.min(f.x,b+d),c+d)),this._drag.stage.current=f,this.animate(f.x))},e.prototype.onDragEnd=function(b){var d=this.difference(this._drag.pointer,this.pointer(b)),e=this._drag.stage.current,f=d.x>0^this.settings.rtl?"left":"right";a(c).off(".owl.core"),this.$element.removeClass(this.options.grabClass),(0!==d.x&&this.is("dragging")||!this.is("valid"))&&(this.speed(this.settings.dragEndSpeed||this.settings.smartSpeed),this.current(this.closest(e.x,0!==d.x?f:this._drag.direction)),this.invalidate("position"),this.update(),this._drag.direction=f,(Math.abs(d.x)>3||(new Date).getTime()-this._drag.time>300)&&this._drag.target.one("click.owl.core",function(){return!1})),this.is("dragging")&&(this.leave("dragging"),this.trigger("dragged"))},e.prototype.closest=function(b,c){var d=-1,e=30,f=this.width(),g=this.coordinates();return this.settings.freeDrag||a.each(g,a.proxy(function(a,h){return"left"===c&&b>h-e&&b<h+e?d=a:"right"===c&&b>h-f-e&&b<h-f+e?d=a+1:this.op(b,"<",h)&&this.op(b,">",g[a+1]||h-f)&&(d="left"===c?a+1:a),d===-1},this)),this.settings.loop||(this.op(b,">",g[this.minimum()])?d=b=this.minimum():this.op(b,"<",g[this.maximum()])&&(d=b=this.maximum())),d},e.prototype.animate=function(b){var c=this.speed()>0;this.is("animating")&&this.onTransitionEnd(),c&&(this.enter("animating"),this.trigger("translate")),a.support.transform3d&&a.support.transition?this.$stage.css({transform:"translate3d("+b+"px,0px,0px)",transition:this.speed()/1e3+"s"}):c?this.$stage.animate({left:b+"px"},this.speed(),this.settings.fallbackEasing,a.proxy(this.onTransitionEnd,this)):this.$stage.css({left:b+"px"})},e.prototype.is=function(a){return this._states.current[a]&&this._states.current[a]>0},e.prototype.current=function(a){if(a===d)return this._current;if(0===this._items.length)return d;if(a=this.normalize(a),this._current!==a){var b=this.trigger("change",{property:{name:"position",value:a}});b.data!==d&&(a=this.normalize(b.data)),this._current=a,this.invalidate("position"),this.trigger("changed",{property:{name:"position",value:this._current}})}return this._current},e.prototype.invalidate=function(b){return"string"===a.type(b)&&(this._invalidated[b]=!0,this.is("valid")&&this.leave("valid")),a.map(this._invalidated,function(a,b){return b})},e.prototype.reset=function(a){a=this.normalize(a),a!==d&&(this._speed=0,this._current=a,this.suppress(["translate","translated"]),this.animate(this.coordinates(a)),this.release(["translate","translated"]))},e.prototype.normalize=function(a,b){var c=this._items.length,e=b?0:this._clones.length;return!this.isNumeric(a)||c<1?a=d:(a<0||a>=c+e)&&(a=((a-e/2)%c+c)%c+e/2),a},e.prototype.relative=function(a){return a-=this._clones.length/2,this.normalize(a,!0)},e.prototype.maximum=function(a){var b,c,d,e=this.settings,f=this._coordinates.length;if(e.loop)f=this._clones.length/2+this._items.length-1;else if(e.autoWidth||e.merge){for(b=this._items.length,c=this._items[--b].width(),d=this.$element.width();b--&&(c+=this._items[b].width()+this.settings.margin,!(c>d)););f=b+1}else f=e.center?this._items.length-1:this._items.length-e.items;return a&&(f-=this._clones.length/2),Math.max(f,0)},e.prototype.minimum=function(a){return a?0:this._clones.length/2},e.prototype.items=function(a){return a===d?this._items.slice():(a=this.normalize(a,!0),this._items[a])},e.prototype.mergers=function(a){return a===d?this._mergers.slice():(a=this.normalize(a,!0),this._mergers[a])},e.prototype.clones=function(b){var c=this._clones.length/2,e=c+this._items.length,f=function(a){return a%2===0?e+a/2:c-(a+1)/2};return b===d?a.map(this._clones,function(a,b){return f(b)}):a.map(this._clones,function(a,c){return a===b?f(c):null})},e.prototype.speed=function(a){return a!==d&&(this._speed=a),this._speed},e.prototype.coordinates=function(b){var c,e=1,f=b-1;return b===d?a.map(this._coordinates,a.proxy(function(a,b){return this.coordinates(b)},this)):(this.settings.center?(this.settings.rtl&&(e=-1,f=b+1),c=this._coordinates[b],c+=(this.width()-c+(this._coordinates[f]||0))/2*e):c=this._coordinates[f]||0,c=Math.ceil(c))},e.prototype.duration=function(a,b,c){return 0===c?0:Math.min(Math.max(Math.abs(b-a),1),6)*Math.abs(c||this.settings.smartSpeed)},e.prototype.to=function(a,b){var c=this.current(),d=null,e=a-this.relative(c),f=(e>0)-(e<0),g=this._items.length,h=this.minimum(),i=this.maximum();this.settings.loop?(!this.settings.rewind&&Math.abs(e)>g/2&&(e+=f*-1*g),a=c+e,d=((a-h)%g+g)%g+h,d!==a&&d-e<=i&&d-e>0&&(c=d-e,a=d,this.reset(c))):this.settings.rewind?(i+=1,a=(a%i+i)%i):a=Math.max(h,Math.min(i,a)),this.speed(this.duration(c,a,b)),this.current(a),this.$element.is(":visible")&&this.update()},e.prototype.next=function(a){a=a||!1,this.to(this.relative(this.current())+1,a)},e.prototype.prev=function(a){a=a||!1,this.to(this.relative(this.current())-1,a)},e.prototype.onTransitionEnd=function(a){if(a!==d&&(a.stopPropagation(),(a.target||a.srcElement||a.originalTarget)!==this.$stage.get(0)))return!1;this.leave("animating"),this.trigger("translated")},e.prototype.viewport=function(){var d;return this.options.responsiveBaseElement!==b?d=a(this.options.responsiveBaseElement).width():b.innerWidth?d=b.innerWidth:c.documentElement&&c.documentElement.clientWidth?d=c.documentElement.clientWidth:console.warn("Can not detect viewport width."),d},e.prototype.replace=function(b){this.$stage.empty(),this._items=[],b&&(b=b instanceof jQuery?b:a(b)),this.settings.nestedItemSelector&&(b=b.find("."+this.settings.nestedItemSelector)),b.filter(function(){return 1===this.nodeType}).each(a.proxy(function(a,b){b=this.prepare(b),this.$stage.append(b),this._items.push(b),this._mergers.push(1*b.find("[data-merge]").addBack("[data-merge]").attr("data-merge")||1)},this)),this.reset(this.isNumeric(this.settings.startPosition)?this.settings.startPosition:0),this.invalidate("items")},e.prototype.add=function(b,c){var e=this.relative(this._current);c=c===d?this._items.length:this.normalize(c,!0),b=b instanceof jQuery?b:a(b),this.trigger("add",{content:b,position:c}),b=this.prepare(b),0===this._items.length||c===this._items.length?(0===this._items.length&&this.$stage.append(b),0!==this._items.length&&this._items[c-1].after(b),this._items.push(b),this._mergers.push(1*b.find("[data-merge]").addBack("[data-merge]").attr("data-merge")||1)):(this._items[c].before(b),this._items.splice(c,0,b),this._mergers.splice(c,0,1*b.find("[data-merge]").addBack("[data-merge]").attr("data-merge")||1)),this._items[e]&&this.reset(this._items[e].index()),this.invalidate("items"),this.trigger("added",{content:b,position:c})},e.prototype.remove=function(a){a=this.normalize(a,!0),a!==d&&(this.trigger("remove",{content:this._items[a],position:a}),this._items[a].remove(),this._items.splice(a,1),this._mergers.splice(a,1),this.invalidate("items"),this.trigger("removed",{content:null,position:a}))},e.prototype.preloadAutoWidthImages=function(b){b.each(a.proxy(function(b,c){this.enter("pre-loading"),c=a(c),a(new Image).one("load",a.proxy(function(a){c.attr("src",a.target.src),c.css("opacity",1),this.leave("pre-loading"),!this.is("pre-loading")&&!this.is("initializing")&&this.refresh()},this)).attr("src",c.attr("src")||c.attr("data-src")||c.attr("data-src-retina"))},this))},e.prototype.destroy=function(){this.$element.off(".owl.core"),this.$stage.off(".owl.core"),a(c).off(".owl.core"),this.settings.responsive!==!1&&(b.clearTimeout(this.resizeTimer),this.off(b,"resize",this._handlers.onThrottledResize));for(var d in this._plugins)this._plugins[d].destroy();this.$stage.children(".cloned").remove(),this.$stage.unwrap(),this.$stage.children().contents().unwrap(),this.$stage.children().unwrap(),this.$element.removeClass(this.options.refreshClass).removeClass(this.options.loadingClass).removeClass(this.options.loadedClass).removeClass(this.options.rtlClass).removeClass(this.options.dragClass).removeClass(this.options.grabClass).attr("class",this.$element.attr("class").replace(new RegExp(this.options.responsiveClass+"-\\S+\\s","g"),"")).removeData("owl.carousel")},e.prototype.op=function(a,b,c){var d=this.settings.rtl;switch(b){case"<":return d?a>c:a<c;case">":return d?a<c:a>c;case">=":return d?a<=c:a>=c;case"<=":return d?a>=c:a<=c}},e.prototype.on=function(a,b,c,d){a.addEventListener?a.addEventListener(b,c,d):a.attachEvent&&a.attachEvent("on"+b,c)},e.prototype.off=function(a,b,c,d){a.removeEventListener?a.removeEventListener(b,c,d):a.detachEvent&&a.detachEvent("on"+b,c)},e.prototype.trigger=function(b,c,d,f,g){var h={item:{count:this._items.length,index:this.current()}},i=a.camelCase(a.grep(["on",b,d],function(a){return a}).join("-").toLowerCase()),j=a.Event([b,"owl",d||"carousel"].join(".").toLowerCase(),a.extend({relatedTarget:this},h,c));return this._supress[b]||(a.each(this._plugins,function(a,b){b.onTrigger&&b.onTrigger(j)}),this.register({type:e.Type.Event,name:b}),this.$element.trigger(j),this.settings&&"function"==typeof this.settings[i]&&this.settings[i].call(this,j)),j},e.prototype.enter=function(b){a.each([b].concat(this._states.tags[b]||[]),a.proxy(function(a,b){this._states.current[b]===d&&(this._states.current[b]=0),this._states.current[b]++},this))},e.prototype.leave=function(b){a.each([b].concat(this._states.tags[b]||[]),a.proxy(function(a,b){this._states.current[b]--},this))},e.prototype.register=function(b){if(b.type===e.Type.Event){if(a.event.special[b.name]||(a.event.special[b.name]={}),!a.event.special[b.name].owl){var c=a.event.special[b.name]._default;a.event.special[b.name]._default=function(a){return!c||!c.apply||a.namespace&&a.namespace.indexOf("owl")!==-1?a.namespace&&a.namespace.indexOf("owl")>-1:c.apply(this,arguments)},a.event.special[b.name].owl=!0}}else b.type===e.Type.State&&(this._states.tags[b.name]?this._states.tags[b.name]=this._states.tags[b.name].concat(b.tags):this._states.tags[b.name]=b.tags,this._states.tags[b.name]=a.grep(this._states.tags[b.name],a.proxy(function(c,d){return a.inArray(c,this._states.tags[b.name])===d},this)))},e.prototype.suppress=function(b){a.each(b,a.proxy(function(a,b){this._supress[b]=!0},this))},e.prototype.release=function(b){a.each(b,a.proxy(function(a,b){delete this._supress[b]},this))},e.prototype.pointer=function(a){var c={x:null,y:null};return a=a.originalEvent||a||b.event,a=a.touches&&a.touches.length?a.touches[0]:a.changedTouches&&a.changedTouches.length?a.changedTouches[0]:a,a.pageX?(c.x=a.pageX,c.y=a.pageY):(c.x=a.clientX,c.y=a.clientY),c},e.prototype.isNumeric=function(a){return!isNaN(parseFloat(a))},e.prototype.difference=function(a,b){return{x:a.x-b.x,y:a.y-b.y}},a.fn.owlCarousel=function(b){var c=Array.prototype.slice.call(arguments,1);return this.each(function(){var d=a(this),f=d.data("owl.carousel");f||(f=new e(this,"object"==typeof b&&b),d.data("owl.carousel",f),a.each(["next","prev","to","destroy","refresh","replace","add","remove"],function(b,c){f.register({type:e.Type.Event,name:c}),f.$element.on(c+".owl.carousel.core",a.proxy(function(a){a.namespace&&a.relatedTarget!==this&&(this.suppress([c]),f[c].apply(this,[].slice.call(arguments,1)),this.release([c]))},f))})),"string"==typeof b&&"_"!==b.charAt(0)&&f[b].apply(f,c)})},a.fn.owlCarousel.Constructor=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){var e=function(b){this._core=b,this._interval=null,this._visible=null,this._handlers={"initialized.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.autoRefresh&&this.watch()},this)},this._core.options=a.extend({},e.Defaults,this._core.options),this._core.$element.on(this._handlers)};e.Defaults={autoRefresh:!0,autoRefreshInterval:500},e.prototype.watch=function(){this._interval||(this._visible=this._core.$element.is(":visible"),this._interval=b.setInterval(a.proxy(this.refresh,this),this._core.settings.autoRefreshInterval))},e.prototype.refresh=function(){this._core.$element.is(":visible")!==this._visible&&(this._visible=!this._visible,this._core.$element.toggleClass("owl-hidden",!this._visible),this._visible&&this._core.invalidate("width")&&this._core.refresh())},e.prototype.destroy=function(){var a,c;b.clearInterval(this._interval);for(a in this._handlers)this._core.$element.off(a,this._handlers[a]);for(c in Object.getOwnPropertyNames(this))"function"!=typeof this[c]&&(this[c]=null)},a.fn.owlCarousel.Constructor.Plugins.AutoRefresh=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){var e=function(b){this._core=b,this._loaded=[],this._handlers={"initialized.owl.carousel change.owl.carousel resized.owl.carousel":a.proxy(function(b){if(b.namespace&&this._core.settings&&this._core.settings.lazyLoad&&(b.property&&"position"==b.property.name||"initialized"==b.type))for(var c=this._core.settings,e=c.center&&Math.ceil(c.items/2)||c.items,f=c.center&&e*-1||0,g=(b.property&&b.property.value!==d?b.property.value:this._core.current())+f,h=this._core.clones().length,i=a.proxy(function(a,b){this.load(b)},this);f++<e;)this.load(h/2+this._core.relative(g)),h&&a.each(this._core.clones(this._core.relative(g)),i),g++},this)},this._core.options=a.extend({},e.Defaults,this._core.options),this._core.$element.on(this._handlers)};e.Defaults={lazyLoad:!1},e.prototype.load=function(c){var d=this._core.$stage.children().eq(c),e=d&&d.find(".owl-lazy");!e||a.inArray(d.get(0),this._loaded)>-1||(e.each(a.proxy(function(c,d){var e,f=a(d),g=b.devicePixelRatio>1&&f.attr("data-src-retina")||f.attr("data-src");this._core.trigger("load",{element:f,url:g},"lazy"),f.is("img")?f.one("load.owl.lazy",a.proxy(function(){f.css("opacity",1),this._core.trigger("loaded",{element:f,url:g},"lazy")},this)).attr("src",g):(e=new Image,e.onload=a.proxy(function(){f.css({"background-image":'url("'+g+'")',opacity:"1"}),this._core.trigger("loaded",{element:f,url:g},"lazy")},this),e.src=g)},this)),this._loaded.push(d.get(0)))},e.prototype.destroy=function(){var a,b;for(a in this.handlers)this._core.$element.off(a,this.handlers[a]);for(b in Object.getOwnPropertyNames(this))"function"!=typeof this[b]&&(this[b]=null)},a.fn.owlCarousel.Constructor.Plugins.Lazy=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){var e=function(b){this._core=b,this._handlers={"initialized.owl.carousel refreshed.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.autoHeight&&this.update()},this),"changed.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.autoHeight&&"position"==a.property.name&&this.update()},this),"loaded.owl.lazy":a.proxy(function(a){a.namespace&&this._core.settings.autoHeight&&a.element.closest("."+this._core.settings.itemClass).index()===this._core.current()&&this.update()},this)},this._core.options=a.extend({},e.Defaults,this._core.options),this._core.$element.on(this._handlers)};e.Defaults={autoHeight:!1,autoHeightClass:"owl-height"},e.prototype.update=function(){var b=this._core._current,c=b+this._core.settings.items,d=this._core.$stage.children().toArray().slice(b,c),e=[],f=0;a.each(d,function(b,c){e.push(a(c).height())}),f=Math.max.apply(null,e),this._core.$stage.parent().height(f).addClass(this._core.settings.autoHeightClass)},e.prototype.destroy=function(){var a,b;for(a in this._handlers)this._core.$element.off(a,this._handlers[a]);for(b in Object.getOwnPropertyNames(this))"function"!=typeof this[b]&&(this[b]=null)},a.fn.owlCarousel.Constructor.Plugins.AutoHeight=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){var e=function(b){this._core=b,this._videos={},this._playing=null,this._handlers={"initialized.owl.carousel":a.proxy(function(a){a.namespace&&this._core.register({type:"state",name:"playing",tags:["interacting"]})},this),"resize.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.video&&this.isInFullScreen()&&a.preventDefault()},this),"refreshed.owl.carousel":a.proxy(function(a){a.namespace&&this._core.is("resizing")&&this._core.$stage.find(".cloned .owl-video-frame").remove()},this),"changed.owl.carousel":a.proxy(function(a){a.namespace&&"position"===a.property.name&&this._playing&&this.stop()},this),"prepared.owl.carousel":a.proxy(function(b){if(b.namespace){var c=a(b.content).find(".owl-video");c.length&&(c.css("display","none"),this.fetch(c,a(b.content)))}},this)},this._core.options=a.extend({},e.Defaults,this._core.options),this._core.$element.on(this._handlers),this._core.$element.on("click.owl.video",".owl-video-play-icon",a.proxy(function(a){this.play(a)},this))};e.Defaults={video:!1,videoHeight:!1,videoWidth:!1},e.prototype.fetch=function(a,b){var c=function(){return a.attr("data-vimeo-id")?"vimeo":a.attr("data-vzaar-id")?"vzaar":"youtube"}(),d=a.attr("data-vimeo-id")||a.attr("data-youtube-id")||a.attr("data-vzaar-id"),e=a.attr("data-width")||this._core.settings.videoWidth,f=a.attr("data-height")||this._core.settings.videoHeight,g=a.attr("href");if(!g)throw new Error("Missing video URL.");if(d=g.match(/(http:|https:|)\/\/(player.|www.|app.)?(vimeo\.com|youtu(be\.com|\.be|be\.googleapis\.com)|vzaar\.com)\/(video\/|videos\/|embed\/|channels\/.+\/|groups\/.+\/|watch\?v=|v\/)?([A-Za-z0-9._%-]*)(\&\S+)?/),d[3].indexOf("youtu")>-1)c="youtube";else if(d[3].indexOf("vimeo")>-1)c="vimeo";else{if(!(d[3].indexOf("vzaar")>-1))throw new Error("Video URL not supported.");c="vzaar"}d=d[6],this._videos[g]={type:c,id:d,width:e,height:f},b.attr("data-video",g),this.thumbnail(a,this._videos[g])},e.prototype.thumbnail=function(b,c){var d,e,f,g=c.width&&c.height?'style="width:'+c.width+"px;height:"+c.height+'px;"':"",h=b.find("img"),i="src",j="",k=this._core.settings,l=function(a){e='<div class="owl-video-play-icon"></div>',d=k.lazyLoad?'<div class="owl-video-tn '+j+'" '+i+'="'+a+'"></div>':'<div class="owl-video-tn" style="opacity:1;background-image:url('+a+')"></div>',b.after(d),b.after(e)};if(b.wrap('<div class="owl-video-wrapper"'+g+"></div>"),this._core.settings.lazyLoad&&(i="data-src",j="owl-lazy"),h.length)return l(h.attr(i)),h.remove(),!1;"youtube"===c.type?(f="//img.youtube.com/vi/"+c.id+"/hqdefault.jpg",l(f)):"vimeo"===c.type?a.ajax({type:"GET",url:"//vimeo.com/api/v2/video/"+c.id+".json",jsonp:"callback",dataType:"jsonp",success:function(a){f=a[0].thumbnail_large,l(f)}}):"vzaar"===c.type&&a.ajax({type:"GET",url:"//vzaar.com/api/videos/"+c.id+".json",jsonp:"callback",dataType:"jsonp",success:function(a){f=a.framegrab_url,l(f)}})},e.prototype.stop=function(){this._core.trigger("stop",null,"video"),this._playing.find(".owl-video-frame").remove(),this._playing.removeClass("owl-video-playing"),this._playing=null,this._core.leave("playing"),this._core.trigger("stopped",null,"video")},e.prototype.play=function(b){var c,d=a(b.target),e=d.closest("."+this._core.settings.itemClass),f=this._videos[e.attr("data-video")],g=f.width||"100%",h=f.height||this._core.$stage.height();this._playing||(this._core.enter("playing"),this._core.trigger("play",null,"video"),e=this._core.items(this._core.relative(e.index())),this._core.reset(e.index()),"youtube"===f.type?c='<iframe width="'+g+'" height="'+h+'" src="//www.youtube.com/embed/'+f.id+"?autoplay=1&rel=0&v="+f.id+'" frameborder="0" allowfullscreen></iframe>':"vimeo"===f.type?c='<iframe src="//player.vimeo.com/video/'+f.id+'?autoplay=1" width="'+g+'" height="'+h+'" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>':"vzaar"===f.type&&(c='<iframe frameborder="0"height="'+h+'"width="'+g+'" allowfullscreen mozallowfullscreen webkitAllowFullScreen src="//view.vzaar.com/'+f.id+'/player?autoplay=true"></iframe>'),a('<div class="owl-video-frame">'+c+"</div>").insertAfter(e.find(".owl-video")),this._playing=e.addClass("owl-video-playing"))},e.prototype.isInFullScreen=function(){var b=c.fullscreenElement||c.mozFullScreenElement||c.webkitFullscreenElement;return b&&a(b).parent().hasClass("owl-video-frame")},e.prototype.destroy=function(){var a,b;this._core.$element.off("click.owl.video");for(a in this._handlers)this._core.$element.off(a,this._handlers[a]);for(b in Object.getOwnPropertyNames(this))"function"!=typeof this[b]&&(this[b]=null)},a.fn.owlCarousel.Constructor.Plugins.Video=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){var e=function(b){this.core=b,this.core.options=a.extend({},e.Defaults,this.core.options),this.swapping=!0,this.previous=d,this.next=d,this.handlers={"change.owl.carousel":a.proxy(function(a){a.namespace&&"position"==a.property.name&&(this.previous=this.core.current(),this.next=a.property.value)},this),"drag.owl.carousel dragged.owl.carousel translated.owl.carousel":a.proxy(function(a){a.namespace&&(this.swapping="translated"==a.type)},this),"translate.owl.carousel":a.proxy(function(a){a.namespace&&this.swapping&&(this.core.options.animateOut||this.core.options.animateIn)&&this.swap()},this)},this.core.$element.on(this.handlers)};e.Defaults={animateOut:!1,animateIn:!1},e.prototype.swap=function(){if(1===this.core.settings.items&&a.support.animation&&a.support.transition){this.core.speed(0);var b,c=a.proxy(this.clear,this),d=this.core.$stage.children().eq(this.previous),e=this.core.$stage.children().eq(this.next),f=this.core.settings.animateIn,g=this.core.settings.animateOut;this.core.current()!==this.previous&&(g&&(b=this.core.coordinates(this.previous)-this.core.coordinates(this.next),d.one(a.support.animation.end,c).css({left:b+"px"}).addClass("animated owl-animated-out").addClass(g)),f&&e.one(a.support.animation.end,c).addClass("animated owl-animated-in").addClass(f))}},e.prototype.clear=function(b){a(b.target).css({left:""}).removeClass("animated owl-animated-out owl-animated-in").removeClass(this.core.settings.animateIn).removeClass(this.core.settings.animateOut),this.core.onTransitionEnd()},e.prototype.destroy=function(){var a,b;for(a in this.handlers)this.core.$element.off(a,this.handlers[a]);for(b in Object.getOwnPropertyNames(this))"function"!=typeof this[b]&&(this[b]=null)},
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          a.fn.owlCarousel.Constructor.Plugins.Animate=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){var e=function(b){this._core=b,this._timeout=null,this._paused=!1,this._handlers={"changed.owl.carousel":a.proxy(function(a){a.namespace&&"settings"===a.property.name?this._core.settings.autoplay?this.play():this.stop():a.namespace&&"position"===a.property.name&&this._core.settings.autoplay&&this._setAutoPlayInterval()},this),"initialized.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.autoplay&&this.play()},this),"play.owl.autoplay":a.proxy(function(a,b,c){a.namespace&&this.play(b,c)},this),"stop.owl.autoplay":a.proxy(function(a){a.namespace&&this.stop()},this),"mouseover.owl.autoplay":a.proxy(function(){this._core.settings.autoplayHoverPause&&this._core.is("rotating")&&this.pause()},this),"mouseleave.owl.autoplay":a.proxy(function(){this._core.settings.autoplayHoverPause&&this._core.is("rotating")&&this.play()},this),"touchstart.owl.core":a.proxy(function(){this._core.settings.autoplayHoverPause&&this._core.is("rotating")&&this.pause()},this),"touchend.owl.core":a.proxy(function(){this._core.settings.autoplayHoverPause&&this.play()},this)},this._core.$element.on(this._handlers),this._core.options=a.extend({},e.Defaults,this._core.options)};e.Defaults={autoplay:!1,autoplayTimeout:5e3,autoplayHoverPause:!1,autoplaySpeed:!1},e.prototype.play=function(a,b){this._paused=!1,this._core.is("rotating")||(this._core.enter("rotating"),this._setAutoPlayInterval())},e.prototype._getNextTimeout=function(d,e){return this._timeout&&b.clearTimeout(this._timeout),b.setTimeout(a.proxy(function(){this._paused||this._core.is("busy")||this._core.is("interacting")||c.hidden||this._core.next(e||this._core.settings.autoplaySpeed)},this),d||this._core.settings.autoplayTimeout)},e.prototype._setAutoPlayInterval=function(){this._timeout=this._getNextTimeout()},e.prototype.stop=function(){this._core.is("rotating")&&(b.clearTimeout(this._timeout),this._core.leave("rotating"))},e.prototype.pause=function(){this._core.is("rotating")&&(this._paused=!0)},e.prototype.destroy=function(){var a,b;this.stop();for(a in this._handlers)this._core.$element.off(a,this._handlers[a]);for(b in Object.getOwnPropertyNames(this))"function"!=typeof this[b]&&(this[b]=null)},a.fn.owlCarousel.Constructor.Plugins.autoplay=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){"use strict";var e=function(b){this._core=b,this._initialized=!1,this._pages=[],this._controls={},this._templates=[],this.$element=this._core.$element,this._overrides={next:this._core.next,prev:this._core.prev,to:this._core.to},this._handlers={"prepared.owl.carousel":a.proxy(function(b){b.namespace&&this._core.settings.dotsData&&this._templates.push('<div class="'+this._core.settings.dotClass+'">'+a(b.content).find("[data-dot]").addBack("[data-dot]").attr("data-dot")+"</div>")},this),"added.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.dotsData&&this._templates.splice(a.position,0,this._templates.pop())},this),"remove.owl.carousel":a.proxy(function(a){a.namespace&&this._core.settings.dotsData&&this._templates.splice(a.position,1)},this),"changed.owl.carousel":a.proxy(function(a){a.namespace&&"position"==a.property.name&&this.draw()},this),"initialized.owl.carousel":a.proxy(function(a){a.namespace&&!this._initialized&&(this._core.trigger("initialize",null,"navigation"),this.initialize(),this.update(),this.draw(),this._initialized=!0,this._core.trigger("initialized",null,"navigation"))},this),"refreshed.owl.carousel":a.proxy(function(a){a.namespace&&this._initialized&&(this._core.trigger("refresh",null,"navigation"),this.update(),this.draw(),this._core.trigger("refreshed",null,"navigation"))},this)},this._core.options=a.extend({},e.Defaults,this._core.options),this.$element.on(this._handlers)};e.Defaults={nav:!1,navText:["prev","next"],navSpeed:!1,navElement:"div",navContainer:!1,navContainerClass:"owl-nav",navClass:["owl-prev","owl-next"],slideBy:1,dotClass:"owl-dot",dotsClass:"owl-dots",dots:!0,dotsEach:!1,dotsData:!1,dotsSpeed:!1,dotsContainer:!1},e.prototype.initialize=function(){var b,c=this._core.settings;this._controls.$relative=(c.navContainer?a(c.navContainer):a("<div>").addClass(c.navContainerClass).appendTo(this.$element)).addClass("disabled"),this._controls.$previous=a("<"+c.navElement+">").addClass(c.navClass[0]).html(c.navText[0]).prependTo(this._controls.$relative).on("click",a.proxy(function(a){this.prev(c.navSpeed)},this)),this._controls.$next=a("<"+c.navElement+">").addClass(c.navClass[1]).html(c.navText[1]).appendTo(this._controls.$relative).on("click",a.proxy(function(a){this.next(c.navSpeed)},this)),c.dotsData||(this._templates=[a("<div>").addClass(c.dotClass).append(a("<span>")).prop("outerHTML")]),this._controls.$absolute=(c.dotsContainer?a(c.dotsContainer):a("<div>").addClass(c.dotsClass).appendTo(this.$element)).addClass("disabled"),this._controls.$absolute.on("click","div",a.proxy(function(b){var d=a(b.target).parent().is(this._controls.$absolute)?a(b.target).index():a(b.target).parent().index();b.preventDefault(),this.to(d,c.dotsSpeed)},this));for(b in this._overrides)this._core[b]=a.proxy(this[b],this)},e.prototype.destroy=function(){var a,b,c,d;for(a in this._handlers)this.$element.off(a,this._handlers[a]);for(b in this._controls)this._controls[b].remove();for(d in this.overides)this._core[d]=this._overrides[d];for(c in Object.getOwnPropertyNames(this))"function"!=typeof this[c]&&(this[c]=null)},e.prototype.update=function(){var a,b,c,d=this._core.clones().length/2,e=d+this._core.items().length,f=this._core.maximum(!0),g=this._core.settings,h=g.center||g.autoWidth||g.dotsData?1:g.dotsEach||g.items;if("page"!==g.slideBy&&(g.slideBy=Math.min(g.slideBy,g.items)),g.dots||"page"==g.slideBy)for(this._pages=[],a=d,b=0,c=0;a<e;a++){if(b>=h||0===b){if(this._pages.push({start:Math.min(f,a-d),end:a-d+h-1}),Math.min(f,a-d)===f)break;b=0,++c}b+=this._core.mergers(this._core.relative(a))}},e.prototype.draw=function(){var b,c=this._core.settings,d=this._core.items().length<=c.items,e=this._core.relative(this._core.current()),f=c.loop||c.rewind;this._controls.$relative.toggleClass("disabled",!c.nav||d),c.nav&&(this._controls.$previous.toggleClass("disabled",!f&&e<=this._core.minimum(!0)),this._controls.$next.toggleClass("disabled",!f&&e>=this._core.maximum(!0))),this._controls.$absolute.toggleClass("disabled",!c.dots||d),c.dots&&(b=this._pages.length-this._controls.$absolute.children().length,c.dotsData&&0!==b?this._controls.$absolute.html(this._templates.join("")):b>0?this._controls.$absolute.append(new Array(b+1).join(this._templates[0])):b<0&&this._controls.$absolute.children().slice(b).remove(),this._controls.$absolute.find(".active").removeClass("active"),this._controls.$absolute.children().eq(a.inArray(this.current(),this._pages)).addClass("active"))},e.prototype.onTrigger=function(b){var c=this._core.settings;b.page={index:a.inArray(this.current(),this._pages),count:this._pages.length,size:c&&(c.center||c.autoWidth||c.dotsData?1:c.dotsEach||c.items)}},e.prototype.current=function(){var b=this._core.relative(this._core.current());return a.grep(this._pages,a.proxy(function(a,c){return a.start<=b&&a.end>=b},this)).pop()},e.prototype.getPosition=function(b){var c,d,e=this._core.settings;return"page"==e.slideBy?(c=a.inArray(this.current(),this._pages),d=this._pages.length,b?++c:--c,c=this._pages[(c%d+d)%d].start):(c=this._core.relative(this._core.current()),d=this._core.items().length,b?c+=e.slideBy:c-=e.slideBy),c},e.prototype.next=function(b){a.proxy(this._overrides.to,this._core)(this.getPosition(!0),b)},e.prototype.prev=function(b){a.proxy(this._overrides.to,this._core)(this.getPosition(!1),b)},e.prototype.to=function(b,c,d){var e;!d&&this._pages.length?(e=this._pages.length,a.proxy(this._overrides.to,this._core)(this._pages[(b%e+e)%e].start,c)):a.proxy(this._overrides.to,this._core)(b,c)},a.fn.owlCarousel.Constructor.Plugins.Navigation=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){"use strict";var e=function(c){this._core=c,this._hashes={},this.$element=this._core.$element,this._handlers={"initialized.owl.carousel":a.proxy(function(c){c.namespace&&"URLHash"===this._core.settings.startPosition&&a(b).trigger("hashchange.owl.navigation")},this),"prepared.owl.carousel":a.proxy(function(b){if(b.namespace){var c=a(b.content).find("[data-hash]").addBack("[data-hash]").attr("data-hash");if(!c)return;this._hashes[c]=b.content}},this),"changed.owl.carousel":a.proxy(function(c){if(c.namespace&&"position"===c.property.name){var d=this._core.items(this._core.relative(this._core.current())),e=a.map(this._hashes,function(a,b){return a===d?b:null}).join();if(!e||b.location.hash.slice(1)===e)return;b.location.hash=e}},this)},this._core.options=a.extend({},e.Defaults,this._core.options),this.$element.on(this._handlers),a(b).on("hashchange.owl.navigation",a.proxy(function(a){var c=b.location.hash.substring(1),e=this._core.$stage.children(),f=this._hashes[c]&&e.index(this._hashes[c]);f!==d&&f!==this._core.current()&&this._core.to(this._core.relative(f),!1,!0)},this))};e.Defaults={URLhashListener:!1},e.prototype.destroy=function(){var c,d;a(b).off("hashchange.owl.navigation");for(c in this._handlers)this._core.$element.off(c,this._handlers[c]);for(d in Object.getOwnPropertyNames(this))"function"!=typeof this[d]&&(this[d]=null)},a.fn.owlCarousel.Constructor.Plugins.Hash=e}(window.Zepto||window.jQuery,window,document),function(a,b,c,d){function e(b,c){var e=!1,f=b.charAt(0).toUpperCase()+b.slice(1);return a.each((b+" "+h.join(f+" ")+f).split(" "),function(a,b){if(g[b]!==d)return e=!c||b,!1}),e}function f(a){return e(a,!0)}var g=a("<support>").get(0).style,h="Webkit Moz O ms".split(" "),i={transition:{end:{WebkitTransition:"webkitTransitionEnd",MozTransition:"transitionend",OTransition:"oTransitionEnd",transition:"transitionend"}},animation:{end:{WebkitAnimation:"webkitAnimationEnd",MozAnimation:"animationend",OAnimation:"oAnimationEnd",animation:"animationend"}}},j={csstransforms:function(){return!!e("transform")},csstransforms3d:function(){return!!e("perspective")},csstransitions:function(){return!!e("transition")},cssanimations:function(){return!!e("animation")}};j.csstransitions()&&(a.support.transition=new String(f("transition")),a.support.transition.end=i.transition.end[a.support.transition]),j.cssanimations()&&(a.support.animation=new String(f("animation")),a.support.animation.end=i.animation.end[a.support.animation]),j.csstransforms()&&(a.support.transform=new String(f("transform")),a.support.transform3d=j.csstransforms3d())}(window.Zepto||window.jQuery,window,document);
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          /*!
 * imagesLoaded PACKAGED v4.1.3
 * JavaScript is all like "You images are done yet or what?"
 * MIT License
 */

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          !function(e,t){"function"==typeof define&&define.amd?define("ev-emitter/ev-emitter",t):"object"==typeof module&&module.exports?module.exports=t():e.EvEmitter=t()}("undefined"!=typeof window?window:this,function(){function e(){}var t=e.prototype;return t.on=function(e,t){if(e&&t){var i=this._events=this._events||{},n=i[e]=i[e]||[];return-1==n.indexOf(t)&&n.push(t),this}},t.once=function(e,t){if(e&&t){this.on(e,t);var i=this._onceEvents=this._onceEvents||{},n=i[e]=i[e]||{};return n[t]=!0,this}},t.off=function(e,t){var i=this._events&&this._events[e];if(i&&i.length){var n=i.indexOf(t);return-1!=n&&i.splice(n,1),this}},t.emitEvent=function(e,t){var i=this._events&&this._events[e];if(i&&i.length){var n=0,o=i[n];t=t||[];for(var r=this._onceEvents&&this._onceEvents[e];o;){var s=r&&r[o];s&&(this.off(e,o),delete r[o]),o.apply(this,t),n+=s?0:1,o=i[n]}return this}},t.allOff=t.removeAllListeners=function(){delete this._events,delete this._onceEvents},e}),function(e,t){"use strict";"function"==typeof define&&define.amd?define(["ev-emitter/ev-emitter"],function(i){return t(e,i)}):"object"==typeof module&&module.exports?module.exports=t(e,require("ev-emitter")):e.imagesLoaded=t(e,e.EvEmitter)}("undefined"!=typeof window?window:this,function(e,t){function i(e,t){for(var i in t)e[i]=t[i];return e}function n(e){var t=[];if(Array.isArray(e))t=e;else if("number"==typeof e.length)for(var i=0;i<e.length;i++)t.push(e[i]);else t.push(e);return t}function o(e,t,r){return this instanceof o?("string"==typeof e&&(e=document.querySelectorAll(e)),this.elements=n(e),this.options=i({},this.options),"function"==typeof t?r=t:i(this.options,t),r&&this.on("always",r),this.getImages(),h&&(this.jqDeferred=new h.Deferred),void setTimeout(function(){this.check()}.bind(this))):new o(e,t,r)}function r(e){this.img=e}function s(e,t){this.url=e,this.element=t,this.img=new Image}var h=e.jQuery,a=e.console;o.prototype=Object.create(t.prototype),o.prototype.options={},o.prototype.getImages=function(){this.images=[],this.elements.forEach(this.addElementImages,this)},o.prototype.addElementImages=function(e){"IMG"==e.nodeName&&this.addImage(e),this.options.background===!0&&this.addElementBackgroundImages(e);var t=e.nodeType;if(t&&d[t]){for(var i=e.querySelectorAll("img"),n=0;n<i.length;n++){var o=i[n];this.addImage(o)}if("string"==typeof this.options.background){var r=e.querySelectorAll(this.options.background);for(n=0;n<r.length;n++){var s=r[n];this.addElementBackgroundImages(s)}}}};var d={1:!0,9:!0,11:!0};return o.prototype.addElementBackgroundImages=function(e){var t=getComputedStyle(e);if(t)for(var i=/url\((['"])?(.*?)\1\)/gi,n=i.exec(t.backgroundImage);null!==n;){var o=n&&n[2];o&&this.addBackground(o,e),n=i.exec(t.backgroundImage)}},o.prototype.addImage=function(e){var t=new r(e);this.images.push(t)},o.prototype.addBackground=function(e,t){var i=new s(e,t);this.images.push(i)},o.prototype.check=function(){function e(e,i,n){setTimeout(function(){t.progress(e,i,n)})}var t=this;return this.progressedCount=0,this.hasAnyBroken=!1,this.images.length?void this.images.forEach(function(t){t.once("progress",e),t.check()}):void this.complete()},o.prototype.progress=function(e,t,i){this.progressedCount++,this.hasAnyBroken=this.hasAnyBroken||!e.isLoaded,this.emitEvent("progress",[this,e,t]),this.jqDeferred&&this.jqDeferred.notify&&this.jqDeferred.notify(this,e),this.progressedCount==this.images.length&&this.complete(),this.options.debug&&a&&a.log("progress: "+i,e,t)},o.prototype.complete=function(){var e=this.hasAnyBroken?"fail":"done";if(this.isComplete=!0,this.emitEvent(e,[this]),this.emitEvent("always",[this]),this.jqDeferred){var t=this.hasAnyBroken?"reject":"resolve";this.jqDeferred[t](this)}},r.prototype=Object.create(t.prototype),r.prototype.check=function(){var e=this.getIsImageComplete();return e?void this.confirm(0!==this.img.naturalWidth,"naturalWidth"):(this.proxyImage=new Image,this.proxyImage.addEventListener("load",this),this.proxyImage.addEventListener("error",this),this.img.addEventListener("load",this),this.img.addEventListener("error",this),void(this.proxyImage.src=this.img.src))},r.prototype.getIsImageComplete=function(){return this.img.complete&&void 0!==this.img.naturalWidth},r.prototype.confirm=function(e,t){this.isLoaded=e,this.emitEvent("progress",[this,this.img,t])},r.prototype.handleEvent=function(e){var t="on"+e.type;this[t]&&this[t](e)},r.prototype.onload=function(){this.confirm(!0,"onload"),this.unbindEvents()},r.prototype.onerror=function(){this.confirm(!1,"onerror"),this.unbindEvents()},r.prototype.unbindEvents=function(){this.proxyImage.removeEventListener("load",this),this.proxyImage.removeEventListener("error",this),this.img.removeEventListener("load",this),this.img.removeEventListener("error",this)},s.prototype=Object.create(r.prototype),s.prototype.check=function(){this.img.addEventListener("load",this),this.img.addEventListener("error",this),this.img.src=this.url;var e=this.getIsImageComplete();e&&(this.confirm(0!==this.img.naturalWidth,"naturalWidth"),this.unbindEvents())},s.prototype.unbindEvents=function(){this.img.removeEventListener("load",this),this.img.removeEventListener("error",this)},s.prototype.confirm=function(e,t){this.isLoaded=e,this.emitEvent("progress",[this,this.element,t])},o.makeJQueryPlugin=function(t){t=t||e.jQuery,t&&(h=t,h.fn.imagesLoaded=function(e,t){var i=new o(this,e,t);return i.jqDeferred.promise(h(this))})},o.makeJQueryPlugin(),o});
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          /*!
 * Packery PACKAGED v2.1.1
 * Gapless, draggable grid layouts
 *
 * Licensed GPLv3 for open source use
 * or Packery Commercial License for commercial use
 *
 * http://packery.metafizzy.co
 * Copyright 2016 Metafizzy
 */
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          /*  NOTE : THIS IS MODIFIED VERSION OF PACKERY TO HANDLE THE VARIOUS ANIMATIONS AND REVEALING ITEMS IS REMOVED */
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          !function(t,e){"use strict";"function"==typeof define&&define.amd?define("jquery-bridget/jquery-bridget",["jquery"],function(i){e(t,i)}):"object"==typeof module&&module.exports?module.exports=e(t,require("jquery")):t.jQueryBridget=e(t,t.jQuery)}(window,function(t,e){"use strict";function i(i,s,a){function h(t,e,n){var o,s="$()."+i+'("'+e+'")';return t.each(function(t,h){var u=a.data(h,i);if(u){var c=u[e];if(c&&"_"!=e.charAt(0)){var d=c.apply(u,n);o=void 0===o?d:o}else r(s+" is not a valid method")}else r(i+" not initialized. Cannot call methods, i.e. "+s)}),void 0!==o?o:t}function u(t,e){t.each(function(t,n){var o=a.data(n,i);o?(o.option(e),o._init()):(o=new s(n,e),a.data(n,i,o))})}(a=a||e||t.jQuery)&&(s.prototype.option||(s.prototype.option=function(t){a.isPlainObject(t)&&(this.options=a.extend(!0,this.options,t))}),a.fn[i]=function(t){return"string"==typeof t?h(this,t,o.call(arguments,1)):(u(this,t),this)},n(a))}function n(t){!t||t&&t.bridget||(t.bridget=i)}var o=Array.prototype.slice,s=t.console,r=void 0===s?function(){}:function(t){s.error(t)};return n(e||t.jQuery),i}),function(t,e){"use strict";"function"==typeof define&&define.amd?define("get-size/get-size",[],function(){return e()}):"object"==typeof module&&module.exports?module.exports=e():t.getSize=e()}(window,function(){"use strict";function t(t){var e=parseFloat(t);return-1==t.indexOf("%")&&!isNaN(e)&&e}function e(){for(var t={width:0,height:0,innerWidth:0,innerHeight:0,outerWidth:0,outerHeight:0},e=0;e<h;e++)t[a[e]]=0;return t}function i(t){var e=getComputedStyle(t);return e||r("Style returned "+e+". Are you running this code in a hidden iframe on Firefox? See http://bit.ly/getsizebug1"),e}function n(){if(!u){u=!0;var e=document.createElement("div");e.style.width="200px",e.style.padding="1px 2px 3px 4px",e.style.borderStyle="solid",e.style.borderWidth="1px 2px 3px 4px",e.style.boxSizing="border-box";var n=document.body||document.documentElement;n.appendChild(e);var r=i(e);o.isBoxSizeOuter=s=200==t(r.width),n.removeChild(e)}}function o(o){if(n(),"string"==typeof o&&(o=document.querySelector(o)),o&&"object"==typeof o&&o.nodeType){var r=i(o);if("none"==r.display)return e();var u={};u.width=o.offsetWidth,u.height=o.offsetHeight;for(var c=u.isBorderBox="border-box"==r.boxSizing,d=0;d<h;d++){var l=a[d],f=r[l],p=parseFloat(f);u[l]=isNaN(p)?0:p}var g=u.paddingLeft+u.paddingRight,m=u.paddingTop+u.paddingBottom,y=u.marginLeft+u.marginRight,v=u.marginTop+u.marginBottom,x=u.borderLeftWidth+u.borderRightWidth,_=u.borderTopWidth+u.borderBottomWidth,b=c&&s,w=t(r.width);!1!==w&&(u.width=w+(b?0:g+x));var E=t(r.height);return!1!==E&&(u.height=E+(b?0:m+_)),u.innerWidth=u.width-(g+x),u.innerHeight=u.height-(m+_),u.outerWidth=u.width+y,u.outerHeight=u.height+v,u}}var s,r="undefined"==typeof console?function(){}:function(t){console.error(t)},a=["paddingLeft","paddingRight","paddingTop","paddingBottom","marginLeft","marginRight","marginTop","marginBottom","borderLeftWidth","borderRightWidth","borderTopWidth","borderBottomWidth"],h=a.length,u=!1;return o}),function(t,e){"function"==typeof define&&define.amd?define("ev-emitter/ev-emitter",e):"object"==typeof module&&module.exports?module.exports=e():t.EvEmitter=e()}(this,function(){function t(){}var e=t.prototype;return e.on=function(t,e){if(t&&e){var i=this._events=this._events||{},n=i[t]=i[t]||[];return-1==n.indexOf(e)&&n.push(e),this}},e.once=function(t,e){if(t&&e){this.on(t,e);var i=this._onceEvents=this._onceEvents||{};return(i[t]=i[t]||{})[e]=!0,this}},e.off=function(t,e){var i=this._events&&this._events[t];if(i&&i.length){var n=i.indexOf(e);return-1!=n&&i.splice(n,1),this}},e.emitEvent=function(t,e){var i=this._events&&this._events[t];if(i&&i.length){var n=0,o=i[n];e=e||[];for(var s=this._onceEvents&&this._onceEvents[t];o;){var r=s&&s[o];r&&(this.off(t,o),delete s[o]),o.apply(this,e),o=i[n+=r?0:1]}return this}},t}),function(t,e){"use strict";"function"==typeof define&&define.amd?define("desandro-matches-selector/matches-selector",e):"object"==typeof module&&module.exports?module.exports=e():t.matchesSelector=e()}(window,function(){"use strict";var t=function(){var t=Element.prototype;if(t.matches)return"matches";if(t.matchesSelector)return"matchesSelector";for(var e=["webkit","moz","ms","o"],i=0;i<e.length;i++){var n=e[i]+"MatchesSelector";if(t[n])return n}}();return function(e,i){return e[t](i)}}),function(t,e){"function"==typeof define&&define.amd?define("fizzy-ui-utils/utils",["desandro-matches-selector/matches-selector"],function(i){return e(t,i)}):"object"==typeof module&&module.exports?module.exports=e(t,require("desandro-matches-selector")):t.fizzyUIUtils=e(t,t.matchesSelector)}(window,function(t,e){var i={};i.extend=function(t,e){for(var i in e)t[i]=e[i];return t},i.modulo=function(t,e){return(t%e+e)%e},i.makeArray=function(t){var e=[];if(Array.isArray(t))e=t;else if(t&&"number"==typeof t.length)for(var i=0;i<t.length;i++)e.push(t[i]);else e.push(t);return e},i.removeFrom=function(t,e){var i=t.indexOf(e);-1!=i&&t.splice(i,1)},i.getParent=function(t,i){for(;t!=document.body;)if(t=t.parentNode,e(t,i))return t},i.getQueryElement=function(t){return"string"==typeof t?document.querySelector(t):t},i.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},i.filterFindElements=function(t,n){var o=[];return(t=i.makeArray(t)).forEach(function(t){if(t instanceof HTMLElement)if(n){e(t,n)&&o.push(t);for(var i=t.querySelectorAll(n),s=0;s<i.length;s++)o.push(i[s])}else o.push(t)}),o},i.debounceMethod=function(t,e,i){var n=t.prototype[e],o=e+"Timeout";t.prototype[e]=function(){var t=this[o];t&&clearTimeout(t);var e=arguments,s=this;this[o]=setTimeout(function(){n.apply(s,e),delete s[o]},i||100)}},i.docReady=function(t){"complete"==document.readyState?t():document.addEventListener("DOMContentLoaded",t)},i.toDashed=function(t){return t.replace(/(.)([A-Z])/g,function(t,e,i){return e+"-"+i}).toLowerCase()};var n=t.console;return i.htmlInit=function(e,o){i.docReady(function(){var s=i.toDashed(o),r="data-"+s,a=document.querySelectorAll("["+r+"]"),h=document.querySelectorAll(".js-"+s),u=i.makeArray(a).concat(i.makeArray(h)),c=r+"-options",d=t.jQuery;u.forEach(function(t){var i,s=t.getAttribute(r)||t.getAttribute(c);try{i=s&&JSON.parse(s)}catch(e){return void(n&&n.error("Error parsing "+r+" on "+t.className+": "+e))}var a=new e(t,i);d&&d.data(t,o,a)})})},i}),function(t,e){"function"==typeof define&&define.amd?define("outlayer/item",["ev-emitter/ev-emitter","get-size/get-size"],e):"object"==typeof module&&module.exports?module.exports=e(require("ev-emitter"),require("get-size")):(t.Outlayer={},t.Outlayer.Item=e(t.EvEmitter,t.getSize))}(window,function(t,e){"use strict";function i(t){for(var e in t)return!1;return null,!0}function n(t,e){t&&(this.element=t,this.layout=e,this.position={x:0,y:0},this._create())}function o(t,e,i,n){var o,s,r,a=!0;if(!i)var i=0;g(window).scroll(function(){a=!0}),setInterval(function(){a&&(a=!1,r=g(this).scrollTop(),g(t).each(function(i){o=g(this).offset().top-g(window).height()/2,s=g(this).height(),r>=o&&!g(this).hasClass(e)&&(g(this).hasClass("anim-done")||(g(this).hasClass("noapply"),g(this).addClass(e)),"function"==typeof n&&n(t))}))},100)}function s(){switch(loadinganimation){case"expand":anime({targets:".run-anim",duration:function(t,e){return 600+75*e},easing:"easeOutExpo",delay:function(t,e){return 50*e},opacity:{value:[0,1],easing:"linear"},scale:[0,1]});break;case"slideup":anime({targets:".run-anim",duration:function(t,e){return 500+50*e},easing:"easeOutExpo",delay:function(t,e){return 20*e},opacity:{value:[0,1],duration:function(t,e){return 250+50*e},easing:"linear"},translateY:[400,0]});break;case"slideright":anime({targets:".run-anim",duration:800,easing:[.1,1,.3,1],delay:function(t,e){return 20*e},opacity:{value:[0,1],duration:600,easing:"linear"},translateX:[-500,0],rotateZ:[15,0]});break;case"shaking":anime({targets:".run-anim",duration:900,elasticity:500,delay:function(t,e){return 15*e},opacity:{value:[0,1],duration:300,easing:"linear"},translateX:function(){return[0===anime.random(0,1)?100:-100,0]},translateY:function(){return[0===anime.random(0,1)?100:-100,0]}});break;case"flipdown":g(".grid-item").map(function(){g(this).css("perspective","800px").css("transform-origin","50% 0% 0px")}),anime({targets:".run-anim",duration:1500,elasticity:400,delay:function(t,e){return 75*e},opacity:{value:[0,1],duration:1e3,easing:"linear"},rotateX:[-90,0]});break;case"revolve":g(".grid-item").map(function(){g(this).css("perspective","3000")}),anime({targets:".run-anim",duration:function(){return anime.random(500,1e3)},easing:[.2,1,.3,1],delay:function(t,e){return 50*e},opacity:{value:[0,1],duration:700,easing:"linear"},translateZ:{value:[-3e3,0],duration:1e3},rotateY:["-1turns",0]});break;case"jelly":anime({targets:".run-anim",duration:800,elasticity:600,delay:function(t,e){return 100*e},opacity:{value:[0,1],duration:600,easing:"linear"},scaleX:{value:[.4,1]},scaleY:{value:[.6,1],duration:1e3}});break;case"dropin":g(".grid-item").map(function(){g(this).css("perspective","1000").css("origin","50% 0%")}),anime({targets:".run-anim",duration:800,easing:[.1,1,.3,1],delay:function(t,e){return 35*e},opacity:{value:[0,1],duration:600,easing:"linear"},translateX:[100,0],translateY:[-100,0],translateZ:[400,0],rotateZ:[10,0],rotateX:[75,0]});break;case"spring":g(".grid-item").map(function(){g(this).css("origin","50% 0%")}),anime({targets:".run-anim",duration:500,easing:"easeOutBack",delay:function(t,e){return 100*e},opacity:{value:[0,1],easing:"linear"},translateY:[400,0],scaleY:[{value:[3,.6],delay:function(t,e){return 100*e+120},duration:300,easing:"easeOutExpo"},{value:[.6,1],duration:1400,easing:"easeOutElastic"}],scaleX:[{value:[.9,1.05],delay:function(t,e){return 100*e+120},duration:300,easing:"easeOutExpo"},{value:[1.05,1],duration:1400,easing:"easeOutElastic"}]});break;case"spred":anime({targets:".run-anim",duration:600,easing:"easeOutExpo",delay:function(t,e){return 100*e},opacity:{value:[0,1],duration:100,easing:"linear"},translateX:function(t,e){var i={left:document.body.scrollLeft+document.documentElement.scrollLeft},n=window.innerWidth/2+i.left,o=t.getBoundingClientRect();return[n-(o.left+i.left+o.width/2),0]},translateY:function(t,e){var i={top:document.body.scrollTop+document.documentElement.scrollTop},n=window.innerHeight+i.top,o=t.getBoundingClientRect();return[n-(o.top+i.top+o.height/2),0]},rotate:function(t,e){var i=window.innerWidth/2,n=t.getBoundingClientRect();return[n.left+n.width/2<i?90:-90,0]},scale:[0,1]});break;default:anime({targets:".run-anim",duration:600,easing:"easeOutExpo",delay:function(t,e){return 100*e},opacity:{value:[0,1],duration:100,easing:"linear"},translateX:function(t,e){var i={left:document.body.scrollLeft+document.documentElement.scrollLeft},n=window.innerWidth/2+i.left,o=t.getBoundingClientRect();return[n-(o.left+i.left+o.width/2),0]},translateY:function(t,e){var i={top:document.body.scrollTop+document.documentElement.scrollTop},n=window.innerHeight+i.top,o=t.getBoundingClientRect();return[n-(o.top+i.top+o.height/2),0]},rotate:function(t,e){var i=window.innerWidth/2,n=t.getBoundingClientRect();return[n.left+n.width/2<i?90:-90,0]},scale:[0,1]})}g(".run-anim").addClass("anim-done").removeClass("run-anim").removeClass("noapply")}var r=document.documentElement.style,a="string"==typeof r.transition?"transition":"WebkitTransition",h="string"==typeof r.transform?"transform":"WebkitTransform",u={WebkitTransition:"webkitTransitionEnd",transition:"transitionend"}[a],c={transform:h,transition:a,transitionDuration:a+"Duration",transitionProperty:a+"Property",transitionDelay:a+"Delay"},d=n.prototype=Object.create(t.prototype);d.constructor=n,d._create=function(){this._transn={ingProperties:{},clean:{},onEnd:{}},this.css({position:"absolute"})},d.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},d.getSize=function(){this.size=e(this.element)},d.css=function(t){var e=this.element.style;for(var i in t)e[c[i]||i]=t[i]},d.getPosition=function(){var t=getComputedStyle(this.element),e=this.layout._getOption("originLeft"),i=this.layout._getOption("originTop"),n=t[e?"left":"right"],o=t[i?"top":"bottom"],s=this.layout.size,r=-1!=n.indexOf("%")?parseFloat(n)/100*s.width:parseInt(n,10),a=-1!=o.indexOf("%")?parseFloat(o)/100*s.height:parseInt(o,10);r=isNaN(r)?0:r,a=isNaN(a)?0:a,r-=e?s.paddingLeft:s.paddingRight,a-=i?s.paddingTop:s.paddingBottom,this.position.x=r,this.position.y=a},d.layoutPosition=function(){var t=this.layout.size,e={},i=this.layout._getOption("originLeft"),n=this.layout._getOption("originTop"),o=i?"paddingLeft":"paddingRight",s=i?"left":"right",r=i?"right":"left",a=this.position.x+t[o];e[s]=this.getXValue(a),e[r]="";var h=n?"paddingTop":"paddingBottom",u=n?"top":"bottom",c=n?"bottom":"top",d=this.position.y+t[h];e[u]=this.getYValue(d),e[c]="",this.css(e),this.emitEvent("layout",[this])},d.getXValue=function(t){var e=this.layout._getOption("horizontal");return this.layout.options.percentPosition&&!e?t/this.layout.size.width*100+"%":t+"px"},d.getYValue=function(t){var e=this.layout._getOption("horizontal");return this.layout.options.percentPosition&&e?t/this.layout.size.height*100+"%":t+"px"},d._transitionTo=function(t,e){this.getPosition();var i=this.position.x,n=this.position.y,o=parseInt(t,10),s=parseInt(e,10),r=o===this.position.x&&s===this.position.y;if(this.setPosition(t,e),!r||this.isTransitioning){var a=t-i,h=e-n,u={};u.transform=this.getTranslate(a,h),this.transition({to:u,onTransitionEnd:{transform:this.layoutPosition},isCleaning:!0})}else this.layoutPosition()},d.getTranslate=function(t,e){var i=this.layout._getOption("originLeft"),n=this.layout._getOption("originTop");return t=i?t:-t,e=n?e:-e,"translate3d("+t+"px, "+e+"px, 0)"},d.goTo=function(t,e){this.setPosition(t,e),this.layoutPosition()},d.moveTo=d._transitionTo,d.setPosition=function(t,e){this.position.x=parseInt(t,10),this.position.y=parseInt(e,10)},d._nonTransition=function(t){this.css(t.to),t.isCleaning&&this._removeStyles(t.to);for(var e in t.onTransitionEnd)t.onTransitionEnd[e].call(this)},d.transition=function(t){if(parseFloat(this.layout.options.transitionDuration)){var e=this._transn;for(var i in t.onTransitionEnd)e.onEnd[i]=t.onTransitionEnd[i];for(i in t.to)e.ingProperties[i]=!0,t.isCleaning&&(e.clean[i]=!0);if(t.from){this.css(t.from);this.element.offsetHeight;null}this.enableTransition(t.to),this.css(t.to),this.isTransitioning=!0}else this._nonTransition(t)};var l="opacity,"+h.replace(/([A-Z])/g,function(t){return"-"+t.toLowerCase()});d.enableTransition=function(){if(!this.isTransitioning){var t=this.layout.options.transitionDuration;t="number"==typeof t?t+"ms":t,this.css({transitionProperty:l,transitionDuration:t,transitionDelay:this.staggerDelay||0}),this.element.addEventListener(u,this,!1)}},d.onwebkitTransitionEnd=function(t){this.ontransitionend(t)},d.onotransitionend=function(t){this.ontransitionend(t)};var f={"-webkit-transform":"transform"};d.ontransitionend=function(t){if(t.target===this.element){var e=this._transn,n=f[t.propertyName]||t.propertyName;delete e.ingProperties[n],i(e.ingProperties)&&this.disableTransition(),n in e.clean&&(this.element.style[t.propertyName]="",delete e.clean[n]),n in e.onEnd&&(e.onEnd[n].call(this),delete e.onEnd[n]),this.emitEvent("transitionEnd",[this])}},d.disableTransition=function(){this.removeTransitionStyles(),this.element.removeEventListener(u,this,!1),this.isTransitioning=!1},d._removeStyles=function(t){var e={};for(var i in t)e[i]="";this.css(e)};var p={transitionProperty:"",transitionDuration:"",transitionDelay:""};d.removeTransitionStyles=function(){this.css(p)},d.stagger=function(t){t=isNaN(t)?0:t,this.staggerDelay=t+"ms"},d.removeElem=function(){this.element.parentNode.removeChild(this.element),this.css({display:""}),this.emitEvent("remove",[this])},d.remove=function(){a&&parseFloat(this.layout.options.transitionDuration)?(this.once("transitionEnd",function(){this.removeElem()}),this.hide()):this.removeElem()};var g=jQuery;return d.reveal=function(){delete this.isHidden,this.css({display:""});this.layout.options;o(".grid-item","run-anim",300,function(){s()})},d.onRevealTransitionEnd=function(){this.isHidden||this.emitEvent("reveal")},d.getHideRevealTransitionEndProperty=function(t){var e=this.layout.options[t];if(e.opacity)return"opacity";for(var i in e)return i},d.hide=function(){this.isHidden=!0,this.css({display:""});var t=this.layout.options,e={};e[this.getHideRevealTransitionEndProperty("hiddenStyle")]=this.onHideTransitionEnd,this.transition({from:t.visibleStyle,to:t.hiddenStyle,isCleaning:!0,onTransitionEnd:e})},d.onHideTransitionEnd=function(){this.isHidden&&(this.css({display:"none"}),this.emitEvent("hide"))},d.destroy=function(){this.css({position:"",left:"",right:"",top:"",bottom:"",transition:"",transform:""})},n}),function(t,e){"use strict";"function"==typeof define&&define.amd?define("outlayer/outlayer",["ev-emitter/ev-emitter","get-size/get-size","fizzy-ui-utils/utils","./item"],function(i,n,o,s){return e(t,i,n,o,s)}):"object"==typeof module&&module.exports?module.exports=e(t,require("ev-emitter"),require("get-size"),require("fizzy-ui-utils"),require("./item")):t.Outlayer=e(t,t.EvEmitter,t.getSize,t.fizzyUIUtils,t.Outlayer.Item)}(window,function(t,e,i,n,o){"use strict";function s(t,e){var i=n.getQueryElement(t);if(i){this.element=i,u&&(this.$element=u(this.element)),this.options=n.extend({},this.constructor.defaults),this.option(e);var o=++d;this.element.outlayerGUID=o,l[o]=this,this._create(),this._getOption("initLayout")&&this.layout()}else h&&h.error("Bad element for "+this.constructor.namespace+": "+(i||t))}function r(t){function e(){t.apply(this,arguments)}return e.prototype=Object.create(t.prototype),e.prototype.constructor=e,e}function a(t){if("number"==typeof t)return t;var e=t.match(/(^\d*\.?\d*)(\w*)/),i=e&&e[1],n=e&&e[2];return i.length?(i=parseFloat(i))*(p[n]||1):0}var h=t.console,u=t.jQuery,c=function(){},d=0,l={};s.namespace="outlayer",s.Item=o,s.defaults={containerStyle:{position:"relative"},initLayout:!0,originLeft:!0,originTop:!0,resize:!0,resizeContainer:!0,transitionDuration:"0.4s",hiddenStyle:{opacity:0,transform:"scale(0.001)"},visibleStyle:{opacity:1,transform:"scale(1)"}};var f=s.prototype;n.extend(f,e.prototype),f.option=function(t){n.extend(this.options,t)},f._getOption=function(t){var e=this.constructor.compatOptions[t];return e&&void 0!==this.options[e]?this.options[e]:this.options[t]},s.compatOptions={initLayout:"isInitLayout",horizontal:"isHorizontal",layoutInstant:"isLayoutInstant",originLeft:"isOriginLeft",originTop:"isOriginTop",resize:"isResizeBound",resizeContainer:"isResizingContainer"},f._create=function(){this.reloadItems(),this.stamps=[],this.stamp(this.options.stamp),n.extend(this.element.style,this.options.containerStyle),this._getOption("resize")&&this.bindResize()},f.reloadItems=function(){this.items=this._itemize(this.element.children)},f._itemize=function(t){for(var e=this._filterFindItemElements(t),i=this.constructor.Item,n=[],o=0;o<e.length;o++){var s=new i(e[o],this);n.push(s)}return n},f._filterFindItemElements=function(t){return n.filterFindElements(t,this.options.itemSelector)},f.getItemElements=function(){return this.items.map(function(t){return t.element})},f.layout=function(){this._resetLayout(),this._manageStamps();var t=this._getOption("layoutInstant"),e=void 0!==t?t:!this._isLayoutInited;this.layoutItems(this.items,e),this._isLayoutInited=!0},f._init=f.layout,f._resetLayout=function(){this.getSize()},f.getSize=function(){this.size=i(this.element)},f._getMeasurement=function(t,e){var n,o=this.options[t];o?("string"==typeof o?n=this.element.querySelector(o):o instanceof HTMLElement&&(n=o),this[t]=n?i(n)[e]:o):this[t]=0},f.layoutItems=function(t,e){t=this._getItemsForLayout(t),this._layoutItems(t,e),this._postLayout()},f._getItemsForLayout=function(t){return t.filter(function(t){return!t.isIgnored})},f._layoutItems=function(t,e){if(this._emitCompleteOnItems("layout",t),t&&t.length){var i=[];t.forEach(function(t){var n=this._getItemLayoutPosition(t);n.item=t,n.isInstant=e||t.isLayoutInstant,i.push(n)},this),this._processLayoutQueue(i)}},f._getItemLayoutPosition=function(){return{x:0,y:0}},f._processLayoutQueue=function(t){this.updateStagger(),t.forEach(function(t,e){this._positionItem(t.item,t.x,t.y,t.isInstant,e)},this)},f.updateStagger=function(){var t=this.options.stagger;{if(null!==t&&void 0!==t)return this.stagger=a(t),this.stagger;this.stagger=0}},f._positionItem=function(t,e,i,n,o){n?t.goTo(e,i):(t.stagger(o*this.stagger),t.moveTo(e,i))},f._postLayout=function(){this.resizeContainer()},f.resizeContainer=function(){if(this._getOption("resizeContainer")){var t=this._getContainerSize();t&&(this._setContainerMeasure(t.width,!0),this._setContainerMeasure(t.height,!1))}},f._getContainerSize=c,f._setContainerMeasure=function(t,e){if(void 0!==t){var i=this.size;i.isBorderBox&&(t+=e?i.paddingLeft+i.paddingRight+i.borderLeftWidth+i.borderRightWidth:i.paddingBottom+i.paddingTop+i.borderTopWidth+i.borderBottomWidth),t=Math.max(t,0),this.element.style[e?"width":"height"]=t+"px"}},f._emitCompleteOnItems=function(t,e){function i(){o.dispatchEvent(t+"Complete",null,[e])}function n(){++r==s&&i()}var o=this,s=e.length;if(e&&s){var r=0;e.forEach(function(e){e.once(t,n)})}else i()},f.dispatchEvent=function(t,e,i){var n=e?[e].concat(i):i;if(this.emitEvent(t,n),u)if(this.$element=this.$element||u(this.element),e){var o=u.Event(e);o.type=t,this.$element.trigger(o,i)}else this.$element.trigger(t,i)},f.ignore=function(t){var e=this.getItem(t);e&&(e.isIgnored=!0)},f.unignore=function(t){var e=this.getItem(t);e&&delete e.isIgnored},f.stamp=function(t){(t=this._find(t))&&(this.stamps=this.stamps.concat(t),t.forEach(this.ignore,this))},f.unstamp=function(t){(t=this._find(t))&&t.forEach(function(t){n.removeFrom(this.stamps,t),this.unignore(t)},this)},f._find=function(t){if(t)return"string"==typeof t&&(t=this.element.querySelectorAll(t)),t=n.makeArray(t)},f._manageStamps=function(){this.stamps&&this.stamps.length&&(this._getBoundingRect(),this.stamps.forEach(this._manageStamp,this))},f._getBoundingRect=function(){var t=this.element.getBoundingClientRect(),e=this.size;this._boundingRect={left:t.left+e.paddingLeft+e.borderLeftWidth,top:t.top+e.paddingTop+e.borderTopWidth,right:t.right-(e.paddingRight+e.borderRightWidth),bottom:t.bottom-(e.paddingBottom+e.borderBottomWidth)}},f._manageStamp=c,f._getElementOffset=function(t){var e=t.getBoundingClientRect(),n=this._boundingRect,o=i(t);return{left:e.left-n.left-o.marginLeft,top:e.top-n.top-o.marginTop,right:n.right-e.right-o.marginRight,bottom:n.bottom-e.bottom-o.marginBottom}},f.handleEvent=n.handleEvent,f.bindResize=function(){t.addEventListener("resize",this),this.isResizeBound=!0},f.unbindResize=function(){t.removeEventListener("resize",this),this.isResizeBound=!1},f.onresize=function(){this.resize()},n.debounceMethod(s,"onresize",100),f.resize=function(){this.isResizeBound&&this.needsResizeLayout()&&this.layout()},f.needsResizeLayout=function(){var t=i(this.element);return this.size&&t&&t.innerWidth!==this.size.innerWidth},f.addItems=function(t){var e=this._itemize(t);return e.length&&(this.items=this.items.concat(e)),e},f.appended=function(t){var e=this.addItems(t);e.length&&(this.layoutItems(e,!0),this.reveal(e))},f.prepended=function(t){var e=this._itemize(t);if(e.length){var i=this.items.slice(0);this.items=e.concat(i),this._resetLayout(),this._manageStamps(),this.layoutItems(e,!0),this.reveal(e),this.layoutItems(i)}},f.reveal=function(t){if(this._emitCompleteOnItems("reveal",t),t&&t.length){var e=this.updateStagger();t.forEach(function(t,i){t.stagger(i*e),t.reveal()})}},f.hide=function(t){if(this._emitCompleteOnItems("hide",t),t&&t.length){var e=this.updateStagger();t.forEach(function(t,i){t.stagger(i*e),t.hide()})}},f.revealItemElements=function(t){var e=this.getItems(t);this.reveal(e)},f.hideItemElements=function(t){var e=this.getItems(t);this.hide(e)},f.getItem=function(t){for(var e=0;e<this.items.length;e++){var i=this.items[e];if(i.element==t)return i}},f.getItems=function(t){var e=[];return(t=n.makeArray(t)).forEach(function(t){var i=this.getItem(t);i&&e.push(i)},this),e},f.remove=function(t){var e=this.getItems(t);this._emitCompleteOnItems("remove",e),e&&e.length&&e.forEach(function(t){t.remove(),n.removeFrom(this.items,t)},this)},f.destroy=function(){var t=this.element.style;t.height="",t.position="",t.width="",this.items.forEach(function(t){t.destroy()}),this.unbindResize();var e=this.element.outlayerGUID;delete l[e],delete this.element.outlayerGUID,u&&u.removeData(this.element,this.constructor.namespace)},s.data=function(t){var e=(t=n.getQueryElement(t))&&t.outlayerGUID;return e&&l[e]},s.create=function(t,e){var i=r(s);return i.defaults=n.extend({},s.defaults),n.extend(i.defaults,e),i.compatOptions=n.extend({},s.compatOptions),i.namespace=t,i.data=s.data,i.Item=r(o),n.htmlInit(i,t),u&&u.bridget&&u.bridget(t,i),i};var p={ms:1,s:1e3};return s.Item=o,s}),function(t,e){"function"==typeof define&&define.amd?define("packery/js/rect",e):"object"==typeof module&&module.exports?module.exports=e():(t.Packery=t.Packery||{},t.Packery.Rect=e())}(window,function(){"use strict";function t(e){for(var i in t.defaults)this[i]=t.defaults[i];for(i in e)this[i]=e[i]}t.defaults={x:0,y:0,width:0,height:0};var e=t.prototype;return e.contains=function(t){var e=t.width||0,i=t.height||0;return this.x<=t.x&&this.y<=t.y&&this.x+this.width>=t.x+e&&this.y+this.height>=t.y+i},e.overlaps=function(t){var e=this.x+this.width,i=this.y+this.height,n=t.x+t.width,o=t.y+t.height;return this.x<n&&e>t.x&&this.y<o&&i>t.y},e.getMaximalFreeRects=function(e){if(!this.overlaps(e))return!1;var i,n=[],o=this.x+this.width,s=this.y+this.height,r=e.x+e.width,a=e.y+e.height;return this.y<e.y&&(i=new t({x:this.x,y:this.y,width:this.width,height:e.y-this.y}),n.push(i)),o>r&&(i=new t({x:r,y:this.y,width:o-r,height:this.height}),n.push(i)),s>a&&(i=new t({x:this.x,y:a,width:this.width,height:s-a}),n.push(i)),this.x<e.x&&(i=new t({x:this.x,y:this.y,width:e.x-this.x,height:this.height}),n.push(i)),n},e.canFit=function(t){return this.width>=t.width&&this.height>=t.height},t}),function(t,e){if("function"==typeof define&&define.amd)define("packery/js/packer",["./rect"],e);else if("object"==typeof module&&module.exports)module.exports=e(require("./rect"));else{var i=t.Packery=t.Packery||{};i.Packer=e(i.Rect)}}(window,function(t){"use strict";function e(t,e,i){this.width=t||0,this.height=e||0,this.sortDirection=i||"downwardLeftToRight",this.reset()}var i=e.prototype;i.reset=function(){this.spaces=[];var e=new t({x:0,y:0,width:this.width,height:this.height});this.spaces.push(e),this.sorter=n[this.sortDirection]||n.downwardLeftToRight},i.pack=function(t){for(var e=0;e<this.spaces.length;e++){var i=this.spaces[e];if(i.canFit(t)){this.placeInSpace(t,i);break}}},i.columnPack=function(t){for(var e=0;e<this.spaces.length;e++){var i=this.spaces[e];if(i.x<=t.x&&i.x+i.width>=t.x+t.width&&i.height>=t.height-.01){t.y=i.y,this.placed(t);break}}},i.rowPack=function(t){for(var e=0;e<this.spaces.length;e++){var i=this.spaces[e];if(i.y<=t.y&&i.y+i.height>=t.y+t.height&&i.width>=t.width-.01){t.x=i.x,this.placed(t);break}}},i.placeInSpace=function(t,e){t.x=e.x,t.y=e.y,this.placed(t)},i.placed=function(t){for(var e=[],i=0;i<this.spaces.length;i++){var n=this.spaces[i],o=n.getMaximalFreeRects(t);o?e.push.apply(e,o):e.push(n)}this.spaces=e,this.mergeSortSpaces()},i.mergeSortSpaces=function(){e.mergeRects(this.spaces),this.spaces.sort(this.sorter)},i.addSpace=function(t){this.spaces.push(t),this.mergeSortSpaces()},e.mergeRects=function(t){var e=0,i=t[e];t:for(;i;){for(var n=0,o=t[e+n];o;){if(o==i)n++;else{if(o.contains(i)){t.splice(e,1),i=t[e];continue t}i.contains(o)?t.splice(e+n,1):n++}o=t[e+n]}i=t[++e]}return t};var n={downwardLeftToRight:function(t,e){return t.y-e.y||t.x-e.x},rightwardTopToBottom:function(t,e){return t.x-e.x||t.y-e.y}};return e}),function(t,e){"function"==typeof define&&define.amd?define("packery/js/item",["outlayer/outlayer","./rect"],e):"object"==typeof module&&module.exports?module.exports=e(require("outlayer"),require("./rect")):t.Packery.Item=e(t.Outlayer,t.Packery.Rect)}(window,function(t,e){"use strict";var i="string"==typeof document.documentElement.style.transform?"transform":"WebkitTransform",n=function(){t.Item.apply(this,arguments)},o=n.prototype=Object.create(t.Item.prototype),s=o._create;o._create=function(){s.call(this),this.rect=new e};var r=o.moveTo;return o.moveTo=function(t,e){var i=Math.abs(this.position.x-t),n=Math.abs(this.position.y-e);this.layout.dragItemCount&&!this.isPlacing&&!this.isTransitioning&&i<1&&n<1?this.goTo(t,e):r.apply(this,arguments)},o.enablePlacing=function(){this.removeTransitionStyles(),this.isTransitioning&&i&&(this.element.style[i]="none"),this.isTransitioning=!1,this.getSize(),this.layout._setRectSize(this.element,this.rect),this.isPlacing=!0},o.disablePlacing=function(){this.isPlacing=!1},o.removeElem=function(){this.element.parentNode.removeChild(this.element),this.layout.packer.addSpace(this.rect),this.emitEvent("remove",[this])},o.showDropPlaceholder=function(){var t=this.dropPlaceholder;t||((t=this.dropPlaceholder=document.createElement("div")).className="packery-drop-placeholder",t.style.position="absolute"),t.style.width=this.size.width+"px",t.style.height=this.size.height+"px",this.positionDropPlaceholder(),this.layout.element.appendChild(t)},o.positionDropPlaceholder=function(){this.dropPlaceholder.style[i]="translate("+this.rect.x+"px, "+this.rect.y+"px)"},o.hideDropPlaceholder=function(){var t=this.dropPlaceholder.parentNode;t&&t.removeChild(this.dropPlaceholder)},n}),function(t,e){"function"==typeof define&&define.amd?define(["get-size/get-size","outlayer/outlayer","packery/js/rect","packery/js/packer","packery/js/item"],e):"object"==typeof module&&module.exports?module.exports=e(require("get-size"),require("outlayer"),require("./rect"),require("./packer"),require("./item")):t.Packery=e(t.getSize,t.Outlayer,t.Packery.Rect,t.Packery.Packer,t.Packery.Item)}(window,function(t,e,i,n,o){"use strict";function s(t,e){return t.position.y-e.position.y||t.position.x-e.position.x}function r(t,e){return t.position.x-e.position.x||t.position.y-e.position.y}function a(t,e){var i=e.x-t.x,n=e.y-t.y;return Math.sqrt(i*i+n*n)}i.prototype.canFit=function(t){return this.width>=t.width-1&&this.height>=t.height-1};var h=e.create("packery");h.Item=o;var u=h.prototype;u._create=function(){e.prototype._create.call(this),this.packer=new n,this.shiftPacker=new n,this.isEnabled=!0,this.dragItemCount=0;var t=this;this.handleDraggabilly={dragStart:function(){t.itemDragStart(this.element)},dragMove:function(){t.itemDragMove(this.element,this.position.x,this.position.y)},dragEnd:function(){t.itemDragEnd(this.element)}},this.handleUIDraggable={start:function(e,i){i&&t.itemDragStart(e.currentTarget)},drag:function(e,i){i&&t.itemDragMove(e.currentTarget,i.position.left,i.position.top)},stop:function(e,i){i&&t.itemDragEnd(e.currentTarget)}}},u._resetLayout=function(){this.getSize(),this._getMeasurements();var t,e,i;this._getOption("horizontal")?(t=1/0,e=this.size.innerHeight+this.gutter,i="rightwardTopToBottom"):(t=this.size.innerWidth+this.gutter,e=1/0,i="downwardLeftToRight"),this.packer.width=this.shiftPacker.width=t,this.packer.height=this.shiftPacker.height=e,this.packer.sortDirection=this.shiftPacker.sortDirection=i,this.packer.reset(),this.maxY=0,this.maxX=0},u._getMeasurements=function(){this._getMeasurement("columnWidth","width"),this._getMeasurement("rowHeight","height"),this._getMeasurement("gutter","width")},u._getItemLayoutPosition=function(t){if(this._setRectSize(t.element,t.rect),this.isShifting||this.dragItemCount>0){var e=this._getPackMethod();this.packer[e](t.rect)}else this.packer.pack(t.rect);return this._setMaxXY(t.rect),t.rect},u.shiftLayout=function(){this.isShifting=!0,this.layout(),delete this.isShifting},u._getPackMethod=function(){return this._getOption("horizontal")?"rowPack":"columnPack"},u._setMaxXY=function(t){this.maxX=Math.max(t.x+t.width,this.maxX),this.maxY=Math.max(t.y+t.height,this.maxY)},u._setRectSize=function(e,i){var n=t(e),o=n.outerWidth,s=n.outerHeight;(o||s)&&(o=this._applyGridGutter(o,this.columnWidth),s=this._applyGridGutter(s,this.rowHeight)),i.width=Math.min(o,this.packer.width),i.height=Math.min(s,this.packer.height)},u._applyGridGutter=function(t,e){if(!e)return t+this.gutter;var i=t%(e+=this.gutter),n=i&&i<1?"round":"ceil";return t=Math[n](t/e)*e},u._getContainerSize=function(){return this._getOption("horizontal")?{width:this.maxX-this.gutter}:{height:this.maxY-this.gutter}},u._manageStamp=function(t){var e,n=this.getItem(t);if(n&&n.isPlacing)e=n.rect;else{var o=this._getElementOffset(t);e=new i({x:this._getOption("originLeft")?o.left:o.right,y:this._getOption("originTop")?o.top:o.bottom})}this._setRectSize(t,e),this.packer.placed(e),this._setMaxXY(e)},u.sortItemsByPosition=function(){var t=this._getOption("horizontal")?r:s;this.items.sort(t)},u.fit=function(t,e,i){var n=this.getItem(t);n&&(this.stamp(n.element),n.enablePlacing(),this.updateShiftTargets(n),e=void 0===e?n.rect.x:e,i=void 0===i?n.rect.y:i,this.shift(n,e,i),this._bindFitEvents(n),n.moveTo(n.rect.x,n.rect.y),this.shiftLayout(),this.unstamp(n.element),this.sortItemsByPosition(),n.disablePlacing())},u._bindFitEvents=function(t){function e(){2==++n&&i.dispatchEvent("fitComplete",null,[t])}var i=this,n=0;t.once("layout",e),this.once("layoutComplete",e)},u.resize=function(){this.isResizeBound&&this.needsResizeLayout()&&(this.options.shiftPercentResize?this.resizeShiftPercentLayout():this.layout())},u.needsResizeLayout=function(){var e=t(this.element),i=this._getOption("horizontal")?"innerHeight":"innerWidth";return e[i]!=this.size[i]},u.resizeShiftPercentLayout=function(){var e=this._getItemsForLayout(this.items),i=this._getOption("horizontal"),n=i?"y":"x",o=i?"height":"width",s=i?"rowHeight":"columnWidth",r=i?"innerHeight":"innerWidth",a=this[s];if(a=a&&a+this.gutter){this._getMeasurements();var h=this[s]+this.gutter;e.forEach(function(t){var e=Math.round(t.rect[n]/a);t.rect[n]=e*h})}else{var u=t(this.element)[r]+this.gutter,c=this.packer[o];e.forEach(function(t){t.rect[n]=t.rect[n]/c*u})}this.shiftLayout()},u.itemDragStart=function(t){if(this.isEnabled){this.stamp(t);var e=this.getItem(t);e&&(e.enablePlacing(),e.showDropPlaceholder(),this.dragItemCount++,this.updateShiftTargets(e))}},u.updateShiftTargets=function(t){this.shiftPacker.reset(),this._getBoundingRect();var e=this._getOption("originLeft"),n=this._getOption("originTop");this.stamps.forEach(function(t){var o=this.getItem(t);if(!o||!o.isPlacing){var s=this._getElementOffset(t),r=new i({x:e?s.left:s.right,y:n?s.top:s.bottom});this._setRectSize(t,r),this.shiftPacker.placed(r)}},this);var o=this._getOption("horizontal"),s=o?"rowHeight":"columnWidth",r=o?"height":"width";this.shiftTargetKeys=[],this.shiftTargets=[];var a,h=this[s];if(h=h&&h+this.gutter){var u=Math.ceil(t.rect[r]/h),c=Math.floor((this.shiftPacker[r]+this.gutter)/h);a=(c-u)*h;for(var d=0;d<c;d++){var l=o?0:d*h,f=o?d*h:0;this._addShiftTarget(l,f,a)}}else a=this.shiftPacker[r]+this.gutter-t.rect[r],this._addShiftTarget(0,0,a);var p=this._getItemsForLayout(this.items),g=this._getPackMethod();p.forEach(function(t){var e=t.rect;this._setRectSize(t.element,e),this.shiftPacker[g](e),this._addShiftTarget(e.x,e.y,a);var i=o?e.x+e.width:e.x,n=o?e.y:e.y+e.height;if(this._addShiftTarget(i,n,a),h)for(var s=Math.round(e[r]/h),u=1;u<s;u++){var c=o?i:e.x+h*u,d=o?e.y+h*u:n;this._addShiftTarget(c,d,a)}},this)},u._addShiftTarget=function(t,e,i){var n=this._getOption("horizontal")?e:t;if(!(0!==n&&n>i)){var o=t+","+e;-1!=this.shiftTargetKeys.indexOf(o)||(this.shiftTargetKeys.push(o),this.shiftTargets.push({x:t,y:e}))}},u.shift=function(t,e,i){var n,o=1/0,s={x:e,y:i};this.shiftTargets.forEach(function(t){var e=a(t,s);e<o&&(n=t,o=e)}),t.rect.x=n.x,t.rect.y=n.y};u.itemDragMove=function(t,e,i){function n(){s.shift(o,e,i),o.positionDropPlaceholder(),s.layout()}var o=this.isEnabled&&this.getItem(t);if(o){e-=this.size.paddingLeft,i-=this.size.paddingTop;var s=this,r=new Date;this._itemDragTime&&r-this._itemDragTime<120?(clearTimeout(this.dragTimeout),this.dragTimeout=setTimeout(n,120)):(n(),this._itemDragTime=r)}},u.itemDragEnd=function(t){function e(){2==++n&&(i.element.classList.remove("is-positioning-post-drag"),i.hideDropPlaceholder(),o.dispatchEvent("dragItemPositioned",null,[i]))}var i=this.isEnabled&&this.getItem(t);if(i){clearTimeout(this.dragTimeout),i.element.classList.add("is-positioning-post-drag");var n=0,o=this;i.once("layout",e),this.once("layoutComplete",e),i.moveTo(i.rect.x,i.rect.y),this.layout(),this.dragItemCount=Math.max(0,this.dragItemCount-1),this.sortItemsByPosition(),i.disablePlacing(),this.unstamp(i.element)}},u.bindDraggabillyEvents=function(t){this._bindDraggabillyEvents(t,"on")},u.unbindDraggabillyEvents=function(t){this._bindDraggabillyEvents(t,"off")},u._bindDraggabillyEvents=function(t,e){var i=this.handleDraggabilly;t[e]("dragStart",i.dragStart),t[e]("dragMove",i.dragMove),t[e]("dragEnd",i.dragEnd)},u.bindUIDraggableEvents=function(t){this._bindUIDraggableEvents(t,"on")},u.unbindUIDraggableEvents=function(t){this._bindUIDraggableEvents(t,"off")},u._bindUIDraggableEvents=function(t,e){var i=this.handleUIDraggable;t[e]("dragstart",i.start)[e]("drag",i.drag)[e]("dragstop",i.stop)};var c=u.destroy;return u.destroy=function(){c.apply(this,arguments),this.isEnabled=!1},h.Rect=i,h.Packer=n,h});
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          /*
Anime.js
 2017 Julian Garnier
 Released under the MIT license
*/
var $jscomp$this=this;!function(t,n){"function"==typeof define&&define.amd?define([],n):"object"==typeof module&&module.exports?module.exports=n():t.anime=n()}(this,function(){function t(t){if(!S.col(t))try{return document.querySelectorAll(t)}catch(t){}}function n(t){return t.reduce(function(t,e){return t.concat(S.arr(e)?n(e):e)},[])}function e(n){return S.arr(n)?n:(S.str(n)&&(n=t(n)||n),n instanceof NodeList||n instanceof HTMLCollection?[].slice.call(n):[n])}function r(t,n){return t.some(function(t){return t===n})}function a(t){var n,e={};for(n in t)e[n]=t[n];return e}function i(t,n){var e,r=a(t);for(e in t)r[e]=n.hasOwnProperty(e)?n[e]:t[e];return r}function u(t,n){var e,r=a(t);for(e in n)r[e]=S.und(t[e])?n[e]:t[e];return r}function o(t){t=t.replace(/^#?([a-f\d])([a-f\d])([a-f\d])$/i,function(t,n,e,r){return n+n+e+e+r+r});var n=/^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i.exec(t);return"rgb("+(t=parseInt(n[1],16))+","+parseInt(n[2],16)+","+(n=parseInt(n[3],16))+")"}function s(t){function n(t,n,e){return 0>e&&(e+=1),1<e&&--e,e<1/6?t+6*(n-t)*e:.5>e?n:e<2/3?t+(n-t)*(2/3-e)*6:t}r=/hsl\((\d+),\s*([\d.]+)%,\s*([\d.]+)%\)/g.exec(t);t=parseInt(r[1])/360;var e=parseInt(r[2])/100,r=parseInt(r[3])/100;if(0==e)e=r=t=r;else{var a=.5>r?r*(1+e):r+e-r*e,i=2*r-a,e=n(i,a,t+1/3),r=n(i,a,t);t=n(i,a,t-1/3)}return"rgb("+255*e+","+255*r+","+255*t+")"}function c(t){if(t=/([\+\-]?[0-9#\.]+)(%|px|pt|em|rem|in|cm|mm|ex|pc|vw|vh|deg|rad|turn)?/.exec(t))return t[2]}function f(t){return-1<t.indexOf("translate")?"px":-1<t.indexOf("rotate")||-1<t.indexOf("skew")?"deg":void 0}function l(t,n){return S.fnc(t)?t(n.target,n.id,n.total):t}function d(t,n){if(n in t.style)return getComputedStyle(t).getPropertyValue(n.replace(/([a-z])([A-Z])/g,"$1-$2").toLowerCase())||"0"}function p(t,n){return S.dom(t)&&r(C,n)?"transform":S.dom(t)&&(t.getAttribute(n)||S.svg(t)&&t[n])?"attribute":S.dom(t)&&"transform"!==n&&d(t,n)?"css":null!=t[n]?"object":void 0}function m(t,n){var e=f(n),e=-1<n.indexOf("scale")?1:0+e;if(!(t=t.style.transform))return e;for(var r=[],a=[],i=[],u=/(\w+)\((.+?)\)/g;r=u.exec(t);)a.push(r[1]),i.push(r[2]);return t=i.filter(function(t,e){return a[e]===n}),t.length?t[0]:e}function h(t,n){switch(p(t,n)){case"transform":return m(t,n);case"css":return d(t,n);case"attribute":return t.getAttribute(n)}return t[n]||0}function g(t,n){var e=/^(\*=|\+=|-=)/.exec(t);if(!e)return t;switch(n=parseFloat(n),t=parseFloat(t.replace(e[0],"")),e[0][0]){case"+":return n+t;case"-":return n-t;case"*":return n*t}}function v(t){return S.obj(t)&&t.hasOwnProperty("totalLength")}function y(t,n){function e(e){return e=void 0===e?0:e,t.el.getPointAtLength(1<=n+e?n+e:0)}var r=e(),a=e(-1),i=e(1);switch(t.property){case"x":return r.x;case"y":return r.y;case"angle":return 180*Math.atan2(i.y-a.y,i.x-a.x)/Math.PI}}function b(t,n){var e=/-?\d*\.?\d+/g;if(t=v(t)?t.totalLength:t,S.col(t))n=S.rgb(t)?t:S.hex(t)?o(t):S.hsl(t)?s(t):void 0;else{var r=c(t);t=r?t.substr(0,t.length-r.length):t,n=n?t+n:t}return n+="",{original:n,numbers:n.match(e)?n.match(e).map(Number):[0],strings:n.split(e)}}function w(t,n){return n.reduce(function(n,e,r){return n+t[r-1]+e})}function x(t){return(t?n(S.arr(t)?t.map(e):e(t)):[]).filter(function(t,n,e){return e.indexOf(t)===n})}function M(t){var n=x(t);return n.map(function(t,e){return{target:t,id:e,total:n.length}})}function P(t,n){var r=a(n);if(S.arr(t)){var i=t.length;2!==i||S.obj(t[0])?S.fnc(n.duration)||(r.duration=n.duration/i):t={value:t}}return e(t).map(function(t,e){return e=e?0:n.delay,t=S.obj(t)&&!v(t)?t:{value:t},S.und(t.delay)&&(t.delay=e),t}).map(function(t){return u(t,r)})}function O(t,n){var e,r={};for(e in t){var a=l(t[e],n);S.arr(a)&&1===(a=a.map(function(t){return l(t,n)})).length&&(a=a[0]),r[e]=a}return r.duration=parseFloat(r.duration),r.delay=parseFloat(r.delay),r}function $(t){return S.arr(t)?V.apply(this,t):X[t]}function A(t,n){var e;return t.tweens.map(function(r){var a=(r=O(r,n)).value,i=h(n.target,t.name),u=e?e.to.original:i,u=S.arr(a)?a[0]:u,o=g(S.arr(a)?a[1]:a,u),i=c(o)||c(u)||c(i);return r.isPath=v(a),r.from=b(u,i),r.to=b(o,i),r.start=e?e.end:t.offset,r.end=r.start+r.delay+r.duration,r.easing=$(r.easing),r.elasticity=(1e3-Math.min(Math.max(r.elasticity,1),999))/1e3,S.col(r.from.original)&&(r.round=1),e=r})}function j(t,e){return n(t.map(function(t){return e.map(function(n){var e=p(t.target,n.name);if(e){var r=A(n,t);n={type:e,property:n.name,animatable:t,tweens:r,duration:r[r.length-1].end,delay:r[0].delay}}else n=void 0;return n})})).filter(function(t){return!S.und(t)})}function I(t,n,e){var r="delay"===t?Math.min:Math.max;return n.length?r.apply(Math,n.map(function(n){return n[t]})):e[t]}function k(t){var n,e=i(T,t),r=i(E,t),a=M(t.targets),o=[],s=u(e,r);for(n in t)s.hasOwnProperty(n)||"targets"===n||o.push({name:n,offset:s.offset,tweens:P(t[n],r)});return t=j(a,o),u(e,{animatables:a,animations:t,duration:I("duration",t,r),delay:I("delay",t,r)})}function F(t){function n(){return window.Promise&&new Promise(function(t){return f=t})}function e(t){return p.reversed?p.duration-t:t}function r(t){for(var n=0,e={},r=p.animations,a={};n<r.length;){var i=r[n],u=i.animatable,o=i.tweens;a.tween=o.filter(function(n){return t<n.end})[0]||o[o.length-1],a.isPath$0=a.tween.isPath,a.round=a.tween.round,a.eased=a.tween.easing(Math.min(Math.max(t-a.tween.start-a.tween.delay,0),a.tween.duration)/a.tween.duration,a.tween.elasticity),o=w(a.tween.to.numbers.map(function(t){return function(n,e){return e=t.isPath$0?0:t.tween.from.numbers[e],n=e+t.eased*(n-e),t.isPath$0&&(n=y(t.tween.value,n)),t.round&&(n=Math.round(n*t.round)/t.round),n}}(a)),a.tween.to.strings),Y[i.type](u.target,i.property,o,e,u.id),i.currentValue=o,n++,a={isPath$0:a.isPath$0,tween:a.tween,eased:a.eased,round:a.round}}if(e)for(var s in e)L||(L=d(document.body,"transform")?"transform":"-webkit-transform"),p.animatables[s].target.style[L]=e[s].join(" ");p.currentTime=t,p.progress=t/p.duration*100}function a(t){p[t]&&p[t](p)}function i(){p.remaining&&!0!==p.remaining&&p.remaining--}function u(t){var u=p.duration,d=p.offset,m=p.delay,h=p.currentTime,g=p.reversed,v=e(t);if((v=Math.min(Math.max(v,0),u))>d&&v<u?(r(v),!p.began&&v>=m&&(p.began=!0,a("begin")),a("run")):(v<=d&&0!==h&&(r(0),g&&i()),v>=u&&h!==u&&(r(u),g||i())),t>=u&&(p.remaining?(s=o,"alternate"===p.direction&&(p.reversed=!p.reversed)):(p.pause(),f(),l=n(),p.completed||(p.completed=!0,a("complete"))),c=0),p.children)for(t=p.children,u=0;u<t.length;u++)t[u].seek(v);a("update")}t=void 0===t?{}:t;var o,s,c=0,f=null,l=n(),p=k(t);return p.reset=function(){var t=p.direction,n=p.loop;p.currentTime=0,p.progress=0,p.paused=!0,p.began=!1,p.completed=!1,p.reversed="reverse"===t,p.remaining="alternate"===t&&1===n?2:n},p.tick=function(t){o=t,s||(s=o),u((c+o-s)*F.speed)},p.seek=function(t){u(e(t))},p.pause=function(){var t=Z.indexOf(p);-1<t&&Z.splice(t,1),p.paused=!0},p.play=function(){p.paused&&(p.paused=!1,s=0,c=p.completed?0:e(p.currentTime),Z.push(p),Q||q())},p.reverse=function(){p.reversed=!p.reversed,s=0,c=e(p.currentTime)},p.restart=function(){p.pause(),p.reset(),p.play()},p.finished=l,p.reset(),p.autoplay&&p.play(),p}var L,T={update:void 0,begin:void 0,run:void 0,complete:void 0,loop:1,direction:"normal",autoplay:!0,offset:0},E={duration:1e3,delay:0,easing:"easeOutElastic",elasticity:500,round:0},C="translateX translateY translateZ rotate rotateX rotateY rotateZ scale scaleX scaleY scaleZ skewX skewY".split(" "),S={arr:function(t){return Array.isArray(t)},obj:function(t){return-1<Object.prototype.toString.call(t).indexOf("Object")},svg:function(t){return t instanceof SVGElement},dom:function(t){return t.nodeType||S.svg(t)},str:function(t){return"string"==typeof t},fnc:function(t){return"function"==typeof t},und:function(t){return void 0===t},hex:function(t){return/(^#[0-9A-F]{6}$)|(^#[0-9A-F]{3}$)/i.test(t)},rgb:function(t){return/^rgb/.test(t)},hsl:function(t){return/^hsl/.test(t)},col:function(t){return S.hex(t)||S.rgb(t)||S.hsl(t)}},V=function(){function t(t,n,e){return(((1-3*e+3*n)*t+(3*e-6*n))*t+3*n)*t}return function(n,e,r,a){if(0<=n&&1>=n&&0<=r&&1>=r){var i=new Float32Array(11);if(n!==e||r!==a)for(var u=0;11>u;++u)i[u]=t(.1*u,n,r);return function(u){if(n===e&&r===a)return u;if(0===u)return 0;if(1===u)return 1;for(var o=0,s=1;10!==s&&i[s]<=u;++s)o+=.1;var s=o+(u-i[--s])/(i[s+1]-i[s])*.1,c=3*(1-3*r+3*n)*s*s+2*(3*r-6*n)*s+3*n;if(.001<=c){for(o=0;4>o&&0!=(c=3*(1-3*r+3*n)*s*s+2*(3*r-6*n)*s+3*n);++o)var f=t(s,n,r)-u,s=s-f/c;u=s}else if(0===c)u=s;else{var s=o,o=o+.1,l=0;do{f=s+(o-s)/2,c=t(f,n,r)-u,0<c?o=f:s=f}while(1e-7<Math.abs(c)&&10>++l);u=f}return t(u,e,a)}}}}(),X=function(){function t(t,n){return 0===t||1===t?t:-Math.pow(2,10*(t-1))*Math.sin(2*(t-1-n/(2*Math.PI)*Math.asin(1))*Math.PI/n)}var n,e="Quad Cubic Quart Quint Sine Expo Circ Back Elastic".split(" "),r={In:[[.55,.085,.68,.53],[.55,.055,.675,.19],[.895,.03,.685,.22],[.755,.05,.855,.06],[.47,0,.745,.715],[.95,.05,.795,.035],[.6,.04,.98,.335],[.6,-.28,.735,.045],t],Out:[[.25,.46,.45,.94],[.215,.61,.355,1],[.165,.84,.44,1],[.23,1,.32,1],[.39,.575,.565,1],[.19,1,.22,1],[.075,.82,.165,1],[.175,.885,.32,1.275],function(n,e){return 1-t(1-n,e)}],InOut:[[.455,.03,.515,.955],[.645,.045,.355,1],[.77,0,.175,1],[.86,0,.07,1],[.445,.05,.55,.95],[1,0,0,1],[.785,.135,.15,.86],[.68,-.55,.265,1.55],function(n,e){return.5>n?t(2*n,e)/2:1-t(-2*n+2,e)/2}]},a={linear:V(.25,.25,.75,.75)},i={};for(n in r)i.type=n,r[i.type].forEach(function(t){return function(n,r){a["ease"+t.type+e[r]]=S.fnc(n)?n:V.apply($jscomp$this,n)}}(i)),i={type:i.type};return a}(),Y={css:function(t,n,e){return t.style[n]=e},attribute:function(t,n,e){return t.setAttribute(n,e)},object:function(t,n,e){return t[n]=e},transform:function(t,n,e,r,a){r[a]||(r[a]=[]),r[a].push(n+"("+e+")")}},Z=[],Q=0,q=function(){function t(){Q=requestAnimationFrame(n)}function n(n){var e=Z.length;if(e){for(var r=0;r<e;)Z[r]&&Z[r].tick(n),r++;t()}else cancelAnimationFrame(Q),Q=0}return t}();return F.version="2.0.1",F.speed=1,F.running=Z,F.remove=function(t){t=x(t);for(var n=Z.length-1;0<=n;n--)for(var e=Z[n],a=e.animations,i=a.length-1;0<=i;i--)r(t,a[i].animatable.target)&&(a.splice(i,1),a.length||e.pause())},F.getValue=h,F.path=function(n,e){var r=S.str(n)?t(n)[0]:n,a=e||100;return function(t){return{el:r,property:t,totalLength:r.getTotalLength()*(a/100)}}},F.setDashoffset=function(t){var n=t.getTotalLength();return t.setAttribute("stroke-dasharray",n),n},F.bezier=V,F.easings=X,F.timeline=function(t){var n=F(t);return n.duration=0,n.children=[],n.add=function(t){return e(t).forEach(function(t){var e=t.offset,r=n.duration;t.autoplay=!1,t.offset=S.und(e)?r:g(e,r),(t=F(t)).duration>r&&(n.duration=t.duration),n.children.push(t)}),n},n},F.random=function(t,n){return Math.floor(Math.random()*(n-t+1))+t},F});
      // Generated by CoffeeScript 1.9.3
      /*

INSTA FEED PLUGIN
LICENCE: MIT
OWNER : stevenschobert (http://instafeedjs.com)
MODIFIED BY : BLOSSOM THEMES [MIT LICENCE FOR MODIFICATION - REMAIN THE CREDIT INTACT]
********************************/
      // Generated by CoffeeScript 1.9.3
     (function(){var t;t=function(){function t(t,e){var o,i;if(this.options={target:"instafeed",get:"popular",resolution:"thumbnail",sortBy:"none",links:!0,mock:!1,useHttp:!1},"object"==typeof t)for(o in t)i=t[o],this.options[o]=i;this.context=null!=e?e:this,this.unique=this._genKey()}return t.prototype.hasNext=function(){return"string"==typeof this.context.nextUrl&&this.context.nextUrl.length>0},t.prototype.next=function(){return!!this.hasNext()&&this.run(this.context.nextUrl)},t.prototype.run=function(e){var o,i;if("string"!=typeof this.options.clientId&&"string"!=typeof this.options.accessToken)throw new Error("Missing clientId or accessToken.");if("string"!=typeof this.options.accessToken&&"string"!=typeof this.options.clientId)throw new Error("Missing clientId or accessToken.");return null!=this.options.before&&"function"==typeof this.options.before&&this.options.before.call(this),"undefined"!=typeof document&&null!==document&&((i=document.createElement("script")).id="instafeed-fetcher",i.src=e||this._buildUrl(),document.getElementsByTagName("head")[0].appendChild(i),o="instafeedCache"+this.unique,window[o]=new t(this.options,this),window[o].unique=this.unique),!0},t.prototype.parse=function(t){var e,o,i,n,r,s,a,l,p,c,h,u,d,f,m,g,y,w,b,k,_,v,E,I,x,N,B,j;if("object"!=typeof t){if(null!=this.options.error&&"function"==typeof this.options.error)return this.options.error.call(this,"Invalid JSON data"),!1;throw new Error("Invalid JSON response")}if(200!==t.meta.code){if(null!=this.options.error&&"function"==typeof this.options.error)return this.options.error.call(this,t.meta.error_message),!1;throw new Error("Error from Instagram: "+t.meta.error_message)}if(0===t.data.length){if(null!=this.options.error&&"function"==typeof this.options.error)return this.options.error.call(this,"No images were returned from Instagram"),!1;throw new Error("No images were returned from Instagram")}if(null!=this.options.success&&"function"==typeof this.options.success&&this.options.success.call(this,t),this.context.nextUrl="",null!=t.pagination&&(this.context.nextUrl=t.pagination.next_url),"none"!==this.options.sortBy)switch(N="random"===this.options.sortBy?["","random"]:this.options.sortBy.split("-"),x="least"===N[0],N[1]){case"random":t.data.sort(function(){return.5-Math.random()});break;case"recent":t.data=this._sortBy(t.data,"created_time",x);break;case"liked":t.data=this._sortBy(t.data,"likes.count",x);break;case"commented":t.data=this._sortBy(t.data,"comments.count",x);break;default:throw new Error("Invalid option for sortBy: '"+this.options.sortBy+"'.")}if("undefined"!=typeof document&&null!==document&&!1===this.options.mock){if(u=t.data,I=parseInt(this.options.limit,10),null!=this.options.limit&&u.length>I&&(u=u.slice(0,I)),s=document.createDocumentFragment(),null!=this.options.filter&&"function"==typeof this.options.filter&&(u=this._filter(u,this.options.filter)),null!=this.options.template&&"string"==typeof this.options.template){a="","","";var T=!0;for(j=document.createElement("div"),l=0,k=u.length;l<k;l++){if(p=u[l],T&&(a=a+'<div class="button-follow"><a class="follow-button" target="_blank" href="https://www.instagram.com/'+p.user.username+'/">Follow me on <i class="fa fa-instagram" aria-hidden="true"></i></a></div>',T=!1),"object"!=typeof(c=p.images[this.options.resolution]))throw r="No image found for resolution: "+this.options.resolution+".",new Error(r);m="square",(g=c.width)>(f=c.height)&&(m="landscape"),g<f&&(m="portrait"),h=c.url,window.location.protocol.indexOf("http")>=0&&!this.options.useHttp&&(h=h.replace(/https?:\/\//,"//")),a+=this._makeTemplate(this.options.template,{model:p,id:p.id,link:p.link,type:p.type,uname:p.user.username,image:h,width:g,height:f,orientation:m,caption:this._getObjectProperty(p,"caption.text"),likes:p.likes.count,comments:p.comments.count,location:this._getObjectProperty(p,"location.name")})}for(j.innerHTML=a,n=[],i=0,o=j.childNodes.length;i<o;)n.push(j.childNodes[i]),i+=1;for(w=0,_=n.length;w<_;w++)E=n[w],s.appendChild(E)}else for(b=0,v=u.length;b<v;b++){if(p=u[b],d=document.createElement("img"),"object"!=typeof(c=p.images[this.options.resolution]))throw r="No image found for resolution: "+this.options.resolution+".",new Error(r);h=c.url,window.location.protocol.indexOf("http")>=0&&!this.options.useHttp&&(h=h.replace(/https?:\/\//,"//")),d.src=h,!0===this.options.links?((e=document.createElement("a")).href=p.link,e.appendChild(d),s.appendChild(e)):s.appendChild(d)}if("string"==typeof(B=this.options.target)&&(B=document.getElementById(B)),null==B)throw r='No element with id="'+this.options.target+'" on page.',new Error(r);B.appendChild(s),document.getElementsByTagName("head")[0].removeChild(document.getElementById("instafeed-fetcher")),y="instafeedCache"+this.unique,window[y]=void 0;try{delete window[y]}catch(t){t}}return null!=this.options.after&&"function"==typeof this.options.after&&this.options.after.call(this),!0},t.prototype._buildUrl=function(){var t,e,o;switch(t="https://api.instagram.com/v1",this.options.get){case"popular":e="media/popular";break;case"tagged":if(!this.options.tagName)throw new Error("No tag name specified. Use the 'tagName' option.");e="tags/"+this.options.tagName+"/media/recent";break;case"location":if(!this.options.locationId)throw new Error("No location specified. Use the 'locationId' option.");e="locations/"+this.options.locationId+"/media/recent";break;case"user":if(!this.options.userId)throw new Error("No user specified. Use the 'userId' option.");e="users/"+this.options.userId+"/media/recent";break;default:throw new Error("Invalid option for get: '"+this.options.get+"'.")}return o=t+"/"+e,null!=this.options.accessToken?o+="?access_token="+this.options.accessToken:o+="?client_id="+this.options.clientId,null!=this.options.limit&&(o+="&count="+this.options.limit),o+="&callback=instafeedCache"+this.unique+".parse"},t.prototype._genKey=function(){var t;return""+(t=function(){return(65536*(1+Math.random())|0).toString(16).substring(1)})()+t()+t()+t()},t.prototype._makeTemplate=function(t,e){var o,i,n,r,s;for(i=/(?:\{{2})([\w\[\]\.]+)(?:\}{2})/,o=t;i.test(o);)r=o.match(i)[1],s=null!=(n=this._getObjectProperty(e,r))?n:"",o=o.replace(i,function(){return""+s});return o},t.prototype._getObjectProperty=function(t,e){var o,i;for(i=(e=e.replace(/\[(\w+)\]/g,".$1")).split(".");i.length;){if(o=i.shift(),!(null!=t&&o in t))return null;t=t[o]}return t},t.prototype._sortBy=function(t,e,o){var i;return i=function(t,i){var n,r;return n=this._getObjectProperty(t,e),r=this._getObjectProperty(i,e),o?n>r?1:-1:n<r?1:-1},t.sort(i.bind(this)),t},t.prototype._filter=function(t,e){var o,i,n,r;for(o=[],i=function(t){if(e(t))return o.push(t)},n=0,r=t.length;n<r;n++)i(t[n]);return o},t}(),function(t,e){"function"==typeof define&&define.amd?define([],e):"object"==typeof module&&module.exports?module.exports=e():t.Instafeed=e()}(this,function(){return t})}).call(this);
      //]]>
    </script>
    <script type='text/javascript'>
      //<![CDATA[
      $(document).ready(function(){function e(e,t){return e.replace(/<.*?>/gi,"").split(/\s+/).slice(0,t-1).join(" ")}$(".search-button, .toogle_search_button").click(function(){jQuery("html,body").animate({scrollTop:0},0),$("#tilting").addClass("searchopen"),$("body").addClass("hidescroll"),$("#searchbox").removeClass("hidden"),$(this).addClass("hidden")}),$("#btn-search-close").click(function(){$("#tilting").removeClass("searchopen"),$("body").removeClass("hidescroll"),$("#searchbox").addClass("hidden"),$(".search-button, .toogle_search_button").removeClass("hidden")}),$(".toogle_menu_button").click(function(){$(".nav-sidebar-area").addClass("open")}),$(".nav-sidebar-area .toggle-button").click(function(){$(".nav-sidebar-area").removeClass("open")}),$(".popular-posts li").map(function(){if($(this).find(".item-thumbnail").length<1){var t='<div class="item-thumbnail"><a href="'+$(this).find(".item-title").find("a").attr("href")+'" target="_blank"><img alt="" src="https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/w90-h100-p-k-no-nu/notfound.png" border="0"></a></div>';$(this).find(".item-content").prepend(t)}else{var a=$(this).find(".item-thumbnail").find("img"),s=a.attr("src");-1!=s.indexOf("w72-h72-p-k-no-nu")&&(s=s.replace("w72-h72-p-k-no-nu","w90-h100-p-k-no-nu"),a.attr("src",s)),-1!=s.indexOf("w72-h72-n-k-no-nu")&&(s=s.replace("w72-h72-n-k-no-nu","w90-h100-n-k-no-nu"),a.attr("src",s))}if($(this).find(".item-snippet").length>0){var l=$(this).find(".item-snippet");l.html(e(l.html(),13))}}),$(".Label .widget-content li a,.shutter-max-limit").map(function(){$(this).attr("href",$(this).attr("href")+"?&max-results="+perpage)});var t=-1,a="",s="";$("#nav-responsive").find("ul").find("li").each(function(){for(var e=$(this).text(),l=$(this).find("a").attr("href"),i=0,r=0;r<e.length&&-1!=(i=e.indexOf("_",i));r++)i++;if(level=r,level>t&&(a+="<ul>",s+="<ul>"),level<t){offset=t-level;for(r=0;r<offset;r++)a+="</ul></li>",s+="</ul></li>"}e=e.replace(/_/gi,""),a+="<li><a href='"+l+"'>"+e+"</a>",s+="<li><a href='"+l+"'>";for(r=0;r<level;r++)s+="";s+=e+"</a>",t=level});for(l=0;t>=l;l++)a+="</ul>",s+="</ul>",0!=l&&(a+="</li>",s+="</li>");$("#nav-responsive").html(s),$("#nav-responsive li a").map(function(){var e=$(this).attr("href");if(-1!=(e=e.toLowerCase()).indexOf("[mega menu]")){var t="/search/label/"+$(this).text()+"?&max-results="+perpage;$(this).attr("href",t)}});var t=-1,a="",s="";$("#navmenu").find("ul").find("li").each(function(){for(var e=$(this).text(),l=$(this).find("a").attr("href"),i=0,r=0;r<e.length&&-1!=(i=e.indexOf("_",i));r++)i++;if(level=r,level>t&&(a+="<ul>",s+="<ul>"),level<t){offset=t-level;for(r=0;r<offset;r++)a+="</ul></li>",s+="</ul></li>"}e=e.replace(/_/gi,""),a+="<li><a href='"+l+"'>"+e+"</a>",s+="<li><a href='"+l+"'>";for(r=0;r<level;r++)s+="";s+=e+"</a>",t=level});for(var l=0;t>=l;l++)a+="</ul>",s+="</ul>",0!=l&&(a+="</li>",s+="</li>");$("#navmenu").html(function(){$(this).html(s),$("#navmenu li a").map(function(){var e=$(this),t=e.attr("href");if(-1!=(t=t.toLowerCase()).indexOf("[mega menu]")){var a=e.text();$.ajax({url:"/feeds/posts/default/-/"+a+"?alt=json-in-script&max-results=4",type:"get",dataType:"jsonp",success:function(t){for(f=0;f<t.feed.link.length;f++){var s=t.feed.link[f],l=s.rel,i=s.type;if("alternate"==l&&"text/html"==i){var r=s.href+"?&max-results="+perpage;e.attr("href",r)}}var n=t.feed.openSearch$totalResults.$t,d=t.feed.openSearch$startIndex.$t,o=t.feed.openSearch$itemsPerPage.$t;if(n>4)c="";else var c="nav-disable";var u=Math.ceil(n/o);if(t.feed.entry){for(var h='<ul class="mega-list" data-itemnums="'+o+'" data-label="'+a+'" data-start="'+d+'" data-stages="'+u+'" data-cstage="1" data-tpst="'+n+'"><li><a class="upnav nav-disable" href="javascript:;"><i class="ion-chevron-up"></i></a><div class="items-shutter"><div class="item-shutter-table"><div class="item-shutter-cell"><div class="shutter-mega-loadingwrapper hidden"><div class="shutter-loading-table"><div class="shutter-loading-cell"><div class="shutter-loading"></div></div></div></div>',f=0;f<t.feed.entry.length;f++){var v=t.feed.entry[f];if(v.media$thumbnail)-1!==(m=v.media$thumbnail.url).indexOf("/s72-c")&&(m=m.replace("/s72-c","/s1600")),-1!==m.indexOf("img.youtube.com")&&(m=m.replace("/default.jpg","/maxresdefault.jpg"));else var m="https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/s1600/notfound.png";for(var g=v.title.$t,p=0;p<v.link.length;p++)if("alternate"==v.link[p].rel)var b=v.link[p].href;h=h+'<div class="shutter-mega-item"><div class="shutter-m-thumb" style="background:url(\''+m+'\')"></div><div class="shutter-text"><a href="'+b+'">'+g+"</a></div></div>"}h=h+'</div></div></div><a class="downnav '+c+'" href="javascript:;"><i class="ion-chevron-down"></i></a></li></ul>',e.closest("li").addClass("shutter-mega-list"),e.after(h);var A=e.closest(".shutter-mega-list").find(".mega-list");A.find(".upnav").click(function(){var e=$(this).closest(".mega-list"),t=e.attr("data-label"),a=Number(e.attr("data-start")),s=Number(e.attr("data-cstage")),l=(Number(e.attr("data-stages")),Number(e.attr("data-itemnums")));if(a-=l,s-1<=1?$(this).addClass("nav-disable"):$(this).removeClass("nav-disable"),e.find(".downnav").removeClass("nav-disable"),s>1){e.find(".shutter-mega-loadingwrapper").removeClass("hidden");var i='<div class="shutter-mega-loadingwrapper hidden"><div class="shutter-loading-table"><div class="shutter-loading-cell"><div class="shutter-loading"></div></div></div></div>',r="/feeds/posts/default/-/"+t+"?alt=json-in-script&start-index="+a+"&max-results="+l;$.ajax({url:r,type:"get",dataType:"jsonp",success:function(t){if(e.attr("data-start",a),e.attr("data-cstage",s-1),t.feed.entry){for(var l=0;l<t.feed.entry.length;l++){var r=t.feed.entry[l];if(r.media$thumbnail)-1!==(n=r.media$thumbnail.url).indexOf("/s72-c")&&(n=n.replace("/s72-c","/s1600")),-1!==n.indexOf("img.youtube.com")&&(n=n.replace("/default.jpg","/maxresdefault.jpg"));else var n="https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/s1600/notfound.png";for(var d=r.title.$t,o=0;o<r.link.length;o++)if("alternate"==r.link[o].rel)var c=r.link[o].href;i=i+'<div class="shutter-mega-item"><div class="shutter-m-thumb" style="background:url(\''+n+'\')"></div><div class="shutter-text"><a href="'+c+'">'+d+"</a></div></div>"}e.find(".item-shutter-cell").html(i)}}})}}),A.find(".downnav").click(function(){var e=$(this).closest(".mega-list"),t=e.attr("data-label"),a=Number(e.attr("data-start")),s=Number(e.attr("data-cstage")),l=Number(e.attr("data-stages")),i=Number(e.attr("data-itemnums"));if(a+=i,s+1==l?$(this).addClass("nav-disable"):$(this).removeClass("nav-disable"),s>=1?e.find(".upnav").removeClass("nav-disable"):e.find(".upnav").addClass("nav-disable"),l>s){e.find(".shutter-mega-loadingwrapper").removeClass("hidden");var r='<div class="shutter-mega-loadingwrapper hidden"><div class="shutter-loading-table"><div class="shutter-loading-cell"><div class="shutter-loading"></div></div></div></div>',n="/feeds/posts/default/-/"+t+"?alt=json-in-script&start-index="+a+"&max-results="+i;$.ajax({url:n,type:"get",dataType:"jsonp",success:function(t){if(e.attr("data-start",a),e.attr("data-cstage",s+1),t.feed.entry){for(var l=0;l<t.feed.entry.length;l++){var i=t.feed.entry[l];if(i.media$thumbnail)-1!==(n=i.media$thumbnail.url).indexOf("/s72-c")&&(n=n.replace("/s72-c","/s1600")),-1!==n.indexOf("img.youtube.com")&&(n=n.replace("/default.jpg","/maxresdefault.jpg"));else var n="https://4.bp.blogspot.com/-wPwjv7-YYGY/Wc98wlDT8qI/AAAAAAAAAEE/mH8YkPl8qJAH9FMuFKcShQvXXYMmVyrIgCLcBGAs/s1600/notfound.png";for(var d=i.title.$t,o=0;o<i.link.length;o++)if("alternate"==i.link[o].rel)var c=i.link[o].href;r=r+'<div class="shutter-mega-item"><div class="shutter-m-thumb" style="background:url(\''+n+'\')"></div><div class="shutter-text"><a href="'+c+'">'+d+"</a></div></div>"}e.find(".item-shutter-cell").html(r)}}})}})}}})}}),$(this).children("ul").superfish({animation:{opacity:"show"},delay:700})}),$(".FeaturedPost .post-summary").map(function(){if($(this).find(".image")){var e=$(this).find(".image").attr("src");$(this).attr("style","background-image:url("+e+");")}$(this).append("<div class='overlay'></div>")});var i=0,r=!1,n=!1;$("#sidebar-left-1").length<1?$("#left-sidebar-area").remove():(i++,r=!0),$("#sidebar-right-1").length<1?$("#right-sidebar-area").remove():(i++,n=!0),2==i&&($("#content-area").toggleClass("col-md-8").toggleClass("col-lg-6").toggleClass("col-md-push-3"),$("#right-sidebar-area").toggleClass("col-md-4").toggleClass("col-lg-3"),$("#left-sidebar-area").toggleClass("col-md-4").toggleClass("col-lg-3").toggleClass("col-md-pull-6")),0==i?($("#content-area").toggleClass("col-md-8").toggleClass("col-md-12"),$("body").addClass("shutter-no-sidebar")):(1==r&&1==n&&$("body").addClass("shutter-two-sidebar"),0==r&&1==n&&$("body").addClass("shutter-one-sidebar"),1==r&&0==n&&($("#content-area").addClass("col-md-push-4"),$("#left-sidebar-area").addClass("col-md-pull-8"),$("body").addClass("shutter-one-sidebar")))});
      //]]>
    </script>

    <script type='text/javascript'>
      //<![CDATA[
      $(document).ready(function(){$(".grid-wrapper").imagesLoaded(function(){function n(n,e,t,a){var i,r,o,u=!0;if(!t)var t=0;$(window).scroll(function(){u=!0}),setInterval(function(){u&&(u=!1,o=$(this).scrollTop(),$(n).each(function(t){i=$(this).offset().top-$(window).height()/2,r=$(this).height(),o>=i&&!$(this).hasClass(e)&&($(this).hasClass("anim-done")||($(this).hasClass("noapply"),$(this).addClass(e)),"function"==typeof a&&a(n))}))},100)}function e(){switch(loadinganimation){case"expand":anime({targets:".run-anim",duration:function(n,e){return 600+75*e},easing:"easeOutExpo",delay:function(n,e){return 50*e},opacity:{value:[0,1],easing:"linear"},scale:[0,1]});break;case"slideup":anime({targets:".run-anim",duration:function(n,e){return 500+50*e},easing:"easeOutExpo",delay:function(n,e){return 20*e},opacity:{value:[0,1],duration:function(n,e){return 250+50*e},easing:"linear"},translateY:[400,0]});break;case"slideright":anime({targets:".run-anim",duration:800,easing:[.1,1,.3,1],delay:function(n,e){return 20*e},opacity:{value:[0,1],duration:600,easing:"linear"},translateX:[-500,0],rotateZ:[15,0]});break;case"shaking":anime({targets:".run-anim",duration:900,elasticity:500,delay:function(n,e){return 15*e},opacity:{value:[0,1],duration:300,easing:"linear"},translateX:function(){return[0===anime.random(0,1)?100:-100,0]},translateY:function(){return[0===anime.random(0,1)?100:-100,0]}});break;case"flipdown":$(".grid-item").map(function(){$(this).css("perspective","800px").css("transform-origin","50% 0% 0px")}),anime({targets:".run-anim",duration:1500,elasticity:400,delay:function(n,e){return 75*e},opacity:{value:[0,1],duration:1e3,easing:"linear"},rotateX:[-90,0]});break;case"revolve":$(".grid-item").map(function(){$(this).css("perspective","3000")}),anime({targets:".run-anim",duration:function(){return anime.random(500,1e3)},easing:[.2,1,.3,1],delay:function(n,e){return 50*e},opacity:{value:[0,1],duration:700,easing:"linear"},translateZ:{value:[-3e3,0],duration:1e3},rotateY:["-1turns",0]});break;case"jelly":anime({targets:".run-anim",duration:800,elasticity:600,delay:function(n,e){return 100*e},opacity:{value:[0,1],duration:600,easing:"linear"},scaleX:{value:[.4,1]},scaleY:{value:[.6,1],duration:1e3}});break;case"dropin":$(".grid-item").map(function(){$(this).css("perspective","1000").css("origin","50% 0%")}),anime({targets:".run-anim",duration:800,easing:[.1,1,.3,1],delay:function(n,e){return 35*e},opacity:{value:[0,1],duration:600,easing:"linear"},translateX:[100,0],translateY:[-100,0],translateZ:[400,0],rotateZ:[10,0],rotateX:[75,0]});break;case"spring":$(".grid-item").map(function(){$(this).css("origin","50% 0%")}),anime({targets:".run-anim",duration:500,easing:"easeOutBack",delay:function(n,e){return 100*e},opacity:{value:[0,1],easing:"linear"},translateY:[400,0],scaleY:[{value:[3,.6],delay:function(n,e){return 100*e+120},duration:300,easing:"easeOutExpo"},{value:[.6,1],duration:1400,easing:"easeOutElastic"}],scaleX:[{value:[.9,1.05],delay:function(n,e){return 100*e+120},duration:300,easing:"easeOutExpo"},{value:[1.05,1],duration:1400,easing:"easeOutElastic"}]});break;case"spred":anime({targets:".run-anim",duration:600,easing:"easeOutExpo",delay:function(n,e){return 100*e},opacity:{value:[0,1],duration:100,easing:"linear"},translateX:function(n,e){var t={left:document.body.scrollLeft+document.documentElement.scrollLeft},a=window.innerWidth/2+t.left,i=n.getBoundingClientRect();return[a-(i.left+t.left+i.width/2),0]},translateY:function(n,e){var t={top:document.body.scrollTop+document.documentElement.scrollTop},a=window.innerHeight+t.top,i=n.getBoundingClientRect();return[a-(i.top+t.top+i.height/2),0]},rotate:function(n,e){var t=window.innerWidth/2,a=n.getBoundingClientRect();return[a.left+a.width/2<t?90:-90,0]},scale:[0,1]});break;default:anime({targets:".run-anim",duration:600,easing:"easeOutExpo",delay:function(n,e){return 100*e},opacity:{value:[0,1],duration:100,easing:"linear"},translateX:function(n,e){var t={left:document.body.scrollLeft+document.documentElement.scrollLeft},a=window.innerWidth/2+t.left,i=n.getBoundingClientRect();return[a-(i.left+t.left+i.width/2),0]},translateY:function(n,e){var t={top:document.body.scrollTop+document.documentElement.scrollTop},a=window.innerHeight+t.top,i=n.getBoundingClientRect();return[a-(i.top+t.top+i.height/2),0]},rotate:function(n,e){var t=window.innerWidth/2,a=n.getBoundingClientRect();return[a.left+a.width/2<t?90:-90,0]},scale:[0,1]})}$(".run-anim").addClass("anim-done").removeClass("run-anim").removeClass("noapply")}$(".grid-wrapper").packery({itemSelector:".grid-item",gutter:0}),n(".grid-item","run-anim",300,function(){e()}),n(".insta-pic","run-insta",300,function(){anime({targets:".run-insta",duration:function(n,e){return 600+75*e},easing:"easeOutExpo",delay:function(n,e){return 50*e},opacity:{value:[0,1],easing:"linear"},scale:[0,1]}),$(".run-insta").addClass("anim-done").removeClass("run-insta")})})});
      //]]>
    </script>

    <b:if cond='data:blog.pageType in {&quot;index&quot;,&quot;archive&quot;}'>
      <script>
        //<![CDATA[

function pagination(e){var a="";leftnum=parseInt(numshowpage/2),leftnum==numshowpage-leftnum&&(numshowpage=2*leftnum+1),start=postnumber-leftnum,start<1&&(start=1),maximum=parseInt(e/postperpage)+1,maximum-1==e/postperpage&&(maximum-=1),end=start+numshowpage-1,end>maximum&&(end=maximum),a+="<span class='totalpages'>Page "+postnumber+" of "+maximum+"</span>";var t=parseInt(postnumber)-1;postnumber>1&&(a+=2==postnumber?"page"==type?'<span class="showpage"><a href="'+home_page+'">'+prevpage+"</a></span>":'<span class="pagenumber"><a href="/search/label/'+lblname1+"?&max-results="+postperpage+'">'+prevpage+"</a></span>":"page"==type?'<span class="pagenumber"><a href="#" onclick="redirectpage('+t+');return false">'+prevpage+"</a></span>":'<span class="pagenumber"><a href="#" onclick="redirectlabel('+t+');return false">'+prevpage+"</a></span>"),start>1&&(a+="page"==type?'<span class="pagenumber"><a href="'+home_page+'">1</a></span>':'<span class="pagenumber"><a href="/search/label/'+lblname1+"?&max-results="+postperpage+'">1</a></span>'),start>2&&(a+="");for(var s=start;s<=end;s++)a+=postnumber==s?'<span class="current">'+s+"</span>":1==s?"page"==type?'<span class="pagenumber"><a href="'+home_page+'">1</a></span>':'<span class="pagenumber"><a href="/search/label/'+lblname1+"?&max-results="+postperpage+'">1</a></span>':"page"==type?'<span class="pagenumber"><a href="#" onclick="redirectpage('+s+');return false">'+s+"</a></span>":'<span class="pagenumber"><a href="#" onclick="redirectlabel('+s+');return false">'+s+"</a></span>";end<maximum-1&&(a+=""),end<maximum&&(a+="page"==type?'<span class="pagenumber"><a href="#" onclick="redirectpage('+maximum+');return false">'+maximum+"</a></span>":'<span class="pagenumber"><a href="#" onclick="redirectlabel('+maximum+');return false">'+maximum+"</a></span>");var r=parseInt(postnumber)+1;postnumber<maximum&&(a+="page"==type?'<span class="pagenumber"><a href="#" onclick="redirectpage('+r+');return false">'+nextpage+"</a></span>":'<span class="pagenumber"><a href="#" onclick="redirectlabel('+r+');return false">'+nextpage+"</a></span>");for(var n=document.getElementsByName("pageArea"),p=document.getElementById("shutter-pager"),i=0;i<n.length;i++)n[i].innerHTML=a;n&&n.length>0&&(a=""),p&&(p.innerHTML=a)}function paginationall(e){var a=e.feed;pagination(parseInt(a.openSearch$totalResults.$t,10))}function bloggerpage(){var e=urlactivepage;-1!=e.indexOf("/search/label/")&&(lblname1=-1!=e.indexOf("?updated-max")?e.substring(e.indexOf("/search/label/")+14,e.indexOf("?updated-max")):e.substring(e.indexOf("/search/label/")+14,e.indexOf("?&max"))),-1==e.indexOf("?q=")&&-1==e.indexOf(".html")&&(-1==e.indexOf("/search/label/")?(type="page",postnumber=-1!=urlactivepage.indexOf("#PageNo=")?urlactivepage.substring(urlactivepage.indexOf("#PageNo=")+8,urlactivepage.length):1,document.write('<script src="'+home_page+'feeds/posts/summary?max-results=1&alt=json-in-script&callback=paginationall"><\/script>')):(type="label",-1==e.indexOf("&max-results=")&&(postperpage=20),postnumber=-1!=urlactivepage.indexOf("#PageNo=")?urlactivepage.substring(urlactivepage.indexOf("#PageNo=")+8,urlactivepage.length):1,document.write('<script src="'+home_page+"feeds/posts/summary/-/"+lblname1+'?alt=json-in-script&callback=paginationall&max-results=1" ><\/script>')))}function redirectpage(e){jsonstart=(e-1)*postperpage,nopage=e;var a=document.getElementsByTagName("head")[0],t=document.createElement("script");t.type="text/javascript",t.setAttribute("src",home_page+"feeds/posts/summary?start-index="+jsonstart+"&max-results=1&alt=json-in-script&callback=finddatepost"),a.appendChild(t)}function redirectlabel(e){jsonstart=(e-1)*postperpage,nopage=e;var a=document.getElementsByTagName("head")[0],t=document.createElement("script");t.type="text/javascript",t.setAttribute("src",home_page+"feeds/posts/summary/-/"+lblname1+"?start-index="+jsonstart+"&max-results=1&alt=json-in-script&callback=finddatepost"),a.appendChild(t)}function finddatepost(e){post=e.feed.entry[0];var a=post.published.$t.substring(0,19)+post.published.$t.substring(23,29),t=encodeURIComponent(a);if("page"==type)s="/search?updated-max="+t+"&max-results="+postperpage+"#PageNo="+nopage;else var s="/search/label/"+lblname1+"?updated-max="+t+"&max-results="+postperpage+"#PageNo="+nopage;location.href=s}var $=jQuery;if("number"==pagit){var postperpage=perpage,numshowpage=4,prevpage='<i class="ion-arrow-left-c"></i>',nextpage='<i class="ion-arrow-right-c"></i>',urlactivepage=location.href,home_page="/",nopage,type,postnumber,lblname1;bloggerpage()}"infinite"==pagit&&function(e){function a(){if(e(".shutter-infinite-loading").fadeIn(),!i){if(i=!0,!r)return e(".shutter-infinite-loading").fadeOut(),void n.html("<a class=\"disable\" href='javascript:void(0);'>No more posts found.</a>");n.find("a").hide(),n.find("img").show(),e.ajax(r,{dataType:"html"}).done(function(a){var t=e("<div></div>").append(a.replace(o,"")),s=t.find("a.shutter-older-link");s?r=s.attr("href"):(r="",n.hide());var l=t.find(p).children();e(p).append(l),e(p).find("article.ajax_pickup.hidden").map(function(){var a="."+e(this).attr("data-class");post(a,"grid-appending")}),window._gaq&&window._gaq.push(["_trackPageview",r]),n.find("img").hide(),n.find("a").show(),e(".shutter-infinite-loading").fadeOut(),i=!1})}}function t(){return Math.max(l.height(),c.height(),document.documentElement.clientHeight)}function s(){t(),l.scrollTop(),l.height()}var r="",n=null,p=".grid-wrapper",i=!1,l=e(window),c=e(document),o=/<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi;e(document).ready(function(){if("item"!=_WidgetManager._GetAllData().blog.pageType&&(r=e("a.shutter-older-link").attr("href"))){var t=e('<a href="javascript:;">Load more posts</a>');t.click(a);var p=e('<div class="shutter-infinite-loading"  style="display: none;"><div class="shttr-thecube"><div class="shttr-cube shttr-c1"></div><div class="shttr-cube shttr-c2"></div><div class="shttr-cube shttr-c4"></div><div class="shttr-cube shttr-c3"></div></div></div>');l.scroll(s),(n=e('<div class="shutter-loadmore"></div>')).append(t),n.append(p),n.insertBefore(e("#shutter-pager")),e("#shutter-pager").hide()}})}(jQuery),"arrow"==pagit&&$("#shutter-pager").addClass("arrow");

        //]]>
      </script>
    </b:if>

  </body>
  <macro:includable id='sections' var='col'>
    <macro:if cond='data:col.num == 0'>
      <macro:else/>
      <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-1&quot;' preferred='yes' showaddelement='yes'/>

      <macro:if cond='data:col.num &gt;= 2'>
        <div mexpr:class='&quot;section-columns shutter-columns-&quot; + data:col.num'>
          <div>
            <div>
              <div class='first columns-cell'>
                <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-1&quot;'/>
              </div>

              <div class='columns-cell'>
                <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-2&quot;'/>
              </div>

              <macro:if cond='data:col.num &gt;= 3'>
                <div class='columns-cell'>
                  <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-3&quot;'/>
                </div>
              </macro:if>

              <macro:if cond='data:col.num &gt;= 4'>
                <div class='columns-cell'>
                  <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-4&quot;'/>
                </div>
              </macro:if>
            </div>
          </div>
        </div>

        <macro:if cond='data:col.includeBottom'>
          <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-3&quot;' showaddelement='no'/>
        </macro:if>
      </macro:if>
    </macro:if>
  </macro:includable>




  <b:section-contents id='sidebar-right-1'>
  <b:widget id='Label1' locked='false' title='Labels' type='Label' version='1'>
    <b:widget-settings>
      <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
      <b:widget-setting name='display'>LIST</b:widget-setting>
      <b:widget-setting name='selectedLabelsList'/>
      <b:widget-setting name='showType'>ALL</b:widget-setting>
      <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
        <b:if cond='data:title != &quot;&quot;'>
          <h2><data:title/></h2>
        </b:if>
        <div expr:class='&quot;widget-content &quot; + data:display + &quot;-label-widget-content&quot;'>
          <b:if cond='data:display == &quot;list&quot;'>
            <ul>
              <b:loop values='data:labels' var='label'>
                <li>
                  <b:if cond='data:blog.url == data:label.url'>
                    <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                    <b:else/>
                    <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                  </b:if>
                  <b:if cond='data:showFreqNumbers'>
                    <span dir='ltr'>(<data:label.count/>)</span>
                  </b:if>
                </li>
              </b:loop>
            </ul>
            <b:else/>
            <b:loop values='data:labels' var='label'>
              <span expr:class='&quot;label-size label-size-&quot; + data:label.cssSize'>
                <b:if cond='data:blog.url == data:label.url'>
                  <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                  <b:else/>
                  <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                </b:if>
                <b:if cond='data:showFreqNumbers'>
                  <span class='label-count' dir='ltr'>(<data:label.count/>)</span>
                </b:if>
              </span>
            </b:loop>
          </b:if>
          <b:include name='quickedit'/>
        </div>
      </b:includable>
  </b:widget>
  <b:widget id='FollowByEmail1' locked='false' title='Follow by Email' type='FollowByEmail' version='1'>
    <b:includable id='main'>
        <b:if cond='data:title != &quot;&quot;'><h2 class='title'><data:title/></h2></b:if>
        <div class='widget-content'>
          <div class='follow-by-email-inner'>
            <form action='https://feedburner.google.com/fb/a/mailverify' expr:onsubmit='&quot;window.open(\&quot;https://feedburner.google.com/fb/a/mailverify?uri=&quot; + data:feedPath + &quot;\&quot;, \&quot;popupwindow\&quot;, \&quot;scrollbars=yes,width=550,height=520\&quot;); return true&quot;' method='post' target='popupwindow'>
              <table width='100%'>
                <tr>
                  <td>
                    <input class='follow-by-email-address' name='email' placeholder='Email address...' type='text'/>
                  </td>
                  <td width='64px'>
                    <input class='follow-by-email-submit' type='submit' value='Submit'/>
                  </td>
                </tr>
              </table>
              <input expr:value='data:feedPath' name='uri' type='hidden'/>
              <input name='loc' type='hidden' value='en_US'/>
            </form>
          </div>
        </div>
        <span class='item-control blog-admin'>
          <b:include name='quickedit'/>
        </span>
      </b:includable>
  </b:widget>
  <b:widget id='BlogArchive1' locked='false' title='Blog Archive' type='BlogArchive' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showStyle'>HIERARCHY</b:widget-setting>
      <b:widget-setting name='yearPattern'>yyyy</b:widget-setting>
      <b:widget-setting name='showWeekEnd'>true</b:widget-setting>
      <b:widget-setting name='monthPattern'>MMMM</b:widget-setting>
      <b:widget-setting name='dayPattern'>MMM dd</b:widget-setting>
      <b:widget-setting name='weekPattern'>MM/dd</b:widget-setting>
      <b:widget-setting name='chronological'>false</b:widget-setting>
      <b:widget-setting name='showPosts'>true</b:widget-setting>
      <b:widget-setting name='frequency'>MONTHLY</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
        <b:if cond='data:title != &quot;&quot;'>
          <h2><data:title/></h2>
        </b:if>
        <div class='widget-content'>
          <div id='ArchiveList'>
            <div expr:id='data:widget.instanceId + &quot;_ArchiveList&quot;'>
              <b:include cond='data:style == &quot;HIERARCHY&quot;' data='data' name='interval'/>
              <b:include cond='data:style == &quot;FLAT&quot;' data='data' name='flat'/>
              <b:include cond='data:style == &quot;MENU&quot;' data='data' name='menu'/>
            </div>
          </div>
          <b:include name='quickedit'/>
        </div>
      </b:includable>
    <b:includable id='flat' var='data'>
        <ul class='flat'>
          <b:loop values='data:data' var='i'>
            <li class='archivedate'>
              <a expr:href='data:i.url'><data:i.name/></a> (<data:i.post-count/>)
            </li>
          </b:loop>
        </ul>
      </b:includable>
    <b:includable id='interval' var='intervalData'>
        <b:loop values='data:intervalData' var='interval'>
          <ul class='hierarchy'>
            <li expr:class='&quot;archivedate &quot; + data:interval.expclass'>
              <b:include cond='data:interval.toggleId' data='interval' name='toggle'/>
              <a class='post-count-link' expr:href='data:interval.url'>
                <data:interval.name/>
              </a>
              <span class='post-count' dir='ltr'>(<data:interval.post-count/>)</span>
              <b:include cond='data:interval.data' data='interval.data' name='interval'/>
              <b:include cond='data:interval.posts' data='interval.posts' name='posts'/>
            </li>
          </ul>
        </b:loop>
      </b:includable>
    <b:includable id='menu' var='data'>
        <select expr:id='data:widget.instanceId + &quot;_ArchiveMenu&quot;'>
          <option value=''><data:title/></option>
          <b:loop values='data:data' var='i'>
            <option expr:value='data:i.url'><data:i.name/> (<data:i.post-count/>)</option>
          </b:loop>
        </select>
      </b:includable>
    <b:includable id='posts' var='posts'>
        <ul class='posts'>
          <b:loop values='data:posts' var='post'>
            <li><a expr:href='data:post.url'><data:post.title/></a></li>
          </b:loop>
        </ul>
      </b:includable>
    <b:includable id='toggle' var='interval'>
        <a class='toggle' href='javascript:void(0)'>
          <span expr:class='&quot;zippy&quot; + (data:interval.expclass == &quot;expanded&quot; ? &quot; toggle-open&quot; : &quot;&quot;)'>
            <b:if cond='data:interval.expclass == &quot;expanded&quot;'>
              &#9660;&#160;
              <b:elseif cond='data:blog.languageDirection == &quot;rtl&quot;'/>
              &#9668;&#160;
              <b:else/>
              &#9658;&#160;
            </b:if>
          </span>
        </a>
      </b:includable>
  </b:widget>
  <b:widget id='FeaturedPost1' locked='false' title='Featured Post' type='FeaturedPost' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showSnippet'>true</b:widget-setting>
      <b:widget-setting name='showPostTitle'>true</b:widget-setting>
      <b:widget-setting name='postId'>8494477366576540598</b:widget-setting>
      <b:widget-setting name='showFirstImage'>true</b:widget-setting>
      <b:widget-setting name='useMostRecentPost'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
        <!-- Only display title if it's non-empty -->
        <b:if cond='data:title != &quot;&quot;'>
          <h2 class='title'><data:title/></h2>
        </b:if>
        <b:include name='content'/>

        <b:include name='quickedit'/>
      </b:includable>
    <b:includable id='content'>
        <div class='post-summary'>
          <b:if cond='data:showPostTitle and data:postTitle != &quot;&quot;'>
            <h3><a expr:href='data:postUrl'><data:postTitle/></a></h3>
          </b:if>
          <b:if cond='data:showSnippet and data:postSummary != &quot;&quot;'>
            <p>
              <data:postSummary/>
            </p>
          </b:if>
          <b:if cond='data:showFirstImage and data:postFirstImage != &quot;&quot;'>
            <img class='image' expr:src='data:postFirstImage'/>
          </b:if>
        </div>

        <style type='text/css'>
          .image {
            width: 100%;
          }
        </style>
      </b:includable>
  </b:widget>
  <b:widget id='PopularPosts1' locked='false' title='Popular Posts' type='PopularPosts' version='1'>
    <b:widget-settings>
      <b:widget-setting name='numItemsToShow'>5</b:widget-setting>
      <b:widget-setting name='showThumbnails'>true</b:widget-setting>
      <b:widget-setting name='showSnippets'>true</b:widget-setting>
      <b:widget-setting name='timeRange'>LAST_YEAR</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
        <b:if cond='data:title != &quot;&quot;'><h2><data:title/></h2></b:if>
        <div class='widget-content popular-posts'>
          <ul>
            <b:loop values='data:posts' var='post'>
              <li>
                <b:if cond='!data:showThumbnails'>
                  <b:if cond='!data:showSnippets'>
                    <!-- (1) No snippet/thumbnail -->
                    <a expr:href='data:post.href'><data:post.title/></a>
                    <b:else/>
                    <!-- (2) Show only snippets -->
                    <div class='item-title'><a expr:href='data:post.href'><data:post.title/></a></div>
                    <div class='item-snippet'><data:post.snippet/></div>
                  </b:if>
                  <b:else/>
                  <!-- (3) Show only thumbnails or (4) Snippets and thumbnails. -->
                  <div expr:class='data:showSnippets ? &quot;item-content&quot; : &quot;item-thumbnail-only&quot;'>
                    <b:if cond='data:post.featuredImage.isResizable or data:post.thumbnail'>
                      <div class='item-thumbnail'>
                        <a expr:href='data:post.href' target='_blank'>
                          <b:with value='data:post.featuredImage.isResizable                                  ? resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)                                  : data:post.thumbnail' var='image'>
                            <img alt='' border='0' expr:src='data:image'/>
                          </b:with>
                        </a>
                      </div>
                    </b:if>
                    <div class='item-title'><a expr:href='data:post.href'><data:post.title/></a></div>
                    <b:if cond='data:showSnippets'>
                      <div class='item-snippet'><data:post.snippet/></div>
                    </b:if>
                  </div>
                  <div style='clear: both;'/>
                </b:if>
              </li>
            </b:loop>
          </ul>
          <b:include name='quickedit'/>
        </div>
      </b:includable>
  </b:widget>
</b:section-contents><b:section-contents id='footer-1'/><b:section-contents id='footer-2-1'>
  <b:widget id='FollowByEmail2' locked='false' title='Follow by Email' type='FollowByEmail' version='1'>
    <b:includable id='main'>
      <b:if cond='data:title != &quot;&quot;'><h2 class='title'><data:title/></h2></b:if>
      <div class='widget-content'>
        <div class='follow-by-email-inner'>
          <form action='https://feedburner.google.com/fb/a/mailverify' expr:onsubmit='&quot;window.open(\&quot;https://feedburner.google.com/fb/a/mailverify?uri=&quot; + data:feedPath + &quot;\&quot;, \&quot;popupwindow\&quot;, \&quot;scrollbars=yes,width=550,height=520\&quot;); return true&quot;' method='post' target='popupwindow'>
            <table width='100%'>
              <tr>
                <td>
                  <input class='follow-by-email-address' name='email' placeholder='Email address...' type='text'/>
                </td>
                <td width='64px'>
                  <input class='follow-by-email-submit' type='submit' value='Submit'/>
                </td>
              </tr>
            </table>
            <input expr:value='data:feedPath' name='uri' type='hidden'/>
            <input name='loc' type='hidden' value='en_US'/>
          </form>
        </div>
      </div>
      <span class='item-control blog-admin'>
        <b:include name='quickedit'/>
      </span>
    </b:includable>
  </b:widget>
  <b:widget id='Profile1' locked='false' title='About Me' type='Profile' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showaboutme'>true</b:widget-setting>
      <b:widget-setting name='showlocation'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
      <b:if cond='data:title != &quot;&quot;'>
        <h2><data:title/></h2>
      </b:if>
      <div class='widget-content'>
        <b:if cond='data:team'> <!-- team blog profile -->
          <ul>
            <b:loop values='data:authors' var='i'>
              <li><a class='profile-name-link g-profile' expr:href='data:i.userUrl' expr:style='&quot;background-image: url(&quot; + data:i.profileLogo + &quot;);&quot;'><data:i.display-name/></a></li>
            </b:loop>
          </ul>

          <b:else/> <!-- normal blog profile -->

          <b:if cond='data:photo.url != &quot;&quot;'>
            <a expr:href='data:userUrl'><img class='profile-img' expr:alt='data:messages.myPhoto' expr:height='data:photo.height' expr:src='data:photo.url' expr:width='data:photo.width'/></a>
          </b:if>

          <dl class='profile-datablock'>
            <dt class='profile-data'>
              <a class='profile-name-link g-profile' expr:href='data:userUrl' expr:style='&quot;background-image: url(&quot; + data:profileLogo + &quot;);&quot;' rel='author'>
                <data:displayname/>
              </a>
              <b:if cond='data:hasgoogleprofile'>
                <br/>
                <div class='g-follow' data-annotation='bubble' data-height='20' expr:data-href='data:userUrl'/>
              </b:if>
            </dt>

            <b:if cond='data:showlocation'>
              <dd class='profile-data'><data:location/></dd>
            </b:if>

            <b:if cond='data:aboutme != &quot;&quot;'><dd class='profile-textblock'><data:aboutme/></dd></b:if>
          </dl>
          <a class='profile-link' expr:href='data:userUrl' rel='author'><data:viewProfileMsg/></a>
        </b:if>

        <b:include name='quickedit'/>
      </div>
    </b:includable>
  </b:widget>
</b:section-contents><b:section-contents id='footer-2-2'>
  <b:widget id='BlogArchive2' locked='false' title='Blog Archive' type='BlogArchive' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showStyle'>HIERARCHY</b:widget-setting>
      <b:widget-setting name='yearPattern'>yyyy</b:widget-setting>
      <b:widget-setting name='showWeekEnd'>true</b:widget-setting>
      <b:widget-setting name='monthPattern'>MMMM</b:widget-setting>
      <b:widget-setting name='dayPattern'>MMM dd</b:widget-setting>
      <b:widget-setting name='weekPattern'>MM/dd</b:widget-setting>
      <b:widget-setting name='chronological'>false</b:widget-setting>
      <b:widget-setting name='showPosts'>true</b:widget-setting>
      <b:widget-setting name='frequency'>MONTHLY</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
      <b:if cond='data:title != &quot;&quot;'>
        <h2><data:title/></h2>
      </b:if>
      <div class='widget-content'>
        <div id='ArchiveList'>
          <div expr:id='data:widget.instanceId + &quot;_ArchiveList&quot;'>
            <b:include cond='data:style == &quot;HIERARCHY&quot;' data='data' name='interval'/>
            <b:include cond='data:style == &quot;FLAT&quot;' data='data' name='flat'/>
            <b:include cond='data:style == &quot;MENU&quot;' data='data' name='menu'/>
          </div>
        </div>
        <b:include name='quickedit'/>
      </div>
    </b:includable>
    <b:includable id='flat' var='data'>
      <ul class='flat'>
        <b:loop values='data:data' var='i'>
          <li class='archivedate'>
            <a expr:href='data:i.url'><data:i.name/></a> (<data:i.post-count/>)
          </li>
        </b:loop>
      </ul>
    </b:includable>
    <b:includable id='interval' var='intervalData'>
      <b:loop values='data:intervalData' var='interval'>
        <ul class='hierarchy'>
          <li expr:class='&quot;archivedate &quot; + data:interval.expclass'>
            <b:include cond='data:interval.toggleId' data='interval' name='toggle'/>
            <a class='post-count-link' expr:href='data:interval.url'>
              <data:interval.name/>
            </a>
            <span class='post-count' dir='ltr'>(<data:interval.post-count/>)</span>
            <b:include cond='data:interval.data' data='interval.data' name='interval'/>
            <b:include cond='data:interval.posts' data='interval.posts' name='posts'/>
          </li>
        </ul>
      </b:loop>
    </b:includable>
    <b:includable id='menu' var='data'>
      <select expr:id='data:widget.instanceId + &quot;_ArchiveMenu&quot;'>
        <option value=''><data:title/></option>
        <b:loop values='data:data' var='i'>
          <option expr:value='data:i.url'><data:i.name/> (<data:i.post-count/>)</option>
        </b:loop>
      </select>
    </b:includable>
    <b:includable id='posts' var='posts'>
      <ul class='posts'>
        <b:loop values='data:posts' var='post'>
          <li><a expr:href='data:post.url'><data:post.title/></a></li>
        </b:loop>
      </ul>
    </b:includable>
    <b:includable id='toggle' var='interval'>
      <a class='toggle' href='javascript:void(0)'>
        <span expr:class='&quot;zippy&quot; + (data:interval.expclass == &quot;expanded&quot; ? &quot; toggle-open&quot; : &quot;&quot;)'>
          <b:if cond='data:interval.expclass == &quot;expanded&quot;'>
            &#9660;&#160;
            <b:elseif cond='data:blog.languageDirection == &quot;rtl&quot;'/>
            &#9668;&#160;
            <b:else/>
            &#9658;&#160;
          </b:if>
        </span>
      </a>
    </b:includable>
  </b:widget>
</b:section-contents><b:section-contents id='footer-2-3'>
  <b:widget id='Label2' locked='false' title='Labels' type='Label' version='1'>
    <b:widget-settings>
      <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
      <b:widget-setting name='display'>LIST</b:widget-setting>
      <b:widget-setting name='selectedLabelsList'/>
      <b:widget-setting name='showType'>ALL</b:widget-setting>
      <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
      <b:if cond='data:title != &quot;&quot;'>
        <h2><data:title/></h2>
      </b:if>
      <div expr:class='&quot;widget-content &quot; + data:display + &quot;-label-widget-content&quot;'>
        <b:if cond='data:display == &quot;list&quot;'>
          <ul>
            <b:loop values='data:labels' var='label'>
              <li>
                <b:if cond='data:blog.url == data:label.url'>
                  <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                  <b:else/>
                  <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                </b:if>
                <b:if cond='data:showFreqNumbers'>
                  <span dir='ltr'>(<data:label.count/>)</span>
                </b:if>
              </li>
            </b:loop>
          </ul>
          <b:else/>
          <b:loop values='data:labels' var='label'>
            <span expr:class='&quot;label-size label-size-&quot; + data:label.cssSize'>
              <b:if cond='data:blog.url == data:label.url'>
                <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                <b:else/>
                <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
              </b:if>
              <b:if cond='data:showFreqNumbers'>
                <span class='label-count' dir='ltr'>(<data:label.count/>)</span>
              </b:if>
            </span>
          </b:loop>
        </b:if>
        <b:include name='quickedit'/>
      </div>
    </b:includable>
  </b:widget>
</b:section-contents></html>
