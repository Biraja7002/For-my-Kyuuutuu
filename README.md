
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#ffe4ef">
<title>For My Kyuutu ♡</title>
<style>
:root {
  --pink: #ec75a9;
  --deep: #b83270;
  --light: #fff4f8;
  --ink: #703650;
  --card: rgba(255,255,255,.78);
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; scroll-padding-top: 78px; }
body {
  margin: 0;
  color: var(--ink);
  font-family: Georgia, "Times New Roman", serif;
  background:
    radial-gradient(ellipse at 10% 5%, #fff 0, transparent 34%),
    radial-gradient(ellipse at 95% 30%, #ffc9df 0, transparent 38%),
    linear-gradient(150deg,#fff5fa,#ffe1ed 48%,#fff8fb);
  overflow-x: hidden;
}
button, a { -webkit-tap-highlight-color: transparent; }
button { font: inherit; }
a { color: inherit; text-decoration: none; }
nav {
  position: sticky; top: 0; z-index: 10;
  display: flex; justify-content: space-between; align-items: center;
  gap: 10px; padding: 13px 5%;
  background: rgba(255,245,250,.88);
  backdrop-filter: blur(14px);
  border-bottom: 1px solid #fff;
}
.logo { color: var(--deep); font-size: 1.15rem; font-weight: bold; }
.navlinks { display:flex; gap: 15px; font: 12px Arial,sans-serif; }
.navlinks a:hover { color: var(--deep); }
section { padding: 74px 6%; }
.hero {
  min-height: 88vh; display: flex; flex-direction: column;
  justify-content: center; align-items: center; text-align: center;
  position: relative; padding-top: 65px;
}
.eyebrow {
  text-transform: uppercase; letter-spacing: 3px;
  font: 11px Arial,sans-serif; color: var(--deep);
}
h1 { font-size: clamp(3.1rem,12vw,6.5rem); line-height: .98;
  margin: 22px 0; color: var(--deep); font-weight: normal; }
h1 span { font-style: italic; color: #e36da1; }
h2 { font-size: clamp(2rem,7vw,3.4rem); font-weight: normal;
  color: var(--deep); margin: 12px 0 18px; }
h3 { color: var(--deep); }
p { line-height: 1.8; }
.subtitle { max-width: 510px; font-size: 1.05rem; }
.btn {
  display: inline-flex; justify-content:center; align-items:center;
  gap: 8px; border: 0; border-radius: 40px; padding: 14px 23px;
  background: linear-gradient(135deg,#ed83b2,#cf4f8d);
  color: white; box-shadow: 0 9px 24px #d65b912e;
  cursor: pointer; transition: transform .2s, box-shadow .2s;
}
.btn:hover { transform: translateY(-3px); box-shadow: 0 12px 30px #d65b9145; }
.btn.secondary { background: white; color: var(--deep); border: 1px solid #f4b8d1; }
.hero-heart { font-size: 4rem; animation: pulse 1.8s infinite; margin-top: 18px; }
@keyframes pulse { 50% { transform: scale(1.13); } }
@keyframes floatUp {
  0% { transform: translateY(0) rotate(0); opacity: 0; }
  15% { opacity: .8; }
  100% { transform: translateY(-110vh) rotate(35deg); opacity: 0; }
}
.float-heart {
  position: fixed; bottom: -35px; pointer-events: none; z-index: 1;
  animation: floatUp linear forwards; color: #e96ca3;
}
section { position: relative; }
.section-head { text-align:center; max-width:650px; margin:0 auto 35px; }
.section-head p { margin:0 auto; max-width:530px; }
.card {
  background: var(--card); border: 1px solid #fff;
  border-radius: 25px; padding: 24px;
  box-shadow: 0 12px 38px #ac47751a;
  backdrop-filter: blur(10px);
}
.countdown { display:grid; grid-template-columns:repeat(4,1fr); gap:10px; max-width:560px; margin:28px auto; }
.countbox { padding:18px 5px; text-align:center; border-radius:18px;
  background:#fff9fc; border:1px solid #f8c9dd; }
.countbox strong { display:block; font-size:clamp(1.5rem,6vw,2.6rem); color:var(--deep); }
.countbox small { font:10px Arial,sans-serif; letter-spacing:1px; }
.center { text-align:center; }
.gallery { display:grid; grid-template-columns:repeat(2,minmax(0,1fr)); gap:15px; }
.photo {
  padding:9px 9px 16px; background:#fff; border-radius:7px;
  box-shadow:0 8px 24px #8e3d621b; transform:rotate(-1deg);
}
.photo:nth-child(even) { transform:rotate(1.5deg); }
.photo img { display:block; width:100%; aspect-ratio:4/5; object-fit:cover;
  background:linear-gradient(140deg,#ffe0ed,#fff4f8); border-radius:3px; }
.photo p { margin:10px 2px 0; text-align:center; font-style:italic; font-size:.95rem; }
.note { text-align:center; margin-top:20px; font:12px Arial,sans-serif; opacity:.8; }
.letter-wrap { max-width:650px; margin:auto; text-align:center; }
.envelope {
  width:min(280px,85%); height:180px; margin:35px auto 25px;
  background:#f6a8c9; border-radius:12px; position:relative;
  cursor:pointer; display:grid; place-items:center;
  box-shadow:0 15px 35px #a73c7025; overflow:hidden;
}
.envelope:before {
  content:""; position:absolute; inset:0;
  background:#ef8db8; clip-path:polygon(0 0,50% 58%,100% 0);
}
.envelope .seal { z-index:1; font-size:2.6rem; transition:.3s; }
.envelope.open .seal { transform:scale(1.3); }
.letter {
  display:none; text-align:left; background:#fffdfb; border:1px solid #f5d8e4;
  padding:clamp(22px,6vw,40px); border-radius:15px;
  box-shadow:0 12px 30px #9f45671a; white-space:pre-line;
  line-height:1.9;
}
.letter.show { display:block; animation: appear .65s ease both; }
@keyframes appear { from {opacity:0;transform:translateY(12px)} to {opacity:1;transform:none} }
.reasons { display:grid; grid-template-columns:repeat(2,minmax(0,1fr)); gap:13px; }
.reason {
  min-height:135px; border:1px solid #fff; background:#ffffffbd;
  border-radius:20px; padding:18px 13px; color:var(--ink); cursor:pointer;
  box-shadow:0 8px 25px #a94c7310; transition:transform .2s;
}
.reason:hover { transform:translateY(-3px); }
.reason .emoji { display:block; font-size:1.8rem; margin-bottom:9px; }
.reason .answer { display:none; font-size:.92rem; line-height:1.6; }
.reason.revealed .prompt { display:none; }
.reason.revealed .answer { display:block; animation:appear .3s ease; }
.secret { max-width:570px; margin:auto; text-align:center; }
.gift {
  font-size:5rem; display:block; margin:20px auto;
  background:none; border:0; cursor:pointer; transition:transform .3s;
}
.gift:hover { transform:rotate(-8deg) scale(1.1); }
.secret-message { display:none; }
.secret-message.show { display:block; animation:appear .6s ease both; }
.music { max-width:520px; margin:auto; text-align:center; }
audio { width:100%; margin:12px 0; }
.music-hint { font:12px Arial,sans-serif; opacity:.8; }
footer { padding:40px 20px 55px; text-align:center; background:#ffffff62; }
footer .heart { color:var(--deep); font-size:1.6rem; }
.small { font:12px Arial,sans-serif; opacity:.8; }
.divider { color:#dc75a0; letter-spacing:8px; margin:25px 0; }
@media (min-width:700px) {
  .gallery { grid-template-columns:repeat(4,minmax(0,1fr)); }
  .reasons { grid-template-columns:repeat(3,minmax(0,1fr)); }
  section { padding:90px 9%; }
}
@media (max-width:390px) {
  .navlinks { gap:9px; font-size:10px; }
  .logo { font-size:1rem; }
  section { padding:60px 5%; }
  .card { padding:18px; }
}
@media (prefers-reduced-motion: reduce) {
  *, *:before, *:after { animation-duration:.01ms !important; scroll-behavior:auto !important; }
}
</style>
</head>
<body>

<nav>
  <a class="logo" href="#home">♡ For Kyuutu</a>
  <div class="navlinks">
    <a href="#countdown">Birthday</a>
    <a href="#memories">Memories</a>
    <a href="#letter">My letter</a>
    <a href="#surprise">Surprise</a>
  </div>
</nav>

<main>
<section class="hero" id="home">
  <p class="eyebrow">A tiny website, a very big feeling</p>
  <h1>For my<br><span>Kyuutu</span> ♡</h1>
  <p class="subtitle">
    For Anuska — the girl who deserves her own little world
    full of love, happiness, and beautiful surprises.
  </p>
  <div class="hero-heart">💗</div>
  <p>Made with love, by Biraja</p>
  <a class="btn" href="#countdown">Your little surprise ↓</a>
  <p class="small">Scroll slowly… there's more for you 🌷</p>
</section>

<section id="countdown">
  <div class="section-head">
    <p class="eyebrow">Save this little date</p>
    <h2>It's your day, Kyuutu 🎂</h2>
    <p>October 5 is a little more special because the world got you.</p>
  </div>
  <div class="card center">
    <p id="countLabel">Counting down to your special day…</p>
    <div class="countdown" id="countdownBoxes">
      <div class="countbox"><strong id="days">--</strong><small>DAYS</small></div>
      <div class="countbox"><strong id="hours">--</strong><small>HOURS</small></div>
      <div class="countbox"><strong id="minutes">--</strong><small>MINUTES</small></div>
      <div class="countbox"><strong id="seconds">--</strong><small>SECONDS</small></div>
    </div>
    <p id="birthdayLine">Until we celebrate you, my girl. 💕</p>
  </div>
</section>

<section id="memories">
  <div class="section-head">
    <p class="eyebrow">Little moments, big feelings</p>
    <h2>Our memory corner 📸</h2>
    <p>Every picture has a story. These spaces are waiting for your favourite memories.</p>
  </div>
  <div class="gallery">
    <div class="photo">
      <img src="photo1.jpg" alt="Our favourite memory 1" loading="lazy">
      <p>One of my favourite moments ♡</p>
    </div>
    <div class="photo">
      <img src="photo2.jpg" alt="Our favourite memory 2" loading="lazy">
      <p>A little memory to keep 🌷</p>
    </div>
    <div class="photo">
      <img src="photo3.jpg" alt="Our favourite memory 3" loading="lazy">
      <p>You make moments special ✨</p>
    </div>
    <div class="photo">
      <img src="photo4.jpg" alt="Our favourite memory 4" loading="lazy">
      <p>And many more to come 💗</p>
    </div>
  </div>
  <p class="note">Add your own photos named photo1.jpg, photo2.jpg, photo3.jpg and photo4.jpg.</p>
</section>

<section id="letter">
  <div class="section-head">
    <p class="eyebrow">Just between us</p>
    <h2>A little letter for you 💌</h2>
    <p>There's something I'd love you to read.</p>
  </div>
  <div class="letter-wrap">
    <button class="envelope" id="envelope" aria-label="Open the birthday letter">
      <span class="seal">💌</span>
    </button>
    <p class="small" id="openHint">Tap the envelope to open your letter</p>
    <article class="letter" id="letterContent">
      <h3>To my Kyuutu, Anuska ♡</h3>
      Happy Birthday, my girl! 🎂💗

      I don't know if words will ever be enough to explain how special you are to me, but today I want to try.

      Thank you for being you — for your little ways, your smile, and the moments that become beautiful simply because you're part of them. Even the smallest conversations with you can mean more to me than you might realise.

      I hope this new year of your life brings you peace, laughter, new dreams, and countless reasons to smile. I hope you always remember how much you matter and how deserving you are of good things.

      I can't promise that every day will be perfect, but I hope we keep choosing kindness, honesty, understanding, and making lovely memories together.

      This little website is just a small gift, made with a lot of thought and love, to remind you that someone is celebrating the wonderful person you are.

      Keep smiling, keep dreaming, and keep being your adorable self.

      Happy Birthday once again, Kyuutu. 🌷

      With lots of love,
      Your Biraja ♡
    </article>
  </div>
</section>

<section id="reasons">
  <div class="section-head">
    <p class="eyebrow">A few little reminders</p>
    <h2>Why you're so special 💕</h2>
    <p>Tap each card to reveal a little reminder. You can change these messages to your own words.</p>
  </div>
  <div class="reasons">
    <button class="reason">
      <span class="emoji">🌸</span><span class="prompt">Reason one…</span>
      <span class="answer">Your unique way of being yourself is something I truly appreciate.</span>
    </button>
    <button class="reason">
      <span class="emoji">😊</span><span class="prompt">Reason two…</span>
      <span class="answer">Your smile can turn an ordinary moment into a lovely memory.</span>
    </button>
    <button class="reason">
      <span class="emoji">🫶</span><span class="prompt">Reason three…</span>
      <span class="answer">I value the comfort and trust we can build by being honest with each other.</span>
    </button>
    <button class="reason">
      <span class="emoji">✨</span><span class="prompt">Reason four…</span>
      <span class="answer">You have your own little magic, and you don't need to be anyone else.</span>
    </button>
    <button class="reason">
      <span class="emoji">🌷</span><span class="prompt">Reason five…</span>
      <span class="answer">I love learning the little things that make you happy.</span>
    </button>
    <button class="reason">
      <span class="emoji">💗</span><span class="prompt">One last reason…</span>
      <span class="answer">Because being you is already special. You never need to prove your worth.</span>
    </button>
  </div>
</section>

<section id="music">
  <div class="section-head">
    <p class="eyebrow">Press play, if you like</p>
    <h2>A song for my girl 🎶</h2>
    <p>A little soundtrack for your little corner of the internet.</p>
  </div>
  <div class="card music">
    <div style="font-size:2.8rem">🎧💗🎵</div>
    <p><strong>Our little song</strong></p>
    <audio controls loop preload="none">
      <source src="song.mp3" type="audio/mpeg">
      Your browser does not support this audio file.
    </audio>
    <p class="music-hint">Optional: upload your own audio file as song.mp3 beside index.html.</p>
  </div>
</section>

<section id="surprise">
  <div class="section-head">
    <p class="eyebrow">There's one more thing</p>
    <h2>A tiny secret for you 🎁</h2>
    <p>Something is waiting inside the gift. Ready, Kyuutu?</p>
  </div>
  <div class="card secret">
    <button class="gift" id="gift" aria-label="Open your birthday gift">🎁</button>
    <p id="giftHint">Tap the gift to reveal your surprise</p>
    <div class="secret-message" id="secretMessage">
      <div style="font-size:3rem">🎉💗🎂</div>
      <h2>Happy Birthday, Anuska!</h2>
      <p>
        Today is all about celebrating YOU — your dreams, your laughter,
        your kindness, and every lovely thing that makes you who you are.
      </p>
      <p>May this year bring you beautiful beginnings and countless happy moments.</p>
      <h3>You're one of a kind, Kyuutu. Never forget that. ♡</h3>
      <button class="btn" id="heartButton">Send a little love 💗</button>
      <p id="heartResponse" class="small"></p>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="heart">♡</div>
  <p>Made especially for Anuska, my Kyuutu.</p>
  <p class="small">A little pink world by Biraja Prasad Jena · 2026</p>
  <a href="#home" class="small">Back to the beginning ↑</a>
</footer>

<script>
/* Birthday countdown: October 5, 2026, in the visitor's local time */
const birthday = new Date(2026, 9, 5, 0, 0, 0);
function updateCountdown() {
  const now = new Date();
  const diff = birthday.getTime() - now.getTime();
  const label = document.getElementById("countLabel");
  const line = document.getElementById("birthdayLine");

  if (diff <= 0 && now.toDateString() === birthday.toDateString()) {
    document.getElementById("days").textContent = "🎂";
    document.getElementById("hours").textContent = "💗";
    document.getElementById("minutes").textContent = "🎉";
    document.getElementById("seconds").textContent = "♡";
    label.textContent = "It's your birthday, Kyuutu!";
    line.textContent = "Today is all about you! Happy Birthday! 🌷";
    return;
  }
  if (diff <= 0) {
    document.getElementById("countdownBoxes").style.display = "none";
    label.textContent = "Your special day has arrived and passed for this year 💗";
    line.textContent = "The birthday wishes stay here for you, always.";
    return;
  }
  document.getElementById("days").textContent = Math.floor(diff / 86400000);
  document.getElementById("hours").textContent = Math.floor(diff / 3600000) % 24;
  document.getElementById("minutes").textContent = Math.floor(diff / 60000) % 60;
  document.getElementById("seconds").textContent = Math.floor(diff / 1000) % 60;
}
updateCountdown();
setInterval(updateCountdown, 1000);

/* Floating hearts */
const heartSymbols = ["♡","♥","💗","💕","✧"];
function createHeart() {
  const heart = document.createElement("span");
  heart.className = "float-heart";
  heart.textContent = heartSymbols[Math.floor(Math.random()*heartSymbols.length)];
  heart.style.left = Math.random()*100 + "vw";
  heart.style.fontSize = (12 + Math.random()*20) + "px";
  heart.style.animationDuration = (7 + Math.random()*6) + "s";
  document.body.appendChild(heart);
  setTimeout(() => heart.remove(), 14000);
}
setInterval(createHeart, 950);

/* Open and close letter */
const envelope = document.getElementById("envelope");
const letter = document.getElementById("letterContent");
envelope.addEventListener("click", () => {
  const opened = letter.classList.toggle("show");
  envelope.classList.toggle("open", opened);
  document.getElementById("openHint").textContent =
    opened ? "A little letter, written with love ♡" : "Tap the envelope to open your letter";
  envelope.querySelector(".seal").textContent = opened ? "💖" : "💌";
});

/* Tap-to-reveal reasons */
document.querySelectorAll(".reason").forEach(card => {
  card.addEventListener("click", () => card.classList.toggle("revealed"));
});

/* Gift reveal and confetti */
let giftOpened = false;
function burstConfetti() {
  const symbols = ["💗","💕","✨","🌸","🎉","♡"];
  for (let i = 0; i < 34; i++) {
    const bit = document.createElement("span");
    bit.textContent = symbols[Math.floor(Math.random()*symbols.length)];
    bit.style.position = "fixed";
    bit.style.zIndex = "30";
    bit.style.left = (5 + Math.random()*90) + "vw";
    bit.style.top = "-30px";
    bit.style.fontSize = (14 + Math.random()*18) + "px";
    bit.style.pointerEvents = "none";
    bit.style.transition = "transform 2.5s ease-in, opacity 2.5s ease-in";
    document.body.appendChild(bit);
    requestAnimationFrame(() => {
      bit.style.transform = `translate(${Math.random()*100-50}px, ${window.innerHeight+80}px) rotate(${Math.random()*500}deg)`;
      bit.style.opacity = "0";
    });
    setTimeout(() => bit.remove(), 2800);
  }
}
document.getElementById("gift").addEventListener("click", () => {
  if (giftOpened) return;
  giftOpened = true;
  document.getElementById("secretMessage").classList.add("show");
  document.getElementById("giftHint").textContent = "Surprise! This one's all yours 💗";
  document.getElementById("gift").textContent = "💝";
  burstConfetti();
});
document.getElementById("heartButton").addEventListener("click", () => {
  document.getElementById("heartResponse").textContent =
    "A little love sent from Biraja to Kyuutu. ♡";
  burstConfetti();
});
</script>
</body>
</html>
