---
layout: slide
title: 
lang: HTML
data:
  background: "#85ef77"
---

<section markdown="1">

##  {{ page.lang }}

The <i>lingua franca</i> of the Web.  Every student should have a chance to learn the basics.

Let's see how interactive {{ page.lang }} examples can enable this:

[![Down arrow](https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png)](#/3/1){: .image .navigate-down}

</section>
<section markdown="1">

Let students `Play` with basic HTML instantly:

{% include trinket-open type='html' height='700' %}
<html>
<head>
  <style>
  body { background: lightgrey }
  p { color: brown }
  </style>
</head>
<body>
  <h1>This is an HTML title</h1>
  <p>And this is a paragraph</p>
  <p>
    This paragraph contains an image...
    <img src="http://trinket.io/img/trinket-logo.png" width="20%" />
    ...and then some more text.  
  </p>
  <h2>Your Assignment</h2>
  <p>
    Notice that all of the paragraphs have the same 
    brown color.  That is because of the instructions 
    in the <code>&lt;style&gt;</code> at the top.
  </p>
  <p>
    Can you find <code>color: brown</code> and change
    it to be <code>color: blue</code>?  What happens?
  </p>
</body>
</html>

{% include trinket-close %}

</section>
<section markdown="1">

Trinkets can `Show` the full power of technology like CSS based animations, motivating authentic inquiry-based learning:

{% include trinket-open type='html' height='600' %}
<html>
    <head>
        <style>
        html , body {height:100%;}
    body {
    	background: #4297cd;
    	padding:0;
    	margin:0;
    }
    .ship {
    	width:350px;
    	height:20px;
    
    	margin-left:5%;
    	position:	absolute;
    }
    .ship { 
    	-webkit-animation:floating-ship 3s aletrnate ;
    	-webkit-transition-timing-function: cubic-bezier(0,.5,.99,.54);
    	-moz-animation:floating-ship 3s aletrnate ;
    	-moz-transition-timing-function: cubic-bezier(0,.5,.99,.54);
    }
     @-webkit-keyframes floating-ship {
    	 from {-webkit-transform:rotate(4deg);}
    	 to {-webkit-transform:rotate(-4deg);}
     }
     @-moz-keyframes floating-ship {
    	 from {-moz-transform:rotate(4deg);}
    	 to {-moz-transform:rotate(-4deg);}
     }
    .bottom-1 {
    	border-right:10px solid transparent;
    	border-top:12px solid #54575c;
    	border-left:16px solid transparent;
    	width:250px;
    	height:0px;
    }
    .bottom-1:after {
    	content:'';
    	display:block;
    	position:absolute;
    	top:-8px;
    	left:-7px;
    	border-right:10px solid transparent;
    	border-top:8px solid #fff;
    	border-left:7px solid transparent;
    	width:276px;
    	height:0px;
    }
    .bottom-1:before {
    	content:'';
    	display:block;
    	position:absolute;
    	top:-11px;
    	left:-8px;
    	border-right:1px solid transparent;
    	border-top:3px solid #e3001b;
    	border-left:1px solid transparent;
    	width:293px;
    	height:0px;
    }
    .bottom-1-top {
    	width:295px;
    	height:5px;
    	background:#e5e9ec;
    	position:absolute;
    	top:-16px;
    	left:-8px;
    }
    .bottom-1-top:after {
    	content:'';
    	display:block;
    	position:absolute;
    	height:5px;
    	width:20px;
    	background:red;
    	-webkit-transform:skewX(-40deg);
    	-moz-transform:skewX(-40deg);
    	background:#e5e9ec;
    	right:-2px;
    }
    .bottom-1-top-left {
    	width:60px;
    	height:15px;
    	background:#fff;
    	position:absolute;
    	top:-31px;
    	left:-8px;
    }
    .bottom-1-top-left:after {
    	content:'';
    	display:block;
    	position:absolute;
    	width:40px;
    	height:15px;
    	-webkit-transform:skewX(50deg);
    	-moz-transform:skewX(50deg);
    	background:#fff;
    	right:-9px;
    }
    .bottom-1-top-left:before {
    	content:'';
    	width:6px;
    	height:6px;
    	border-radius:50%;
    	background:#8a9295;
    	position:absolute;
    	z-index:1;
    	top:5px;
    	left:8px;
    	box-shadow:14px 0 0 #8a9295 , 28px 0 0 #8a9295 , 42px 0 0 #8a9295   ;
    }
    .bottom-1-top-right {
    	width:107px;
    	height:15px;
    	background:#fff;
    	position:absolute;
    	top:-31px;
    	left:180px;
    }
    .bottom-1-top-right:after {
    	content:'';
    	display:block;
    	position:absolute;
    	width:40px;
    	height:15px;
    	-webkit-transform:skewX(-50deg);
    	-moz-transform:skewX(-50deg);
    	background:#fff;
    	left:-9px;
    }
    .bottom-1-top-right:before {
    	content:'';
    	display:block;
    	position:absolute;
    	width:40px;
    	height:15px;
    	-webkit-transform:skewX(-50deg);
    	-moz-transform:skewX(-50deg);
    	background:#fff;
    	right:-13px;
    }
    .ship-body {
    	width:235px;
    	height:40px;
    	background:#ebebeb;
    	position:absolute;
    	top:-54px;
    	left:14px;
    	z-index:-1;
    	box-shadow: 0 -5px 7px rgba(0,0,0,0.1) inset;
    }
    .ship-body:before {
    	position:absolute;
    	left:-10px;
    	content:'';
    	width:40px;
    	-webkit-transform:skewX(-34deg);
    	-moz-transform:skewX(-34deg);
    	height:30px;
    	background:#ebebeb;
    }
    .ship-body:after {
    	position:absolute;
    	right:-16px;
    	content:'';
    	width:40px;
    	-webkit-transform:skewX(44deg);
    	-moz-transform:skewX(44deg);
    	height:30px;
    	background:#ebebeb;
    }
    .blue-strip-top {
    	background:#72a4c4;
    	width:224px;
    	height:4px;
    	position:absolute;
    	top:6px;
    	z-index:1;
    	left:8px;
    }
    .blue-strip-top:before {
    	content:'';
    	position:absolute;
    	width:10px;
    	background:#72a4c4;
    	height:4px;
    	left:-7px;
    	-webkit-transform:skewX(-30deg);
    	-moz-transform:skewX(-30deg);
    }
    .blue-strip-top:after {
    	content:'';
    	position:absolute;
    	width:10px;
    	background:#72a4c4;
    	height:4px;
    	right:-5px;
    	-webkit-transform:skewX(50deg);
    	-moz-transform:skewX(50deg);
    }
    .blue-strip-bottom {
    	background:#72a4c4;
    	width:240px;
    	height:4px;
    	position:absolute;
    	top:14px;
    	z-index:1;
    }
    .blue-strip-bottom:before {
    	content:'';
    	position:absolute;
    	width:10px;
    	background:#72a4c4;
    	height:4px;
    	left:-5px;
    	-webkit-transform:skewX(-30deg);
    	-moz-transform:skewX(-30deg);
    }
    .blue-strip-bottom:after {
    	content:'';
    	position:absolute;
    	width:10px;
    	background:#72a4c4;
    	height:4px;
    	right:-5px;
    	-webkit-transform:skewX(50deg);
    	-moz-transform:skewX(50deg);
    }
    .ship-body-top-back {
    	height:15px;
    	width:60px;
    	position:absolute;
    	background:#ebebeb;
    	top:-12px;
    	left:8px;
    }
    .ship-body-top-back:before {
    	width:15px;
    	height:15px;
    	content:'';
    	display:block;
    	position:absolute;
    	-webkit-transform:skewX(-34deg);
    	-moz-transform:skewX(-34deg);
    	background:#ebebeb;
    	left:-5px;
    }
    .ship-body-top-back:after {
    	width:15px;
    	height:15px;
    	content:'';
    	display:block;
    	position:absolute;
    	-webkit-transform:skewX(43deg);
    	-moz-transform:skewX(43deg);
    	background:#ebebeb;
    	right:-8px;
    }
    .ship-body-top-front {
    	position:absolute;
    	width:40px;
    	height:10px;
    	background:#efefef;
    	right:120px;
    	top:-74px;
    }
    .ship-body-top-front:before {
    	height:30px;
    	width:14px;
    	background:#efefef;
    	position:absolute;
    	content:'';
    	-webkit-transform:skewX(-40deg);
    	-moz-transform:skewX(-40deg);
    	left:-13px;
    	z-index:-2;
    }
    .ship-body-top-front:after {
    	height:10px;
    	width:20px;
    	background:#efefef;
    	position:absolute;
    	content:'';
    	-webkit-transform:skewX(44deg);
    	-moz-transform:skewX(44deg);
    	right:-11px;
    	z-index:-2;
    }
    .ship-body-top-front-mirror {
    	background:#a5d4e4;
    	width:40px;
    	height:18px;
    	position:absolute;
    	top:-70px;
    	right:125px;
    	z-index:-4;
    	border-radius:5px;
    }
    .ship-body-top-front-mirror:after {
    	content:'';
    	background:#a5d4e4;
    	width:40px;
    	height:18px;
    	position:absolute;
    	right:-16px;
    	-webkit-transform:skewX(44deg);
    	-moz-transform:skewX(44deg);
    	z-index:-4;
    }
    .blue-strip-top-half {
    	width:80%;
    	top:8px;
    	z-index:1;
    	height:4px;
    	background:#72a4c4;
    	position:absolute;
    	left:10%;
    }
    .blue-strip-top-half:before {
    	content:'';
    	width:10px;
    	top:0;
    	z-index:1;
    	height:4px;
    	background:#72a4c4;
    	position:absolute;
    	-webkit-transform:skewX(-30deg);
    	-moz-transform:skewX(-30deg);
    	left:-4px;
    }
    .blue-strip-top-half:after {
    	content:'';
    	width:10px;
    	top:0;
    	z-index:1;
    	height:4px;
    	background:#72a4c4;
    	position:absolute;
    	-webkit-transform:skewX(44deg);
    	-moz-transform:skewX(44deg);
    	right:-4px;
    }
    .top-antenna {
    	width:8px;
    	height:16px;
    	background:#fff;
    	position:absolute;
    	top:-16px;
    	left:20px;
    	-webkit-transform:SkewX(44deg);
    	-moz-transform:SkewX(44deg);
    }
    .top-antenna:before {
    	content:'';
    	position:absolute;
    	width:20px;
    	height:4px;
    	background:#fff;
    	display:block;
    	top:-4px;
    	-webkit-transform: skewX(-44deg) !important;
    	-moz-transform: skewX(-44deg) !important;
    	left: 2px;
    }
    .top-antenna:after {
    	content:'';
    	position:absolute;
    	width:0px;
    	height:0px;
    	border-bottom: 20px solid #fff; 
    	border-left: 2px solid transparent; 
    	border-right: 2px solid transparent;
    	display:block;
    	top:-20px;
    	right:5px;
    	z-index:-1;
    	left: 15px;
    }
    .circular-base {
    	display: block;
    position: absolute;
    bottom: 10px;
    left: 10px;
    width: 7px;
    height: 20px;
    overflow: hidden;
    }
    
    .circular-base:before {
    	display:block;
    	content:'';
    	position:absolute;
    	bottom:0px;
    	left:-10px;
    	width:20px;
    	height:20px;
    	background: -moz-radial-gradient(center, ellipse cover,  rgba(255,255,255,0) 0%, rgba(255,255,255,0) 39%, rgba(255,255,255,0.5) 40%, rgba(255,255,255,1) 41%, rgba(255,255,255,1) 100%);
    background: -webkit-gradient(radial, center center, 0px, center center, 100%, color-stop(0%,rgba(255,255,255,0)), color-stop(39%,rgba(255,255,255,0)), color-stop(40%,rgba(255,255,255,0.5)), color-stop(41%,rgba(255,255,255,1)), color-stop(100%,rgba(255,255,255,1)));
    background: -webkit-radial-gradient(center, ellipse cover,  rgba(255,255,255,0) 0%,rgba(255,255,255,0) 39%,rgba(255,255,255,0.5) 40%,rgba(255,255,255,1) 41%,rgba(255,255,255,1) 100%);
    background: -o-radial-gradient(center, ellipse cover,  rgba(255,255,255,0) 0%,rgba(255,255,255,0) 39%,rgba(255,255,255,0.5) 40%,rgba(255,255,255,1) 41%,rgba(255,255,255,1) 100%);
    background: -ms-radial-gradient(center, ellipse cover,  rgba(255,255,255,0) 0%,rgba(255,255,255,0) 39%,rgba(255,255,255,0.5) 40%,rgba(255,255,255,1) 41%,rgba(255,255,255,1) 100%);
    background: radial-gradient(ellipse at center,  rgba(255,255,255,0) 0%,rgba(255,255,255,0) 39%,rgba(255,255,255,0.5) 40%,rgba(255,255,255,1) 41%,rgba(255,255,255,1) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00ffffff', endColorstr='#ffffff',GradientType=1 );
    
    }
    .circular-base-1 {
    	position:absolute;
    	width:26px;
    	height:4px;
    	background:#fff;
    	top:-4px;
    	left:3px;
    }
    .circular-base-1:before {
    	position: absolute;
    	content: '';
    	display: block;
    	width: 8px;
    	height: 8px;
    	background: #fff;
    	top: -8px;
    	left: 13px;
    }
    .chimney-base {
    	width:60px;
    	height:5px;
    	position:absolute;
    	top:-17px;
    	left:9px;
    }
    .chimney {
    	width:25px;
    	height:10px;
    	background:#f5f5f5;
    	position:absolute;
    	bottom:0;
    	margin-left:5px;
    }
    .chimney:before {
    	content:'';
    	width:25px;
    	height:6px;
    	background:grey;
    	position:absolute;
    	top:-6px;
    }
    .chimney:after {
    	content:'';
    	width:25px;
    	height:6px;
    	background:#f7f7f7;
    	position:absolute;
    	top:-12px;
    }
    .ocean {
    	width:100%;
    	position:absolute;
    	height:100px;
    	background:rgba(25,93,164,0.8);
    	bottom:0;
    }
    .ocean-overlay {
    	width:100%;
    	position:absolute;
    	height:100px;
    	background:rgba(25,93,164,0.35);
    	bottom:0;
    	z-index:10;
    	box-shadow:0 25px 25px rgba(25,93,164,0.5) inset;
    }
    .traslate {
    	-webkit-animation:5s ease-in-out 0s normal none infinite floating;
    	-moz-animation:5s ease-in-out 0s normal none infinite floating;
    	width:150px;
    	height:20px;
    	position:absolute;
    	
    }
    @-webkit-keyframes floating {
    	0% {
    		bottom: 48px;
    		-webkit-transform:rotate(1deg);
    		-webkit-transform-origin:-20% -40%;
    	}
    	50% {
    		bottom: 52px;
    		-webkit-transform:rotate(-1deg);
    		-webkit-transform-origin:-20% -40%;
    	}
    	100% {
    		bottom: 48px;
    		-webkit-transform:rotate(1deg) ;
    		-webkit-transform-origin:-20% -40%;
    	}
    }
    @-moz-keyframes floating {
    	0% {
    		bottom: 48px;
    		-moz-transform:rotate(1deg);
    		-moz-transform-origin:-20% -40%;
    	}
    	50% {
    		bottom: 52px;
    		-moz-transform:rotate(-1deg);
    		-moz-transform-origin:-20% -40%;
    	}
    	100% {
    		bottom: 48px;
    		-moz-transform:rotate(1deg) ;
    		-moz-transform-origin:-20% -40%;
    	}
    }
    .here-there {
    	-webkit-animation:movenow 60s infinite ;
    	-moz-animation:movenow 60s infinite ;
    	position:absolute;
    	width:200px;
    	bottom:30px;
    	
    }
    @-webkit-keyframes movenow {
    	0%   {right:110%;}
    	100% {right:0;}
    }
    @-moz-keyframes movenow {
    	0%   {right:110%;}
    	100% {right:0;}
    }
    .wrap {
    	overflow:hidden;
    	position:absolute;
    	width:100%;
    	height:100%;
    }
    .bottom-1-top-right-window {
    	width:6px;
    	height:6px;
    	border-radius:50%;
    	position:absolute;
    	background:#ADB1B3 ;
    	left:3px;
    	z-index:1;
    	top:5px;
    	box-shadow:14px 0 0 #ADB1B3 , 28px 0 0 #ADB1B3 , 42px 0 0 #ADB1B3 , 56px 0 0 #ADB1B3 , 70px 0 0 #ADB1B3 , 84px 0 0 #ADB1B3 , 98px 0 0 #ADB1B3;
    }
    .middle-window {
    	width:6px;
    	height:6px;
    	border-radius:50%;
    	position:absolute;
    	background:#ADB1B3 ;
    	left:56px;
    	z-index:1;
    	bottom:6px;
    	box-shadow:14px 0 0 #ADB1B3 , 28px 0 0 #ADB1B3 , 42px 0 0 #ADB1B3 , 56px 0 0 #ADB1B3 , 70px 0 0 #ADB1B3 , 84px 0 0 #ADB1B3 ;
    }
    </style>

    </head>
<body>
    <div class="wrap">
    </div>
    
    
    <div class="ocean"></div>
    <div class="ocean-overlay"></div>
    <div class="here-there">
    	<div class="traslate">
    		<div class="ship">
    			<div class="bottom-1">
    				<div class="bottom-1-top"></div>
    				<div class="bottom-1-top-left"></div>
    				<div class="bottom-1-top-right">
    					<div class="bottom-1-top-right-window"></div>
    				</div>
    			</div>
    			<div class="ship-body">
    				<div class="middle-window"></div>
    				<div class="blue-strip-top"></div>
    				<div class="blue-strip-bottom"></div>
    				<div class="ship-body-top-back">
    					<div class="blue-strip-top-half"></div>
    				</div>
    				<div class="chimney-base">
    					<div class="chimney"></div>
    					<div class="chimney"></div>
    				</div>
    			</div>
    			<div class="ship-body-top-front">
    				<div class="top-antenna"></div>
    				<div class="circular-base"></div>
    				<div class="circular-base-1"></div>
    			</div>
    			<div class="ship-body-top-front-mirror"></div>
    		</div>
    	</div>
        </div>
    
    </body>
</html>

{% include trinket-close %}

</section>
<section markdown="1">

## What's Next?  World Domination.

Press the right arrow key to learn where you can put these interctive Trinkets

Hint: Everywhere

[![Up arrow](https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png){: style="transform: rotate(270deg);-webkit-transform: rotate(270deg);"}](#/4)

</section>