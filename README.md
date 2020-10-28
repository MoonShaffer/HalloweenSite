# HalloweenSite

<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<link rel="stylesheet" href="css/normalize.css">
<link rel="stylesheet" href="css/style.css">
<meta name="keywords" content="Halloween、pumpkin、ハロウィーン、ハロウィン、
ジャックオランタン、かぼちゃ、カボチャ、南瓜、パンプキン、jacko'lantern、
trick or treat、トリックオアトリート、コウモリ、魔女、ゴースト、witch、ghost、bat" />
<meta name="description" content="ハロウィンをより楽しむための情報が満載！
オシャレでかわいいハロウィングッズやフード情報などを紹介しています！" />
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>YOLO YOLO Halloween</title>
<link rel="stylesheet" type="text/css" href="css/slick.css" media="screen"/>
<link rel="stylesheet" type="text/css" href="css/slick-theme.css" media="screen"/>

</head>

<body onload="init();">
    <header>
        <div id="menuWrapper">
            <a class="trigger" href="#">
                <span></span>
                <span></span>
                <span></span>
            </a>
        </div>
        <nav>
            <ul>
                <li><a href="#abouthalloween">About Halloween</a></li>
                <li><a href="#goods">Halloween Goods</a></li>
                <li><a href="#foods">Halloween Foods</a></li>
            </ul>
        </nav>
        <div class="contentWrapper">
        <h1>コロナでもハロウィンを楽しもう</h1>
        <a href="index.html"><img src="img/halloweentitle.png" 
        alt="YOLO YOLO Halloween"></a>
        </div>
    </header>
    <section id="abouthalloween">
    <div class="contentWrapper">
        <h2>About Halloween</h2>
        <p>ハロウィンとは、万聖節（ばんせいせつ）（11月1日）の前夜祭のこと。<br>
        古代ケルト起源で，秋の収穫を祝い悪霊を追い出すための祭りです。<br>
        カボチャをくりぬき目鼻口をつけた『ジャックオランタン』という提灯を飾り，<br>
        お化けの仮装をした子供たちが 
        「Trick or treat!(ごちそうくれなきゃイタズラするぞ)」<br>
        と言いながら近所を回り、お菓子もらうのが恒例となっています。</p>
        <div class="flex">
            <div class="flexcontent">
                <figure>
                    <img src="img/pumpkin.jpg">
                    <figcaption>オリジナリティ溢れるジャックオランタン</figcaption>
                </figure>
            </div>
            <div class="flexcontent">
                <figure>
                    <img src="img/trickortreat.jpg">
                    <figcaption>近所を回り、お菓子をもらう子供たち</figcaption>
                </figure>
            </div>
            <div class="flexcontent">
                <figure>
                    <img src="img/dollandpumpkin.jpg">
                    <figcaption>ハロウィン仕様のカカシ</figcaption>
                </figure>
            </div>
        </div>
    </div>
    </section>
    <section id="goods">
    <div class="contentWrapper">
        <h2>Halloween Goods</h2>
        <ul class="slider">
            <li><img src="img/ghostlamp.jpg"></li>
            <li><img src="img/halloweencat.jpg"></li>
            <li><img src="img/threeghost.jpg"></li>
            <li><img src="img/witch.jpg"></li>
            <li><img src="img/halloweenplate.jpg"></li>
        </ul>
        <p>飾るだけでハロウィン気分が楽しめるグッズが勢揃い</p>  
    </div>
    </section>  

    <section id="foods">
        <div class="contentWrapper">
        <h2>Halloween Foods</h2>
        <ul class="slider">
            <li><img src="img/halloweencafee.jpg"></li>
            <li><img src="img/pumpkinsoup.jpg"></li>
            <li><img src="img/pumpkinspicelatte.jpg"></li>
            <li><img src="img/pumpkinpie.jpg"></li>
            <li><img src="img/jacksweet.jpg"></li>
        </ul>
        <p>カボチャを贅沢に使ったハロウィン料理</p>
    </div>
    </section>

    <footer>
        <div id="upperFooter">
            <nav>
                <ul class="flex">
                    <li><a href="#abouthalloween">About Halloween</a></li>
                    <li><a href="#goods">Halloween Goods</a></li>
                    <li><a href="#foods">Halloween Foods</a></li>
                </ul>
            </nav>
        </div>
        <div id="bottomFooter">
            <small>copyright©︎YOLO YOLO Halloween, Inc. 
            All Rights Reserved.</small>
        </div>
    </footer>
    <script src="http://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="js/slick.min.js"></script>
    <script>
        $(function() {
            var windowWidth = $(window).width();
            var nos = 0;
            if(windowWidth > 800) {
            nos = 2;
            } else {
            nos = 1;
            }
            $('.slider').slick({
                infinite : true,
                dots : true,
                slidesToShow : nos,
                autoplay : true,
                initialSlide : 1,
                arrows : false,
            });
            $(".trigger").click(function () {
                $(this).toggleClass("active");
                $("header nav").toggleClass("onanimation");
            });
            $('header nav li').click(function() {
                $(".trigger").removeClass("active");
                $("header nav").toggleClass("onanimation");
            });
        });
    </script>
</body>
</html>
    

