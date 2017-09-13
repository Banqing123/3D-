# 3D-
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>3D菜单翻转</title>
<link href="css/menu.css" rel="stylesheet" type="text/css">
</head>

<body>
<div class="banner">
    <ul class="banner-ul">
        <li>
            <a href="#" class="a">
                banner
                <span class="b">
                    <span class="font">banner</span>
                    <span class="font1">banner</span>
                </span>
            </a>
        </li>
        <li>
            <a href="#" class="a">
                banner2
                <span class="b">
                    <span class="font">banner2</span>
                    <span class="font1">banner2</span>
                </span>
            </a>
        </li>
        <li>
            <a href="#" class="a">
                banner3
                <span class="b">
                    <span class="font">banner3</span>
                    <span class="font1">banner3</span>
                </span>
            </a>
        </li>
        <li>
            <a href="#" class="a">
                banner4
                <span class="b">
                    <span class="font">banner4</span>
                    <span class="font1">banner4</span>
                </span>
            </a>
        </li>
        <li>
            <a href="#" class="a">
                banner5
                <span class="b">
                    <span class="font">banner5</span>
                    <span class="font1">banner5</span>
                </span>
            </a>
        </li>
    </ul>
</div>
</body>
</html>

body{margin: 0;padding: 0;font-size: 12px;font-family: "SourceHanSansSC-Light","Microsoft Yahei",微软雅黑,
"Helvetica Neue",Arial,sans-serif;width: 100%;/* [disabled]color:#757575; */background: #F6F6F6;background: #f0f0f0;}
html,dl,dt,dd,ul,ol,li,h1,h2,h4,h5,h6,pre,form,fieldset,input,textarea,blockquote,p,img{padding:0; margin:0;}
img{vertical-align:top; border:none;}
button,select,textarea{outline:none}
figure,form,fieldset{border:0;margin:0;padding:0}
textarea{resize:none}
ul,li{list-style-type:none;}
textarea:focus,input:focus{outline:none;}
table{border-collapse:collapse; border-spacing:0; empty-cells:show; }
a{color:#232323;text-decoration:none;}
a:hover{color:#000;text-decoration:none;}

b,strong{font-weight:normal;}
cite,em,i{font-style:normal;}

.c:after {content:""; display:block; height:0; clear:both;}
.c{*zoom:1;}


.banner-ul{display:block; margin:200px 0 0 650px;}
.banner-ul  li{float:left;border-right:1px solid #94c0be;}
.banner-ul li a{display: block;line-height:20px;font-size:20px; padding: 15px 30px 15px 31px;}
		
.a{perspective: 200px;position: relative;}
.a:hover .b, .b{transform: translateZ(-25px) rotateX(90deg);}
.b{transition: all .3s ease-out;transform: translatez(-25px);transform-style:preserve-3d;position: absolute;top: 0;
left: 0;display: block;width: 100%;height: 100%;}
		

		
.font{transform: rotatex(0deg) translatez(25px);}
.font1{transform: rotatex(-90deg) translatez(25px);color: #FFE7C4;}


.font, .font1{width: 100%;height: 100%;position: absolute;top:0; left:0; background:#74ADAA; padding: 15px 30px 15px 
31px;color: white;pointer-events: none;box-sizing: border-box;}
		
		
.banner-ul li a:hover .font1{background-color:#51938F;background-size: 10px 10px;}							
.banner-ul ul{position: absolute;text-align: left;line-height: 40px;font-size: 14px;width: 200px;transition: all 0.3s ease-in;transform-origin: 0px 0px;transform: rotateX(-90deg);overflow: hidden;}	
.banner-ul li:hover ul{display: block;transform: rotateX(0deg);}
