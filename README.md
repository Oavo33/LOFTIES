<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1"><title>Lofties Windows</title>
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
    <style>body {
        font-family: 'UnifrakturMaguntia', sans-serif;
        background-color: #800000;
        color: #800000;
      }header {
        font-family: 'UnifrakturMaguntia', sans-serif;
        background-color: #800000;
        background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
        background-size: 100%;
        background-position: center 65%;
        color: #00b3b3;
        padding: 30px;
        position: relative;
        text-align: center;
        text-shadow: 2px 2px #800000;}.logo {
        position: absolute;
        bottom: 0;
        left: 0;
        margin: 0;
        display: flex;
        align-items: center;
      }.logo-container {
        display: inline-block;
        border: 1px solid #ff6600;
        border-radius: 10px;
        padding: 10px;
        margin: 20px;
        font: italic 3em 'UnifrakturMaguntia', cursive;
        text-shadow: 2px 2px #ffa500;
        color: #ff6600;
      }ul {
        list-style: none;
        margin: 0;
        padding: 0;
      }ul.social li {
        display: inline-block;
        margin: 0 10px;
      }button {
        position: relative;
        font: bold 1.2rem 'UnifrakturMaguntia', cursive;
        color: #fff;
        background: #ff6600;
        border: none;
        border-radius: 25px;
        padding: 15px 30px;
        cursor: pointer;
      }.ball {
        width: 50px;
        height: 50px;
        border-radius: 50%;
        background: #ffa500;
        opacity: 0;
        position: absolute;
        left: 34%;
        top: 12%;
        transform: translate(-50%, -50%);
        z-index: -1;
        transition: all .5s ease-in-out;
      }.move {
        display: inline-block;
        color: transparent;
        text-shadow: 0 0 5px #ffa500;
      }.move:hover {
        text-shadow: none;
        animation: move-text 14s ease-in-out;
      }@keyframes move-text {
        0% {
          transform: translate(0, 0) rotate(0deg);
        }
        25% {
          transform: translate(100px, 100px) rotate(90deg);
        }
        50% {
          transform: translate(-100px, 100px) rotate(180deg);
        }
        75% {
          transform: translate(-100px, -100px) rotate(270deg);
        }
        100% {
          transform: translate(100px, -100px) rotate(360deg);
        }
      }button:focus+.ball {
        opacity: 1;
        animation: move-ball 2s linear infinite;
        --x: .1;
        --y: .1;
      }@keyframes move-ball {
        to {
          transform: move-ball(calc(200vw * var(--x)), calc(200vh * var(--y)));
        }
      }ul {
        font-family: 'UnifrakturMaguntia', sans-serif;
        list-style-type: none;
        margin: 0;
        padding: 0;
        background-color: #333;
        overflow: hidden;
      }li:nth-child(1) a {
        animation: fadeInLeft 5s ease-out;
      }li:nth-child(2) a {
        animation: pop 0.5s ease-out forwards;
        animation-delay: 5s;
      }li:nth-child(3) a {
      animation: zoomInRight 5s ease-out;
    }li a {
      font-family: 'UnifrakturMaguntia', sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-align: center;
      padding: 14px 16px;
      text-decoration: none;
      font-size: 24px;
      font-weight: bold;
    }@keyframes fadeInLeft {
      0% {
        opacity: 0;
        transform: translateX(-100%);
      }
      100% {
        opacity: 1;
        transform: translateX(0);
      }
    }@keyframes pop {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.5);
      }
      100% {
        transform: scale(1);
      }
    }@keyframes zoomInRight {
      0% {
        opacity: 0;
        transform: scale(0.1) translateX(200%);
      }
      100% {
        opacity: 1;
        transform: scale(1) translateX(0);
      }
    }.icon {
      font-family: 'UnifrakturMaguntia', sans-serif;
      display: inline-block;
      margin-right: 8px;
      font-size: 24px;
    }.video-icon {
      color: red;
    }.game-icon {
      color: green;
    }.music-icon {
      color: blue;}@media screen and (max-width: 768px) {
      h1 {
        font-family: 'UnifrakturMaguntia', sans-serif;
        font-size: 1.5rem;
        padding: 10px;
      }ul.social li {
        margin: 0 5px;
      }button {
        font-family: 'UnifrakturMaguntia', sans-serif;
        margin-top: 30px;
        font-size: 1;
      }
    }.confetti {
        position: fixed;
        width: 5px;
        height: 5px;
        background-color: #f00;
        pointer-events: none;
      }
      canvas {
        position: absolute;
        top: 0;
        left: 0;
        width: 280%;
        height: 280%;
        pointer-events: none;
      }
      .cube-container {
  position: absolute;
  width: 3.33px;
  height: 3.33px;
  bottom: 14px;
  left: 20px;
  transform: translate(1.67px, 1.67px); /* adjust the values as needed */
}.cube {
  position: absolute;
  width: 4.67px; /* 20px / 3 */
  height: 4.67px; /* 20px / 3 */
  transform-style: preserve-3d;
  animation: rotate 10s infinite linear;
  cursor: pointer;
  animation-name: spin;
  animation-duration: 34s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
      .cube:hover {
        animation: spin-slow 20s infinite linear;
      }
      .cube .side {
  font-family: 'UnifrakturMaguntia', sans-serif;
  position: absolute;
  width: 15.33px; /* 70px / 3 */
  height: 15.33px; /* 70px / 3 */
  background-color: #00B3B3;
  border: 1px solid #260606;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 3px; /* 9px / 3 */
  font-weight: bold;
  color: #260606;
  text-transform: uppercase;
  transform-style: preserve-3d;
  text-align: center;
  writing-mode: horizontal-tb;
}.cube .front {font-family: 'UnifrakturMaguntia', sans-serif;
  transform: rotateY(0deg) translateZ(10.67px); /* 50px / 3 */
}.cube .back {font-family: 'UnifrakturMaguntia', sans-serif;
  transform: rotateY(180deg) translateZ(10.67px); /* 50px / 3 */
}.cube .right {font-family: 'UnifrakturMaguntia', sans-serif;
  transform: rotateY(-90deg) translateZ(10.67px); /* 50px / 3 */
}.cube .left {font-family: 'UnifrakturMaguntia', sans-serif;
  transform: rotateY(90deg) translateZ(10.67px); /* 50px / 3 */
}.cube .top {font-family: 'UnifrakturMaguntia', sans-serif;
  transform: rotateX(90deg) translateZ(10.67px); /* 50px / 3 */
}.cube .bottom {font-family: 'UnifrakturMaguntia', sans-serif;
  transform: rotateX(-90deg) translateZ(10.67px); /* 50px / 3 */
}@keyframes rotate {
  from {
    transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
  }
  to {
    transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
  }
}@keyframes spin {
  from {
    transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
  }
  to {
    transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
  }
}@keyframes spin-slow {
  from {
    transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
  }
  to {
    transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
  }
}.cube .front:hover::before,
      .cube .back:hover::before,
      .cube .right:hover::before,
      .cube .left:hover::before,
      .cube .top:hover::before,
      .cube .bottom:hover::before {
        font-family: 'UnifrakturMaguntia', sans-serif;
        content: "Spot the squeegee on our webpage and you'll win a FREE window clean! Look closely!";
        position: absolute;
        top: 35px;
        left: -130px;
background-color: #fff;
color: #260606;
font-size: 10px;
padding: 5px;
border-radius: 5px;
box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.5);
opacity: 0;
transition: opacity 0.2s ease-in-out;
}
.cube .front:hover::before {
transform: rotateY(0deg) translateZ(50px);
}
.cube .back:hover::before {
transform: rotateY(180deg) translateZ(50px);
}
.cube .right:hover::before {
transform: rotateY(-90deg) translateZ(50px);
}
.cube .left:hover::before {
transform: rotateY(90deg) translateZ(50px);
}
.cube .top:hover::before {
transform: rotateX(90deg) translateZ(50px);
}
.cube .bottom:hover::before {
transform: rotateX(-90deg) translateZ(50px);
}
.cube .front:hover::before {
opacity: 1;
}
.cube .back:hover::before {
opacity: 1;
}
.cube .right:hover::before {
opacity: 1;
}
.cube .left:hover::before {
opacity: 1;
}
.cube .top:hover::before {
opacity: 1;
}
.cube .bottom:hover::before {
opacity: 1;
}</style>
</head><body>
  <header>
    <ul>
      <li><a href="#home"><span class="icon video-icon">&#x1F3A5;</span> Videos</a></li>
      <li><a href="#about"><span class="icon game-icon">&#x1F3AE;</span> Games</a></li>
      <li><a href="#contact"><span class="icon music-icon">&#x1F3B5;</span> Music</a></li>
    </ul>
    <div class="logo-container">
      <span class="move">L</span>ofties<span class="move">W</span>indo<span class="move">w</span>s
    </div>
    <button>Click me!</button>
    <div class="ball"></div>
    <ul class="social">
      <li><a href="#"><i class="icon1"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></i></a></li>
      <li><a href="#"><i class="icon4"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></i></a></li>
      <li><a href="#"><i class="icon3"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></i></a></li></ul></header>
