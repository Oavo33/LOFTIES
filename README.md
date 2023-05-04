<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Lofties Windows</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <style>
      body {font-family: 'Pacifico', cursive;
  }
  .header, header {font-family: 'Pacifico', cursive;
    background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
    background-size: 100%;
    background-position: center 65%;
    padding: 50px; 
    position: relative;margin: 0;
    width: 80%;
  }
  .confetti {
    position: fixed;
    width: 14px; 
    height: 14px; 
    background-color: #f00;
    pointer-events: none;
  }
  canvas {
    position: absolute;
    top: 10;
    left: 10;
    width: 14%;
    height: 14%;
    pointer-events: none;
  }.cube-container {
    position: absolute;
    transform: translate(5px, 5px);
  }.cube {position: absolute;transform-style: preserve-3d;
    cursor: pointer;
    animation-name: spin;
    animation-duration: 150s; /* adjusted duration */
    animation-iteration-count: infinite;
    animation-timing-function: linear;
  }.cube .side {
    position: absolute;
    width: 21.67px; 
    height: 21.67px; 
    background-color: #00B3B3;
    border: 0.5px solid #260606;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 2px;
    color: #260606;}
      .cube .front {
        transform: rotateY(0deg) translateZ(15px);
      }
      .cube .back {
        transform: rotateY(180deg) translateZ(15px);
      }
      .cube .right {
        transform: rotateY(-90deg) translateZ(15px);
      }
      .cube .left {
        transform: rotateY(90deg) translateZ(15px);
      }
      .cube .top {
        transform: rotateX(90deg) translateZ(15px);
      }
      .cube .bottom {
        transform: rotateX(-90deg) translateZ(15px);
      }@keyframes rotate {
        from {
          transform: rotateY(0deg);
        }
        to {
          transform: rotateY(60deg);
        }
      }@keyframes spin {
        from {
          transform: rotateX(0deg) rotateY(0deg);
        }
        to {
          transform: rotateX(60deg) rotateY(60deg);
        }
      }@keyframes spin-slow {
        from {
          transform: rotateX(0deg) rotateY(0deg);
        }
        to {
          transform: rotateX(60deg) rotateY(60deg);
        }
      }.cube .front:hover::before,
      .cube .back:hover::before,
      .cube .right:hover::before,
      .cube .left:hover::before,
      .cube .top:hover::before,
      .cube .bottom:hover::before {
        content: "";
position: absolute;
width: 100%;
height: 100%;
background-color: rgba(255, 255, 255, 0.8);
z-index: 5;
}  .cube .front:hover::before {
    content: "Get a free window clean by finding the squeegee on our site. Start searching now!";
  }.cube .back:hover::before {
    content: "LOFTIES";
  }.cube .right:hover::before {
    content: "LOFTIES";
  }.cube .left:hover::before {
    content: "LOFTIES";
  }.cube .top:hover::before {
    content: "LOFTIES";
  }.cube .bottom:hover::before {
    content: "LOFTIES";
  }
</style>
  </head><header><div class="cube">
      <div class="side front">LOFTIES</div>
      <div class="side back">LOFTIES</div>
      <div class="side right">LOFTIES</div>
      <div class="side left">LOFTIES</div>
      <div class="side top">LOFTIES</div>
      <div class="side bottom">LOFTIES</div>
    <canvas id="confetti"></canvas>
</header>
  <body>
  <script>const NUM_CONFETTI = 10;
const DELAY = 50;
const DIAMETER = 15;
const COLORS = ["#800000", "#800000", ];
const canvas = document.getElementById("confetti");
const context = canvas.getContext("2d");
canvas.width = window.innerWidth;
canvas.height = window.innerHeight;function ConfettiDot(x, y, color) {
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
}function animateConfetti() {
  context.clearRect(0, 0, canvas.width, canvas.height);
  drawConfetti(confetti);
  updateConfetti(confetti);
  setTimeout(animateConfetti,DELAY);
}const confetti = initConfetti();
animateConfetti();</script>
 </body>
</html>

