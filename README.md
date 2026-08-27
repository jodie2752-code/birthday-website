<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>下點小雨，也沒關係 ☂️</title>

<style>

@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@400;500;600&family=Zen+Maru+Gothic:wght@400;500;700&display=swap');

*{
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    margin:0;
    background:#111718;
    color:#f7f4ee;
    font-family:"Zen Maru Gothic",sans-serif;
    line-height:1.9;
}

section{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    padding:80px 25px;
    position:relative;
    overflow:hidden;
}

.container{
    width:min(900px,100%);
    text-align:center;
    position:relative;
    z-index:2;
}

.serif{
    font-family:"Noto Serif TC",serif;
}

.small{
    font-size:12px;
    letter-spacing:.3em;
    opacity:.6;
}

h1,h2{
    font-family:"Noto Serif TC",serif;
    font-weight:500;
}

h1{
    font-size:clamp(45px,9vw,90px);
    line-height:1.3;
}

h2{
    font-size:clamp(32px,6vw,58px);
    line-height:1.4;
}

p{
    font-size:18px;
    color:#d9dedc;
}

.btn{
    display:inline-block;
    margin-top:35px;
    padding:13px 30px;
    border:1px solid rgba(255,255,255,.35);
    border-radius:999px;
    color:white;
    text-decoration:none;
    transition:.4s;
}

.btn:hover{
    background:rgba(255,255,255,.1);
    transform:translateY(-3px);
}

/* =========================
   第一幕
========================= */

.hero{
    background:
        linear-gradient(
            rgba(10,18,20,.7),
            rgba(10,18,20,.9)
        );
}

/* 雨 */

.rain{
    position:absolute;
    inset:0;
    pointer-events:none;
}

.drop{
    position:absolute;
    width:1px;
    height:80px;
    background:linear-gradient(
        transparent,
        rgba(255,255,255,.35)
    );
    animation:rain 1s linear infinite;
}

@keyframes rain{

    from{
        transform:translateY(-120px);
    }

    to{
        transform:translateY(110vh);
    }

}

/* =========================
   故事
========================= */

.story{
    background:#202a2a;
}

.destination{
    background:#e3e7e3;
    color:#263232;
}

.destination p{
    color:#596463;
}

.destination h1{
    color:#263232;
}

.card{
    background:rgba(255,255,255,.55);
    border-radius:30px;
    padding:35px;
    margin:30px auto;
    max-width:700px;
}

.info{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:12px;
    margin-top:25px;
}

.info div{
    padding:15px;
    border-radius:18px;
    background:rgba(255,255,255,.5);
}

.info b{
    display:block;
    font-size:11px;
    letter-spacing:.2em;
}

/* =========================
   照片
========================= */

.photo{
    width:min(750px,100%);
    aspect-ratio:16/10;
    margin:35px auto;
    border-radius:25px;
    overflow:hidden;
    background:#374444;
}

.photo img{
    width:100%;
    height:100%;
    object-fit:cover;
    display:block;
}

/* =========================
   住宿
========================= */

.stay{
    background:#172224;
}

/* =========================
   晚餐
========================= */

.dinner{
    background:#211e1b;
}

/* =========================
   行程
========================= */

.timeline{
    max-width:650px;
    margin:40px auto;
    text-align:left;
}

.item{
    display:grid;
    grid-template-columns:80px 1fr;
    gap:20px;
    padding:25px 0;
    border-bottom:1px solid rgba(255,255,255,.15);
}

.day{
    font-family:"Noto Serif TC";
    font-size:25px;
}

/* =========================
   最後
========================= */

.final{
    background:
        radial-gradient(
            circle at center,
            #3b4544,
            #101516 65%
        );
}

.heart{
    font-size:45px;
    margin:25px;
}

/* =========================
   動畫
========================= */

.reveal{
    opacity:0;
    transform:translateY(35px);
    transition:1s ease;
}

.reveal.show{
    opacity:1;
    transform:none;
}

/* =========================
   手機
========================= */

@media(max-width:600px){

    section{
        padding:70px 20px;
    }

    .info{
        grid-template-columns:1fr;
    }

    .item{
        grid-template-columns:60px 1fr;
    }

    p{
        font-size:16px;
    }

}

</style>
</head>


<body>


<!-- =========================
     第一幕
========================= -->

<section class="hero">

<div class="rain" id="rain"></div>

<div class="container">

<div class="small reveal">
A BIRTHDAY TRIP FOR YOU
</div>

<h1 class="reveal">
下點小雨，<br>
也沒關係。
</h1>

<p class="reveal">
因為這次，我想跟你一起出發。
</p>

<a href="#story" class="btn reveal">
☂ 打開這份生日禮物
</a>

</div>

</section>



<!-- =========================
     故事
========================= -->

<section id="story" class="story">

<div class="container">

<div class="small reveal">
FOR MY FAVORITE PERSON
</div>

<h2 class="reveal">
我想送你的，<br>
不是一個東西。
</h2>

<p class="reveal">
而是兩天一夜。
</p>

