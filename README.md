[README.md](https://github.com/user-attachments/files/31495877/README.md)
# birthday-website<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>下點小雨，也沒關係｜給你的生日旅行</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@400;500;600&family=Zen+Maru+Gothic:wght@400;500;700&display=swap');

*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{
  margin:0;background:#101518;color:#f5f2ec;
  font-family:"Zen Maru Gothic",sans-serif;line-height:1.9;
  overflow-x:hidden;
}
section{min-height:100vh;display:flex;align-items:center;justify-content:center;position:relative;padding:80px 22px}
.container{width:min(900px,100%);text-align:center;position:relative;z-index:2}
.serif{font-family:"Noto Serif TC",serif}
.small{font-size:13px;letter-spacing:.25em;opacity:.65}
h1{font-family:"Noto Serif TC",serif;font-weight:500;font-size:clamp(42px,9vw,92px);line-height:1.25;margin:18px 0}
h2{font-family:"Noto Serif TC",serif;font-weight:500;font-size:clamp(30px,6vw,54px);margin:15px 0 28px}
p{font-size:clamp(15px,2.3vw,19px);color:#d8dcda;margin:8px 0}
.btn{
  display:inline-block;margin-top:38px;padding:13px 28px;border:1px solid rgba(255,255,255,.35);
  border-radius:999px;color:white;text-decoration:none;transition:.4s;background:rgba(255,255,255,.04)
}
.btn:hover{background:rgba(255,255,255,.12);transform:translateY(-2px)}
.hero{overflow:hidden;background:linear-gradient(#111a1d,#172225)}
.hero:after{
  content:"";position:absolute;inset:0;opacity:.18;
  background-image:radial-gradient(circle at 20% 30%,#fff 0 1px,transparent 2px),radial-gradient(circle at 70% 65%,#fff 0 1px,transparent 2px);
  background-size:80px 110px,120px 150px;animation:rain 1.2s linear infinite;
}
@keyframes rain{to{background-position:0 110px,0 150px}}
.scroll{position:absolute;bottom:28px;left:50%;transform:translateX(-50%);font-size:12px;letter-spacing:.25em;opacity:.5}
.fade{opacity:0;transform:translateY(24px);transition:1.1s ease}
.show .fade{opacity:1;transform:none}
.story{background:#202a2b}
.photo{
  width:min(760px,92vw);aspect-ratio:16/10;margin:35px auto;border-radius:22px;
  background:linear-gradient(135deg,#536263,#283436);
  display:flex;align-items:center;justify-content:center;overflow:hidden;
  box-shadow:0 20px 70px rgba(0,0,0,.25)
}
.photo span{opacity:.6;font-size:13px;letter-spacing:.15em}
.destination{background:#dfe3df;color:#243032}
.destination p{color:#566160}
.destination h1{color:#243032}
.card{
  background:rgba(255,255,255,.55);border:1px solid rgba(50,65,65,.12);
  border-radius:28px;padding:30px;margin:20px auto;width:min(720px,100%);
  box-shadow:0 20px 60px rgba(35,45,45,.08)
}
.info{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-top:25px}
.info div{padding:14px;border-radius:18px;background:rgba(255,255,255,.5)}
.info b{display:block;font-size:12px;letter-spacing:.15em;margin-bottom:4px}
.stay{background:#172224}
.dinner{background:#211e1b}
.final{background:radial-gradient(circle at 50% 45%,#3d4746,#111516 65%);min-height:110vh}
.final h2{font-size:clamp(32px,7vw,62px)}
.heart{font-size:34px;margin:22px}
.timeline{margin:35px auto;width:min(620px,100%);text-align:left}
.item{display:grid;grid-template-columns:90px 1fr;gap:20px;padding:20px 0;border-bottom:1px solid rgba(255,255,255,.12)}
.item .day{font-family:"Noto Serif TC";font-size:24px}
.item strong{font-size:18px;font-weight:500}
.footer{font-size:12px;opacity:.45;margin-top:55px}
@media(max-width:600px){.info{grid-template-columns:1fr}.item{grid-template-columns:70px 1fr}}
</style>
</head>
<body>

<section class="hero reveal">
  <div class="container">
    <div class="small fade">A BIRTHDAY TRIP FOR YOU</div>
    <h1 class="fade">下點小雨，<br>也沒關係。</h1>
    <p class="fade">與你 一起。</p>
    <a class="btn fade" href="#story">☂ 打開這份生日禮物</a>
  </div>
  <div class="scroll">SCROLL ↓</div>
</section>

<section id="story" class="story reveal">
  <div class="container">
    <div class="small fade">FOR MY FAVORITE PERSON</div>
    <h2 class="fade">我想送你的，<br>不是一個東西。</h2>
    <p class="fade">而是兩天一夜。</p>
    <p class="fade">不用趕著工作、<br>不用想太多事情。</p>
    <p class="fade">我們一起，離開日常一下。</p>
    <div class="photo fade"><span>📷 把你們最喜歡的合照放在這裡</span></div>
  </div>
</section>

<section class="destination reveal">
  <div class="container">
    <div class="small fade">DESTINATION REVEAL</div>
    <h2 class="fade">那麼，去哪裡？</h2>
    <p class="fade">一滴雨，是一個提示。</p>
    <div class="card fade">
      <h1>宜蘭</h1>
      <p>2 DAYS · 1 NIGHT</p>
      <div class="info">
        <div><b>WHEN</b>你的生日旅行</div>
        <div><b>STAY</b>小雨天 VILLA</div>
        <div><b>DINNER</b>小雨淋私廚</div>
      </div>
    </div>
  </div>
</section>

<section class="stay reveal">
  <div class="container">
    <div class="small fade">TONIGHT'S HOME</div>
    <h2 class="fade">今晚，這裡是我們的家。</h2>
    <p class="fade">我想讓你住一個<br>可以什麼都不用做的地方。</p>
    <div class="photo fade"><span>🏡 小雨天 VILLA｜可替換成住宿照片</span></div>
    <p class="fade">有田、有樹、有山。<br>還有一個晚上，時間只留給我們。</p>
    <a class="btn fade" href="https://www.twins-villa.com/" target="_blank" rel="noopener">看看我們今晚住的地方 ↗</a>
  </div>
</section>

<section class="dinner reveal">
  <div class="container">
    <div class="small fade">A DINNER FOR TWO</div>
    <h2 class="fade">還有一個晚上，<br>我偷偷留給你。</h2>
    <div class="card fade">
      <div class="small">DINNER</div>
      <h2>小雨淋私廚</h2>
      <p>不用趕著吃完，<br>不用趕著回家。</p>
      <p>就好好坐在一起，<br>吃一頓只屬於我們的晚餐。</p>
    </div>
  </div>
</section>

<section class="story reveal">
  <div class="container">
    <div class="small fade">OUR LITTLE TRIP</div>
    <h2 class="fade">兩天一夜，慢慢來。</h2>
    <div class="timeline fade">
      <div class="item"><div class="day">01</div><div><strong>出發</strong><br>一起去宜蘭，看看風景、吃點好吃的。</div></div>
      <div class="item"><div class="day">01</div><div><strong>入住</strong><br>把行李放下來，也把生活的忙碌放下來。</div></div>
      <div class="item"><div class="day">01</div><div><strong>生日晚餐</strong><br>小雨淋私廚，今晚只管好好陪彼此。</div></div>
      <div class="item"><div class="day">02</div><div><strong>睡到自然醒</strong><br>慢慢吃早餐，再一起走走。</div></div>
      <div class="item"><div class="day">02</div><div><strong>回家</strong><br>把兩天的回憶一起帶回去。</div></div>
    </div>
  </div>
</section>

<section class="final reveal">
  <div class="container">
    <div class="small fade">THE REAL GIFT</div>
    <h2 class="fade">其實我想送你的，<br>從來都不是宜蘭。</h2>
    <p class="fade">也不是民宿，也不是一頓飯。</p>
    <div class="heart fade">♡</div>
    <p class="fade">我想送你的，是我們的時間。</p>
    <p class="fade">是兩個人一起出發，<br>一起吃飯、一起看風景、一起回家的時間。</p>
    <br>
    <h2 class="fade">生日快樂，<br>我最愛的你。</h2>
    <p class="fade">希望這趟旅行結束以後，<br>我們還可以有很多很多個「一起出發吧」。</p>
    <a class="btn fade" href="#top" onclick="window.scrollTo({top:0,behavior:'smooth'});return false;">☂ 再看一次</a>
    <div class="footer fade">Made with love · just for you</div>
  </div>
</section>

<script>
const obs = new IntersectionObserver(entries=>{
  entries.forEach(e=>{ if(e.isIntersecting) e.target.classList.add('show'); });
},{threshold:.18});
document.querySelectorAll('.reveal').forEach(el=>obs.observe(el));
</script>
</body>
</html>
