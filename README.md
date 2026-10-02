# For-my-Kyuuutuu
💗 A little corner of the internet made with love, especially for my Kyuutu, Anuska. 🎀✨ A place filled with our memories, cute surprises, and all the little things that remind me of you. Happy Birthday, my girl! 🎂💕 You deserve all the happiness in the world. 🌷🫶🏻

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#ffe6f0">
<title>For My Kyuutu 💗</title>
<style>
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{
  margin:0;
  color:#71334f;
  font-family:Georgia,serif;
  text-align:center;
  background:
    radial-gradient(ellipse at 10% 10%,#fff 0%,transparent 35%),
    radial-gradient(ellipse at 90% 25%,#ffd5e6 0%,transparent 40%),
    linear-gradient(160deg,#fff0f6,#ffe0ed,#fff7fb);
  background-attachment:fixed;
  overflow-x:hidden;
}
section{padding:65px 18px}
.hero{
  min-height:100svh;
  display:flex;
  flex-direction:column;
  align-items:center;
  justify-content:center;
  position:relative;
  padding:35px 22px;
  overflow:hidden;
}
.hero:before,.hero:after{
  content:"♡";
  position:absolute;
  color:#f2a9c8;
  opacity:.28;
  font-size:220px;
  pointer-events:none;
}
.hero:before{left:-65px;top:10%;transform:rotate(-20deg)}
.hero:after{right:-65px;bottom:5%;transform:rotate(20deg)}
.hero>*{position:relative;z-index:1}
.eyebrow{letter-spacing:3px;font-size:11px}
h1{font-size:clamp(42px,11vw,66px);margin:14px 0;color:#9b456d}
h2{font-size:30px}
p{line-height:1.8}
button{
  background:#a84976;color:white;border:0;border-radius:30px;
  padding:14px 22px;font:inherit;font-size:15px;
  box-shadow:0 8px 22px #a8497630;margin:8px 0;
  cursor:pointer;
}
button:active{transform:scale(.97)}
.soft{background:#f7cddd;color:#773a59}
.icon{font-size:65px;animation:float 3s ease-in-out infinite}
.card{
  background:#ffffffc9;border:1px solid #f5bfd5;
  border-radius:25px;padding:24px;margin:22px auto;
  max-width:520px;box-shadow:0 12px 35px #a8497615;
}
.hidden{display:none!important}
.gallery{
  max-width:720px;margin:25px auto;
  display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px;
}
.polaroid{
  background:#fff;padding:8px 8px 14px;
  border-radius:9px;box-shadow:0 6px 20px #9d54701c;
  transform:rotate(-2deg);
}
.polaroid:nth-child(even){transform:rotate(2deg)}
.polaroid img{
  display:block;width:100%;aspect-ratio:4/5;object-fit:cover;
  background:#f9dbe8;border-radius:5px;
}
.polaroid p{font-size:13px;margin:9px 0 0}
#letter{white-space:pre-line;text-align:left;line-height:2}
.cake{font-size:85px;margin:15px}
footer{padding:35px 15px}
.heart{
  position:fixed;bottom:-35px;z-index:10;pointer-events:none;
  animation:rise 5s linear forwards;
}
@keyframes rise{
  to{transform:translateY(-110vh) rotate(30deg);opacity:0}
}
@keyframes float{50%{transform:translateY(-12px) rotate(4deg)}}
@media(prefers-reduced-motion:reduce){
  *,*:before,*:after{animation:none!important;scroll-behavior:auto!important}
}
</style>
</head>
<body>

<section class="hero" id="home">
  <div class="icon">💌</div>
  <p class="eyebrow">A LITTLE SURPRISE MADE WITH LOVE</p>
  <h1>For my<br>Kyuutu ♡</h1>
  <p>This little world is just for you, Anuska.<br>
  Open it slowly, beautiful soul. 🌸</p>
  <button onclick="startSurprise()">Open your surprise 💗</button>
  <p style="font-size:12px">Made by Biraja, especially for you ♡</p>
</section>

<section id="birthday">
  <p class="eyebrow">YOUR SPECIAL DAY · 5 OCTOBER</p>
  <h2>Happy Birthday, Anuska! 🎂</h2>
  <p>Today deserves a little extra magic, a lot of smiles,
  and all the happiness life can bring you.</p>
  <div class="card">
    <div style="font-size:38px">🌷 💗 🌷</div>
    <p>To my favourite Kyuutu,<br>
    I hope you feel celebrated today and every day.</p>
    <button onclick="openLetter()">Open your letter 💌</button>
    <div id="letterBox" class="hidden">
      <hr style="border:0;border-top:1px solid #f1c2d6">
      <h2>Dear Kyuutu ♡</h2>
      <p id="letter"></p>
      <p style="text-align:right">With love,<br>Biraja ♡</p>
    </div>
  </div>
</section>

<section id="memories">
  <p class="eyebrow">OUR LITTLE MEMORY BOOK</p>
  <h2>Moments to keep 📸</h2>
  <p>Four little windows into your favourite memories.</p>
  <div class="gallery">
    <div class="polaroid">
      <img src="photo1.jpg" alt="Memory one">
      <p>One of my favourite moments ♡</p>
    </div>
    <div class="polaroid">
      <img src="photo2.jpg" alt="Memory two">
      <p>A little moment of happiness 🌸</p>
    </div>
    <div class="polaroid">
      <img src="photo3.jpg" alt="Memory three">
      <p>Something worth remembering 💗</p>
    </div>
    <div class="polaroid">
      <img src="photo4.jpg" alt="Memory four">
      <p>More beautiful days ahead ✨</p>
    </div>
  </div>
</section>

<section id="cake">
  <p class="eyebrow">CLOSE YOUR EYES AND WISH</p>
  <h2>A little birthday cake 🎂</h2>
  <div class="cake" id="cakeEmoji">🎂</div>
  <p id="wishText">Ready to make a birthday wish?</p>
  <button onclick="makeWish()">Make a wish ✨</button>
</section>

<section>
  <div class="card">
    <p class="eyebrow">ONE LAST SURPRISE</p>
    <h2>For you, always ♡</h2>
    <p>May your next chapter bring peaceful days, lovely
    surprises, new adventures, and endless reasons to smile.</p>
    <button onclick="finalSurprise()">One last thing 💝</button>
    <div id="finalBox" class="hidden">
      <h2>You are so special! 🌸</h2>
      <p>Happy Birthday, Anuska. I hope this tiny gift
      brings a smile to your face whenever you see it.</p>
      <div style="font-size:35px">💗 🌷 💗</div>
    </div>
  </div>
</section>

<section>
  <h2>A little music 🎵</h2>
  <p>Press play whenever you want a soundtrack.</p>
  <audio controls loop preload="none" style="max-width:100%">
    <source src="song.mp3" type="audio/mpeg">
  </audio>
  <p style="font-size:12px">Music is optional. Press play to start.</p>
</section>

<footer>
  Made with love for Anuska ♡<br>
  <span style="font-size:13px">From Biraja · 5 October 2026 🌸</span>
</footer>

<script>
const letterText = `Happy Birthday, my Kyuutu! ♡

I made this little corner of the internet just for you.

I hope your days are filled with happiness, your dreams keep growing, and you always find reasons to smile.

Thank you for being part of my life and for all the little moments that make life feel special.

May this new year bring you beautiful memories, peaceful days, and lots of love.

Enjoy your special day, Anuska. You deserve to feel celebrated today and always.

Happy Birthday once again! 🌸💗`;

function hearts(n){
  const symbols=["♡","💗","💕","🌸","✨"];
  for(let i=0;i<n;i++){
    const el=document.createElement("span");
    el.className="heart";
    el.textContent=symbols[Math.floor(Math.random()*symbols.length)];
    el.style.left=Math.random()*100+"vw";
    el.style.fontSize=(17+Math.random()*20)+"px";
    el.style.animationDelay=Math.random()+"s";
    document.body.appendChild(el);
    setTimeout(()=>el.remove(),6000);
  }
}
function startSurprise(){
  hearts(22);
  document.getElementById("birthday").scrollIntoView({behavior:"smooth"});
}
function openLetter(){
  document.getElementById("letterBox").classList.remove("hidden");
  document.getElementById("letter").textContent=letterText;
  hearts(15);
}
let wished=false;
function makeWish(){
  document.getElementById("cakeEmoji").textContent=wished?"🎂":"🎂✨";
  document.getElementById("wishText").textContent=wished
    ?"Your cake is ready for another wish! 🌸"
    :"Wish made! May beautiful things find their way to you. 💗";
  wished=!wished;
  hearts(25);
}
function finalSurprise(){
  document.getElementById("finalBox").classList.remove("hidden");
  hearts(30);
}
</script>
</body>
</html>