<p class="reveal">
不用趕著工作，<br>
不用想太多事情。
</p>

<p class="reveal">
就跟我一起，離開日常一下。
</p>


<div class="photo reveal">

<img src="images/photo01.jpg"
     alt="我們的照片">

</div>

</div>

</section>



<!-- =========================
     宜蘭揭曉
========================= -->

<section class="destination">

<div class="container">

<div class="small reveal">
DESTINATION REVEAL
</div>

<h2 class="reveal">
那麼，去哪裡？
</h2>

<p class="reveal">
一滴雨，是一個提示。
</p>


<div class="card reveal">

<h1>
宜蘭
</h1>

<p>
2 DAYS · 1 NIGHT
</p>


<div class="info">

<div>
<b>STAY</b>
小雨天 VILLA
</div>

<div>
<b>DINNER</b>
小雨淋私廚
</div>

<div>
<b>MOOD</b>
慢慢來
</div>

</div>

</div>

</div>

</section>



<!-- =========================
     住宿
========================= -->

<section class="stay">

<div class="container">

<div class="small reveal">
TONIGHT'S HOME
</div>

<h2 class="reveal">
今晚，這裡是我們的家。
</h2>

<p class="reveal">
我想讓你住一個<br>
可以什麼都不用做的地方。
</p>


<div class="photo reveal">

<img src="images/photo02.jpg"
     alt="小雨天 VILLA">

</div>


<p class="reveal">
有田、有樹、有山。<br>
還有一個晚上，時間只留給我們。
</p>


<a
href="https://www.twins-villa.com/"
target="_blank"
class="btn reveal">

看看我們今晚住的地方 ↗

</a>

</div>

</section>



<!-- =========================
     晚餐
========================= -->

<section class="dinner">

<div class="container">

<div class="small reveal">
A DINNER FOR TWO
</div>

<h2 class="reveal">
還有一個晚上，<br>
我偷偷留給你。
</h2>


<div class="card reveal">

<div class="small">
DINNER
</div>

<h2>
小雨淋私廚
</h2>

<p>
不用趕著吃完，<br>
不用趕著回家。
</p>

<p>
就好好坐在一起，<br>
吃一頓只屬於我們的晚餐。
</p>

</div>

</div>

</section>



<!-- =========================
     行程
========================= -->

<section class="story">

<div class="container">

<div class="small reveal">
OUR LITTLE TRIP
</div>

<h2 class="reveal">
兩天一夜，慢慢來。
</h2>


<div class="timeline">

<div class="item reveal">

<div class="day">
01
</div>

<div>
<strong>出發</strong><br>
一起去宜蘭，看看風景、吃點好吃的。
</div>

</div>


<div class="item reveal">

<div class="day">
01
</div>

<div>
<strong>入住</strong><br>
把行李放下來，也把生活的忙碌放下來。
</div>

</div>


<div class="item reveal">

<div class="day">
01
</div>

<div>
<strong>生日晚餐</strong><br>
小雨淋私廚，今晚只管好好陪彼此。
</div>

</div>


<div class="item reveal">

<div class="day">
02
</div>

<div>
<strong>睡到自然醒</strong><br>
慢慢吃早餐，再一起走走。
</div>

</div>


<div class="item reveal">

<div class="day">
02
</div>

<div>
<strong>回家</strong><br>
把兩天的回憶一起帶回去。
</div>

</div>

</div>

</div>

</section>



<!-- =========================
     最後
========================= -->

<section class="final">

<div class="container">

<div class="small reveal">
THE REAL GIFT
</div>


<h2 class="reveal">
其實我想送你的，<br>
從來都不是宜蘭。
</h2>


<p class="reveal">
也不是民宿，也不是一頓飯。
</p>


<div class="heart reveal">
♡
</div>


<p class="reveal">
我想送你的，是我們的時間。
</p>


<p class="reveal">
是兩個人一起出發，<br>
一起吃飯、一起看風景、一起回家的時間。
</p>


<br>


<h2 class="reveal">
生日快樂，<br>
我最愛的你。
</h2>


<p class="reveal">
希望這趟旅行結束以後，<br>
我們還可以有很多很多個「一起出發吧」。
</p>


<a href="#story" class="btn reveal">
☂ 再看一次
</a>

</div>

</section>



<script>

/* =========================
   產生雨滴
========================= */

const rain =
document.getElementById("rain");

for(let i=0;i<45;i++){

    const drop =
    document.createElement("div");

    drop.className="drop";

    drop.style.left =
    Math.random()*100+"%";

    drop.style.animationDelay =
    Math.random()*2+"s";

    drop.style.opacity =
    Math.random();

    rain.appendChild(drop);

}


/* =========================
   滑入動畫
========================= */

const observer =
new IntersectionObserver(
(entries)=>{

    entries.forEach(
    entry=>{

        if(entry.isIntersecting){

            entry.target
            .classList
            .add("show");

        }

    });

},
{
    threshold:.15
}
);


document
.querySelectorAll(".reveal")
.forEach(
el=>observer.observe(el)
);

</script>

</body>
</html>
