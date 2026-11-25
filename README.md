
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pink Lilies For You 💗</title>

<style>
* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  min-height: 100vh;
  min-height: 100dvh;
  background: radial-gradient(
    ellipse at center,
    #fff0f6,
    #ffc4dc 65%,
    #f59abd
  );
  font-family: Georgia, serif;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  overflow-x: hidden;
  color: #963b61;
}

/* MAIN CONTAINER */
.container {
  width: 100%;
  max-width: 900px;
  padding: 40px 24px;
  margin: auto;
  position: relative;
  z-index: 2;
}

/* HEADINGS */
h1 {
  font-size: clamp(28px, 4vw, 46px);
  margin-bottom: 25px;
}

h2 {
  font-size: clamp(22px, 3vw, 30px);
}

p {
  font-size: 18px;
  line-height: 1.8;
}

/* BUTTON */
button {
  background: #e65b93;
  color: white;
  border: none;
  padding: 18px 35px;
  border-radius: 30px;
  font-size: 18px;
  cursor: pointer;
  box-shadow: 0 5px 20px #c8518270;
  transition: transform 0.3s, background 0.3s;
}

button:hover {
  background: #d94a85;
  transform: scale(1.05);
}

#surprise {
  display: none;
}

/* BIGGER FLOWERS */
.bouquet {
  display: block;
  width: 100%;
  max-width: 550px;
  height: auto;
  margin: 10px auto 30px;
  overflow: visible;
  filter: drop-shadow(0 10px 12px #b44d7755);
}

/* STEM ANIMATION */
.stem {
  fill: none;
  stroke: #4c8650;
  stroke-width: 7;
  stroke-linecap: round;
  stroke-dasharray: 400;
  stroke-dashoffset: 400;
  animation: grow 2s ease forwards;
}

/* LEAVES */
.leaf {
  fill: #53945c;
  transform-box: fill-box;
  transform-origin: bottom center;
  animation: leafGrow 1.5s ease both;
}

/* FLOWER BLOOMING */
.flower {
  transform-box: fill-box;
  transform-origin: center;
  transform: scale(0);
  animation: bloom 2.5s
    cubic-bezier(.2,1.5,.5,1) forwards;
}

.flower.two {
  animation-delay: 1s;
}

.flower.three {
  animation-delay: 1.7s;
}

/* PETALS */
.petal {
  fill: url(#petalGradient);
  stroke: #dc75a0;
  stroke-width: 1;
}

.petal-line {
  fill: none;
  stroke: #d56a99;
  stroke-width: 1.3;
  opacity: .55;
}

/* FLOWER DETAILS */
.stamen {
  stroke: #8c4960;
  stroke-width: 2;
  stroke-linecap: round;
}

.anther {
  fill: #a64e35;
}

/* APOLOGY LETTER */
.message {
  background: #ffffffd9;
  padding: 40px;
  border-radius: 25px;
  margin: 20px auto;
  width: 100%;
  max-width: 650px;
  box-shadow: 0 8px 30px #ba5a8560;
  animation: appear 2s ease 2s both;
  line-height: 1.8;
}

.message p {
  font-size: 19px;
  line-height: 1.9;
  margin-bottom: 20px;
}

.message h3 {
  font-size: 24px;
}

/* FLOATING HEARTS */
.heart {
  position: fixed;
  bottom: -30px;
  pointer-events: none;
  animation: float 7s linear forwards;
  z-index: 1;
}

/* ANIMATIONS */
@keyframes grow {
  to {
    stroke-dashoffset: 0;
  }
}

@keyframes leafGrow {
  from {
    transform: scale(0);
    opacity: 0;
  }
  to {
    transform: scale(1);
    opacity: 1;
  }
}

@keyframes bloom {
  0% {
    transform: scale(0);
    opacity: 0;
  }
  65% {
    transform: scale(1.12);
    opacity: 1;
  }
  100% {
    transform: scale(1);
    opacity: 1;
  }
}

@keyframes appear {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes float {
  to {
    transform: translateY(-110vh) rotate(30deg);
    opacity: 0;
  }
}

/* TABLET */
@media (max-width: 768px) {
  .container {
    max-width: 600px;
    padding: 30px 20px;
  }

  .bouquet {
    max-width: 440px;
  }

  .message {
    max-width: 520px;
    padding: 30px;
  }

  .message p {
    font-size: 17px;
  }
}

/* MOBILE PHONES */
@media (max-width: 480px) {
  body {
    align-items: center;
  }

  .container {
    width: 100%;
    padding: 25px 15px;
  }

  h1 {
    font-size: 29px;
    margin-bottom: 15px;
  }

  .bouquet {
    width: 100%;
    max-width: 350px;
    margin: 10px auto 20px;
  }

  .message {
    width: 100%;
    max-width: 380px;
    padding: 25px 20px;
    border-radius: 20px;
    margin: 15px auto;
  }

  .message p {
    font-size: 16px;
    line-height: 1.8;
  }

  .message h3 {
    font-size: 21px;
  }

  button {
    font-size: 16px;
    padding: 15px 25px;
  }
}

/* SMALL PHONES */
@media (max-width: 360px) {
  .container {
    padding: 20px 12px;
  }

  .bouquet {
    max-width: 300px;
  }

  .message {
    padding: 20px 15px;
  }

  .message p {
    font-size: 15px;
  }
}
</style>
</head>

<body>

<div class="container">

  <!-- OPENING SCREEN -->
  <div id="start">

    <h1>For my favorite girl 💗</h1>

    <p>I know you love pink lilies...</p>
    <p>So I made these just for you.</p>

    <button onclick="openGift()">
      Open your flowers ♡
    </button>

  </div>

  <!-- SURPRISE SCREEN -->
  <div id="surprise">

    <h1>I'm Sorry, My Love ♡</h1>

    <!-- PINK LILY BOUQUET -->
    <svg class="bouquet"
      viewBox="0 0 400 430"
      xmlns="http://www.w3.org/2000/svg">

      <defs>

        <!-- PINK PETAL GRADIENT -->
        <radialGradient id="petalGradient">
          <stop offset="0%" stop-color="#fff3b9"/>
          <stop offset="25%" stop-color="#ffe4ec"/>
          <stop offset="65%" stop-color="#f7a1c5"/>
          <stop offset="100%" stop-color="#d95796"/>
        </radialGradient>

        <!-- LILY FLOWER -->
        <g id="lily">

          <!-- SIX PETALS -->
          <path class="petal"
            d="M0 0 Q-43 -35 -13 -102
               Q0 -125 13 -102 Q43 -35 0 0"/>

          <path class="petal"
            d="M0 0 Q-43 -35 -13 -102
               Q0 -125 13 -102 Q43 -35 0 0"
            transform="rotate(60)"/>

          <path class="petal"
            d="M0 0 Q-43 -35 -13 -102
               Q0 -125 13 -102 Q43 -35 0 0"
            transform="rotate(120)"/>

          <path class="petal"
            d="M0 0 Q-43 -35 -13 -102
               Q0 -125 13 -102 Q43 -35 0 0"
            transform="rotate(180)"/>

          <path class="petal"
            d="M0 0 Q-43 -35 -13 -102
               Q0 -125 13 -102 Q43 -35 0 0"
            transform="rotate(240)"/>

          <path class="petal"
            d="M0 0 Q-43 -35 -13 -102
               Q0 -125 13 -102 Q43 -35 0 0"
            transform="rotate(300)"/>

          <!-- PETAL VEINS -->
          <g class="petal-line">

            <path d="M0 0 L0 -92"/>

            <path d="M0 0 L0 -92"
              transform="rotate(60)"/>

            <path d="M0 0 L0 -92"
              transform="rotate(120)"/>

            <path d="M0 0 L0 -92"
              transform="rotate(180)"/>

            <path d="M0 0 L0 -92"
              transform="rotate(240)"/>

            <path d="M0 0 L0 -92"
              transform="rotate(300)"/>

          </g>

          <!-- STAMENS -->
          <g class="stamen">
            <path d="M0 0 L-17 -35"/>
            <path d="M0 0 L17 -35"/>
            <path d="M0 0 L-33 -12"/>
            <path d="M0 0 L33 -12"/>
            <path d="M0 0 L-15 31"/>
            <path d="M0 0 L15 31"/>
          </g>

          <!-- ANTHERS -->
          <g class="anther">
            <ellipse cx="-17" cy="-35" rx="5" ry="9"/>
            <ellipse cx="17" cy="-35" rx="5" ry="9"/>
            <ellipse cx="-33" cy="-12" rx="5" ry="9"/>
            <ellipse cx="33" cy="-12" rx="5" ry="9"/>
            <ellipse cx="-15" cy="31" rx="5" ry="9"/>
            <ellipse cx="15" cy="31" rx="5" ry="9"/>
          </g>

          <circle r="7" fill="#fff1ac"/>

        </g>
      </defs>

      <!-- STEMS -->
      <path class="stem"
        d="M200 390 Q130 270 105 155"/>

      <path class="stem"
        d="M200 390 Q200 245 200 100"/>

      <path class="stem"
        d="M200 390 Q275 270 300 155"/>

      <!-- LEAVES -->
      <path class="leaf"
        d="M180 315 Q95 235 115 310 Q145 350 180 315"/>

      <path class="leaf"
        d="M220 315 Q310 235 280 315 Q255 345 220 315"/>

      <path class="leaf"
        d="M195 270 Q135 195 155 265 Q180 295 195 270"/>

      <path class="leaf"
        d="M210 260 Q270 190 255 260 Q235 290 210 260"/>

      <!-- THREE PINK LILIES -->
      <g class="flower one">
        <use href="#lily"
          transform="translate(105 155) scale(.72)"/>
      </g>

      <g class="flower two">
        <use href="#lily"
          transform="translate(200 105) scale(.82)"/>
      </g>

      <g class="flower three">
        <use href="#lily"
          transform="translate(300 155) scale(.72)"/>
      </g>

      <!-- PINK RIBBON -->
      <path
        d="M172 350 Q200 340 228 350
           L220 380 Q200 389 180 380 Z"
        fill="#f38ab4"/>

      <path
        d="M192 360 Q120 315 155 380 L192 370"
        fill="#ffb3d0"/>

      <path
        d="M208 360 Q280 315 245 380 L208 370"
        fill="#ffb3d0"/>

      <circle cx="200" cy="365"
        r="10" fill="#e45b96"/>

    </svg>

    <!-- PERSONALIZED APOLOGY LETTER -->
    <div class="message">

      <h2>💗</h2>

      <p>
        I'm sorry making you overthink :<
      </p>

      <p>
        Just like these flowers, I hope we can
        continue to grow together.
      </p>

      <p>
        You deserve everything good in this world
        and I wanna sgare it with you.
        I promise to keep working to be better for you.
      </p>

      <h3>I love you so much. ♡</h3>

    </div>

  </div>
</div>

<script>

/* OPEN THE SURPRISE */
function openGift() {
  document.getElementById("start").style.display = "none";
  document.getElementById("surprise").style.display = "block";
}

/* FLOATING HEARTS */
function makeHeart() {

  const heart = document.createElement("div");

  heart.className = "heart";

  heart.textContent = ["♡", "♥", "💕", "🌸"][
    Math.floor(Math.random() * 4)
  ];

  heart.style.left = Math.random() * 100 + "vw";

  heart.style.fontSize =
    (15 + Math.random() * 18) + "px";

  heart.style.color = "#e65b93";

  document.body.appendChild(heart);

  setTimeout(() => heart.remove(), 7000);
}

setInterval(makeHeart, 500);

</script>

</body>
</html>