<div class="cube-container">
    <div class="cube">
      <div class="side front">LOFTIES</div>
      <div class="side back">LOFTIES</div>
      <div class="side right">LOFTIES</div>
      <div class="side left">LOFTIES</div>
      <div class="side top">LOFTIES</div>
      <div class="side bottom">LOFTIES</div>
    <canvas id="confetti"></canvas><script>const NUM_CONFETTI = 10;
const DELAY = 50;
const DIAMETER = 15;
const COLORS = ["#800000", "#800000", ];
const canvas = document.getElementById("confetti");
const context = canvas.getContext("2d");
canvas.width = window.innerWidth;
canvas.height = window.innerHeight;
function ConfettiDot(x, y, color) {
  this.x = x;
  this.y = y;
  this.color = color;
  this.colorIndex = 0;
}function randomInt(min, max) {
  return Math.floor(Math.random() * (max - min + 1) + min);
}function initConfetti() {
  const confetti = [];
  for (let i = 0; i < NUM_CONFETTI; i++) {
    const x = randomInt(0, canvas.width - DIAMETER);
    const y = randomInt(0, canvas.height - DIAMETER);
    const color = COLORS[0];
    confetti.push(new ConfettiDot(x, y, color));
  }
  return confetti;
}function drawConfetti(confetti) {
  for (let i = 0; i < confetti.length; i++) {
    const dot = confetti[i];
    context.beginPath();
    context.arc(dot.x, dot.y, DIAMETER, 0, 2 * Math.PI, false);
    context.fillStyle = dot.color;
    context.fill();
  }
}function updateConfetti(confetti) {
  for (let i = 0; i < confetti.length; i++) {
    const dot = confetti[i];
    if (dot.colorIndex < COLORS.length - 1) {
     dot.colorIndex += 1;
      const startColor = COLORS[dot.colorIndex - 1];
      const endColor = COLORS[dot.colorIndex];
      const r1 = parseInt(startColor.substr(1, 2), 16);
      const g1 = parseInt(startColor.substr(3, 2), 16);
      const b1 = parseInt(startColor.substr(5, 2), 16);
      const r2 = parseInt(endColor.substr(1, 2), 16);
      const g2 = parseInt(endColor.substr(3, 2), 16);
      const b2 = parseInt(endColor.substr(5, 2), 16);
      const r = Math.floor((r1 * (COLORS.length - dot.colorIndex) + r2 * dot.colorIndex) / COLORS.length);
      const g = Math.floor((g1 * (COLORS.length - dot.colorIndex) + g2 * dot.colorIndex) / COLORS.length);
      const b = Math.floor((b1 * (COLORS.length - dot.colorIndex) + b2 * dot.colorIndex) / COLORS.length);
      dot.color = `rgb(${r},${g},${b})`;
    }
    dot.x += randomInt(-1, 1);
    dot.y += randomInt(1, 3);
    if (dot.y > canvas.height) {
      dot.y = -DIAMETER;
      dot.x = randomInt(0, canvas.width - DIAMETER);
    }
  }
}
function animateConfetti() {
  context.clearRect(0, 0, canvas.width, canvas.height);
  drawConfetti(confetti);
  updateConfetti(confetti);
  setTimeout(animateConfetti,DELAY);
}
const confetti = initConfetti();
animateConfetti();</script></body>
</html>


