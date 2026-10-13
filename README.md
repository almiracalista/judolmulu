# judolmulu

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HEY JOE!!! 💢</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&family=Quicksand:wght@500;700;800&display=swap');

:root {
  --pink: #f5b9c8;
  --cream: #fff8e9;
  --brown: #49332b;
  --red: #f15b64;
}

* { box-sizing: border-box; }

body {
  margin: 0;
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 20px;
  color: var(--brown);
  font-family: 'Quicksand', sans-serif;
  background-color: #e9d9c8;
  background-image:
    radial-gradient(#fff9e8 2px, transparent 2.5px),
    repeating-linear-gradient(0deg, transparent 0 24px, #b99c8a30 25px 27px),
    repeating-linear-gradient(90deg, transparent 0 24px, #b99c8a30 25px 27px);
  background-size: 35px 35px, 100% 100%, 100% 100%;
  overflow-x: hidden;
}

.scrapbook {
  width: min(100%, 480px);
  min-height: 610px;
  padding: 25px 23px;
  position: relative;
  overflow: hidden;
  border: 8px solid #fff8ec;
  outline: 2px dashed #b89a87;
  outline-offset: -13px;
  background:
    repeating-linear-gradient(0deg, #5d4035 0 3px, #64483d 3px 6px);
  box-shadow: 0 15px 40px #51392b35;
  text-align: center;
}

.page {
  display: none;
  min-height: 545px;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  animation: appear .55s ease both;
}

.page.active { display: flex; }

@keyframes appear {
  from { opacity: 0; transform: translateY(18px) scale(.97); }
  to { opacity: 1; transform: translateY(0) scale(1); }
}

.tape {
  position: absolute;
  width: 105px;
  height: 25px;
  top: 5px;
  left: 50%;
  transform: translateX(-50%) rotate(-4deg);
  background: #f8d3d2c9;
  z-index: 3;
}

.paper {
  width: 100%;
  padding: 28px 17px;
  position: relative;
  background: var(--cream);
  border: 5px solid white;
  outline: 2px dotted #e6b7b9;
  outline-offset: -10px;
  box-shadow: 4px 6px 0 #2d1d1838;
}

.paper::before {
  content: '✿  ♡  ✿  ♡  ✿';
  display: block;
  color: #dc9eaa;
  letter-spacing: 5px;
  font-size: 14px;
  margin-bottom: 13px;
}

h1, h2, p { margin-top: 8px; }

h1 {
  font-size: clamp(30px, 8vw, 44px);
  line-height: 1.1;
  font-weight: 800;
}

h2 {
  font-size: clamp(25px, 7vw, 36px);
  line-height: 1.15;
}

p {
  line-height: 1.7;
  font-size: 15px;
}

.hand {
  font-family: 'Patrick Hand', cursive;
}

.pink { color: #e66d89; }
.red { color: #e94b57; }

.doodle {
  font-size: 64px;
  margin: 7px 0;
  animation: wobble 1.5s infinite ease-in-out;
}

@keyframes wobble {
  0%, 100% { transform: rotate(-7deg) scale(1); }
  50% { transform: rotate(7deg) scale(1.08); }
}

button {
  border: 2px solid #624538;
  border-radius: 30px;
  padding: 12px 21px;
  margin: 8px 3px;
  background: #f6b7c6;
  color: #49332b;
  font: 800 14px 'Quicksand', sans-serif;
  cursor: pointer;
  box-shadow: 0 4px 0 #624538;
  transition: .15s;
}

button:hover {
  transform: translateY(-3px) rotate(-2deg);
  background: #ffccd8;
}

button:active {
  transform: translateY(2px);
  box-shadow: none;
}

.secondary { background: #fff8e9; }

.sticker {
  display: inline-block;
  font-size: 31px;
  margin: 3px;
  animation: shake .55s infinite alternate;
}

.sticker:nth-child(even) { animation-delay: -.3s; }

@keyframes shake {
  from { transform: rotate(-12deg) scale(.94); }
  to { transform: rotate(12deg) scale(1.08); }
}

.sticker-wall {
  width: 100%;
  min-height: 115px;
  margin: 12px 0;
  display: flex;
  align-content: center;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 4px;
}

.sticker-wall span {
  display: inline-block;
  font-size: 28px;
  animation: pop .45s ease both, shake .6s infinite alternate;
}

@keyframes pop {
  from { transform: scale(0); }
  to { transform: scale(1); }
}

.mini {
  font-size: 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
}

.footer {
  margin-top: 17px;
  font: 16px 'Patrick Hand', cursive;
  color: #fff0df;
}

.counter {
  font-size: 12px;
  color: #fff0df;
  margin-top: 10px;
}

#floating {
  position: fixed;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
  z-index: 10;
}

.floaty {
  position: absolute;
  bottom: -60px;
  animation: fly 3.4s ease-out forwards;
}

@keyframes fly {
  0% { transform: translateY(0) rotate(0); opacity: 1; }
  100% { transform: translateY(-110vh) rotate(400deg); opacity: 0; }
}

@media(max-width:380px) {
  .scrapbook { padding: 18px 15px; }
  .paper { padding: 25px 13px; }
}
</style>
</head>

<body>
<div id="floating"></div>

<main class="scrapbook">
  <div class="tape"></div>

  <!-- PAGE 1 -->
  <section class="page active" id="page1">
    <div class="paper">
      <div class="mini">♡ a very important announcement ♡</div>

      <div class="doodle">૮ ˶ᵔ ᵕ ᵔ˶ ა</div>

      <h1>HALOOO<br>JOEEEE!!!</h1>

      <p class="hand pink" style="font-size:23px">
        helloooo, mister troublemaker ♡
      </p>

      <p>
        i made a tiny website<br>
        specifically for YOU, joe.
      </p>

      <p class="hand">and no, you cannot escape. HEHE.</p>

      <div>🎀 🧸 💌 🐻 🎀</div>

      <button onclick="nextPage(2)">
        CLICK ME, JOE ♡ →
      </button>
    </div>
    <div class="footer">made with love & 2% patience ♡</div>
  </section>

  <!-- PAGE 2 -->
  <section class="page" id="page2">
    <div class="paper">
      <div class="mini">🚨 emergency announcement 🚨</div>

      <div class="sticker-wall">
        <span>😡</span><span>💢</span><span>👊</span>
        <span>😤</span><span>💥</span>
      </div>

      <h1 class="red">STOP<br>JUDOL</h1>
      <h2 class="red">JOEEEEEE!!!</h2>

      <p class="hand" style="font-size:23px">
        JOE, I AM WATCHING YOU. 👁️👁️
      </p>

      <p>
        your money deserves better things!!<br>
        snacks 🍟, cute stuff 🎀, and a future! 🥹
      </p>

      <div class="sticker-wall">
        <span>👊</span><span>😡</span><span>💢</span>
        <span>👊</span><span>💥</span><span>😤</span>
      </div>

      <button onclick="rage()">SPAM TINJU 👊💢</button>
      <button class="secondary" onclick="nextPage(3)">NEXT PAGE →</button>
    </div>
    <div class="footer">THIS IS YOUR OFFICIAL WARNING!!! 💢</div>
  </section>

  <!-- PAGE 3 -->
  <section class="page" id="page3">
    <div class="paper">
      <div class="mini">a message from your tiny manager ♡</div>

      <div class="sticker-wall">
        <span>😡</span><span>👊</span><span>💢</span>
        <span>👊</span><span>😤</span><span>💥</span>
        <span>👊</span><span>😡</span><span>👊</span>
      </div>

      <h2 class="red">OKAY JOE...</h2>
      <h1 class="pink">JANGAN<br>MARAH MULU!!</h1>

      <div class="doodle">૮₍ ˶•⤙•˶ ₎ა</div>

      <p class="hand" style="font-size:23px">
        take a deep breath, bubs. ♡
      </p>

      <p>
        breathe in... 🌸<br>
        breathe out... 🧸<br>
        unclench your jaw, please. 😭
      </p>

      <p><b>you look cuter when you're happy!</b></p>

      <button onclick="calmDown()">OKAY, I WILL TRY ♡</button>
      <button class="secondary" onclick="nextPage(1)">START AGAIN ↺</button>

      <div id="calmMessage" class="hand pink"></div>
    </div>
    <div class="footer">be nice to yourself & everyone else ♡</div>
  </section>

  <div class="counter" id="counter">PAGE 1 / 3</div>
</main>

<script>
let currentPage = 1;

function nextPage(number) {
  document.getElementById('page' + currentPage)
    .classList.remove('active');

  currentPage = number;

  document.getElementById('page' + currentPage)
    .classList.add('active');

  document.getElementById('counter').textContent =
    'PAGE ' + currentPage + ' / 3';

  window.scrollTo({ top: 0, behavior: 'smooth' });

  if (number === 2) {
    setTimeout(() => burst(8), 200);
  }

  if (number === 3) {
    setTimeout(() => burst(12), 200);
  }
}

function burst(amount = 12) {
  const area = document.getElementById('floating');
  const stickers = ['👊', '😡', '💢', '😤', '💥', '🗯️'];

  for (let i = 0; i < amount; i++) {
    const item = document.createElement('span');

    item.className = 'floaty';
    item.textContent =
      stickers[Math.floor(Math.random() * stickers.length)];

    item.style.left = Math.random() * 95 + 'vw';
    item.style.fontSize = (25 + Math.random() * 28) + 'px';
    item.style.animationDuration = (2 + Math.random() * 2) + 's';

    area.appendChild(item);

    setTimeout(() => item.remove(), 4500);
  }
}

function rage() {
  burst(32);

  const wall = document.querySelector('#page2 .sticker-wall');
  const stickers = ['👊', '😡', '💢', '😤', '💥', '🗯️'];

  for (let i = 0; i < 18; i++) {
    const item = document.createElement('span');
    item.textContent =
      stickers[Math.floor(Math.random() * stickers.length)];
    wall.appendChild(item);
  }
}

function calmDown() {
  const message = document.getElementById('calmMessage');

  message.textContent = 'YAYYYY!! PROUD OF YOU, JOE 🥹💗';
  burst(20);

  document.querySelector('#page3 .paper h1').textContent =
    'GOOD JOB, JOE!!';

  document.querySelector('#page3 .paper h1').classList.remove('pink');
  document.querySelector('#page3 .paper h1').classList.add('pink');
}
</script>
</body>
</html>
