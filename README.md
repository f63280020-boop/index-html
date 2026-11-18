<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>For Asmaa 💗</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;700;800&family=Playfair+Display:ital,wght@1,600&display=swap');

* {box-sizing:border-box;margin:0;padding:0}

body {
 min-height:100vh;
 background:linear-gradient(135deg,#ffe5ef,#eee2ff,#e1f5ff);
 font-family:Cairo,sans-serif;
 display:flex;
 justify-content:center;
 align-items:center;
 padding:20px;
 color:#856b91;
 overflow-x:hidden;
}

#sky {
 position:fixed;
 inset:0;
 overflow:hidden;
 pointer-events:none;
}

.float {
 position:absolute;
 bottom:-40px;
 animation:up 8s linear forwards;
}

@keyframes up {
 0% {transform:translateY(0) rotate(0);opacity:0}
 20% {opacity:.8}
 100% {transform:translateY(-110vh) rotate(360deg);opacity:0}
}

.container {
 width:100%;
 max-width:420px;
 text-align:center;
 position:relative;
 z-index:2;
}

.top {
 font-family:'Playfair Display',serif;
 letter-spacing:3px;
 color:#b18bbd;
 font-size:16px;
}

h1 {
 color:#b078a9;
 font-size:43px;
 margin:10px 0;
}

.subtitle {
 font-size:14px;
 color:#9e83a9;
 margin-bottom:20px;
}

.bouquet {
 font-size:45px;
 animation:sway 3s infinite;
}

@keyframes sway {
 50% {transform:rotate(8deg) scale(1.08)}
}

.envelope-area {
 height:205px;
 display:flex;
 align-items:center;
 justify-content:center;
}

.envelope {
 width:225px;
 height:140px;
 background:#e8b9df;
 position:relative;
 border-radius:9px;
 cursor:pointer;
 box-shadow:0 15px 35px #a981b755;
}

.envelope:before {
 content:"";
 position:absolute;
 inset:0;
 background:#f5d5ed;
 clip-path:polygon(0 0,50% 60%,100% 0);
 z-index:4;
 transform-origin:top;
 transition:.7s;
}

.envelope:after {
 content:"";
 position:absolute;
 inset:0;
 background:#d8a8d6;
 clip-path:polygon(0 100%,50% 43%,100% 100%);
 z-index:3;
}

.letter {
 position:absolute;
 width:185px;
 height:125px;
 left:20px;
 bottom:8px;
 background:#fffafd;
 border-radius:8px;
 z-index:2;
 display:flex;
 flex-direction:column;
 justify-content:center;
 align-items:center;
 transition:.8s;
}

.letter span {font-size:35px}

.seal {
 position:absolute;
 top:50px;
 left:95px;
 font-size:32px;
 z-index:5;
 transition:.4s;
}

.envelope.open:before {
 transform:rotateX(180deg);
}

.envelope.open .letter {
 transform:translateY(-105px);
}

.envelope.open .seal {opacity:0}

.hint {
 color:#a587b1;
 font-size:13px;
 animation:blink 1.5s infinite;
}

@keyframes blink {
 50% {opacity:.4}
}

.card {
 display:none;
 background:rgba(255,255,255,.85);
 border:1px solid white;
 border-radius:28px;
 padding:28px 20px;
 box-shadow:0 15px 40px #a98bb644;
 animation:show .8s;
}

@keyframes show {
 from {opacity:0;transform:translateY(25px)}
 to {opacity:1;transform:translateY(0)}
}

.card h2 {
 color:#b078a9;
 font-size:25px;
 margin:12px 0;
}

.heart {
 font-size:50px;
 animation:beat 1.4s infinite;
}

@keyframes beat {
 50% {transform:scale(1.2)}
}

.line {
 width:60px;
 height:2px;
 background:#e6b6dc;
 margin:15px auto;
}

.message {
 line-height:2.3;
 font-size:15px;
 color:#806d91;
}

button {
 border:0;
 border-radius:30px;
 padding:13px 24px;
 background:linear-gradient(120deg,#c59cda,#f0b5d4);
 color:white;
 font-family:Cairo;
 font-size:14px;
 font-weight:bold;
 margin-top:20px;
 cursor:pointer;
}

.extra {
 display:none;
 margin-top:20px;
 line-height:2.2;
 color:#a276aa;
 animation:show .7s;
}

.footer {
 margin-top:25px;
 font-family:'Playfair Display',serif;
 font-size:12px;
 letter-spacing:2px;
 color:#b49bbd;
}
</style>
</head>

<body>

<div id="sky"></div>

<div class="container">

 <div class="top">A SPECIAL GIFT FOR YOU</div>

 <div class="bouquet">🌷🦋🌷</div>

 <h1>Asmaa</h1>

 <div class="subtitle">
  في حاجة صغيرة معمولة مخصوص ليكي ♡
 </div>

 <div class="envelope-area" id="envelopeArea">
  <div class="envelope" id="envelope" onclick="openGift()">

   <div class="letter">
    <span>💌</span>
    <small style="color:#ad83b3">For my lovely friend</small>
   </div>

   <div class="seal">💗</div>

  </div>
 </div>

 <div class="hint" id="hint">
  دوسي على الظرف وافتحي هديتك 🥹
 </div>

 <div class="card" id="card">

  <div class="heart">💗</div>

  <h2>إلى أسماء الجميلة 🌸</h2>

  <div class="line"></div>

  <div class="message">
   في ناس وجودها بيخلي الأيام أحلى،<br>
   وبيسيبوا في القلب ذكريات جميلة ✨<br><br>

   حبيت أعملك حاجة مختلفة وصغيرة،<br>
   تفكرك إنك تستاهلي كل حاجة حلوة.<br><br>

   أتمنى أشوفك دايمًا مبسوطة،<br>
   وناجحة، وضحكتك منورة الدنيا 🌷<br><br>

   ربنا يحققلك كل أحلامك يا أسماء 🦋
  </div>

  <button onclick="showExtra()">
   اضغطي هنا للمفاجأة 👀
  </button>

  <div class="extra" id="extra">
   <div style="font-size:40px">🎀🌸✨</div>
   خلي قلبك دايمًا مليان فرحة،<br>
   وأيامك كلها ورد وسعادة.<br><br>
   <strong>You're one of a kind, Asmaa! 💗</strong>
  </div>

 </div>

 <div class="footer">
  MADE WITH LOVE ♡
 </div>

</div>

<script>
const sky=document.getElementById("sky");
const symbols=["🌸","💕","✨","🦋","🌷","♡"];

function createFloat(){
 const el=document.createElement("div");
 el.className="float";
 el.textContent=symbols[Math.floor(Math.random()*symbols.length)];
 el.style.left=Math.random()*100+"%";
 el.style.fontSize=(15+Math.random()*18)+"px";
 el.style.animationDuration=(6+Math.random()*6)+"s";
 sky.appendChild(el);
 setTimeout(()=>el.remove(),13000);
}

setInterval(createFloat,450);

let opened=false;

function openGift(){
 if(opened)return;
 opened=true;

 document.getElementById("envelope").classList.add("open");

 setTimeout(()=>{
  document.getElementById("envelopeArea").style.display="none";
  document.getElementById("hint").style.display="none";
  document.getElementById("card").style.display="block";
 },1000);
}

function showExtra(){
 document.getElementById("extra").style.display="block";

 for(let i=0;i<25;i++){
  setTimeout(createFloat,i*100);
 }
}
</script>

</body>
</html>
