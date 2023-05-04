
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Lofties Windows</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #333333;
      color: #f2f2f2;
      font-family: 'Pacifico', cursive;
    }
    header {
      background-color: #800000;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
      background-size: 100%;
      background-position: center 65%;
      padding: 60px;
      position: relative;
      bottom: 0;
      left: 0;
      margin: 0;
      font-family: 'Pacifico', cursive;
    }
    .confetti {
      position: fixed;
      width: 10px;
      height: 10px;
      background-color: #f00;
      pointer-events: none;
    }
    canvas {
      position: absolute;
      top: 0;
      left: 0;
      width: 110%;
      height: 110%;
      pointer-events: none;
    }
    .cube-container {
      position: relative;
      width: 8.33px;
      height: 8.33px;
      top: 60%;
      left: 10%;
      transform: translate(10px, 10px);
    }
    .cube {
      position: absolute;
      width: 23.33px;
      height: 23.33px;
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
      position: absolute;
      width: 23.33px;
      height: 23.33px;
      background-color: #00B3B3;
      border: 1px solid #260606;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 4px;
      font-weight: bold;
      color: #260606;
      text-transform: uppercase;
      transform-style: preserve-3d;
      text-align: center;
      writing-mode: horizontal-tb;
    }
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
    }
  @keyframes rotate {
    from {
      transform: rotateY(0deg);
    }
    to {
      transform: rotateY(360deg);
    }
  }
  @keyframes spin {
    from {
      transform: rotateX(0deg) rotateY(0deg);
    }
    to {
      transform: rotateX(360deg) rotateY(360deg);
    }
  }
  @keyframes spin-slow {
    from {
      transform: rotateX(0deg) rotateY(0deg);
}
to {
transform: rotateX(360deg) rotateY(360deg);
}
}</style>

<header>
  <h1>Welcome to my website!</h1>
  <p>Thanks for visiting.</p>
</header>
<canvas id="canvas"></canvas>

<div class="confetti"></div>
<div class="cube-container">
  <div class="cube">
    <div class="side front">Front</div>
    <div class="side back">Back</div>
    <div class="side right">Right</div>
    <div class="side left">Left</div>
    <div class="side top">Top</div>
    <div class="side bottom">Bottom</div>
  </div>
</div>
<script>
  const canvas = document.getElementById("canvas");
  const context = canvas.getContext("2d");
let width = canvas.width = window.innerWidth;
  let height = canvas.height = window.innerHeight;
const confettiColors = [
    "#E71D36",
    "#F44336",
    "#FF4081",
    "#9C27B0",
    "#673AB7",
    "#3F51B5",
    "#2196F3",
    "#00BBD6",
    "#009688",
    "#4CAF50",
    "#8BC34A",
    "#CDDC39",
    "#FFC107",
    "#FF9800",
    "#FF5722"
  ];
const confettiArray = [];
function Confetti(x, y, angle, color) {
    this.x = x;
    this.y = y;
    this.color = color;
    this.angle = angle;
    this.speed = Math.random() * 4 + 1;
    this.radius = Math.random() * 4 + 1;
    this.gravity = 0.1;
    this.opacity = Math.random() * 0.5 + 0.5;
  }
Confetti.prototype.update = function() {
    this.x += Math.cos(this.angle) * this.speed;
    this.y += Math.sin(this.angle) * this.speed + this.gravity;
    this.speed -= this.speed / 50;
    this.radius -= this.radius / 50;
    this.opacity -= 0.01;
  }
Confetti.prototype.draw = function() {
    context.beginPath();
    context.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
    context.fillStyle = this.color;
    context.globalAlpha = this.opacity;
    context.fill();
  }
function createConfetti() {
    const angle = Math.random() * Math.PI * 2;
    const x = width / 2 + Math.cos(angle) * (Math.random() * width);
    const y = height / 2 + Math.sin(angle) * (Math.random() * height);
    const color = confettiColors[Math.floor(Math.random() * confettiColors.length)];
    confettiArray.push(new Confetti(x, y, angle, color));
  }
function animateConfetti() {
    context.clearRect(0, 0, width, height);
    for (let i = 0; i < confettiArray.length; i++) {
      confettiArray[i].update();
      confettiArray[i].draw();
      if (confettiArray[i].radius < 1 || confettiArray[i].opacity < 0) {
        confettiArray.splice(i, 1);
        i--;
      }
    }requestAnimationFrame(animateConfetti);
  }
setInterval(createConfetti, 50);
  requestAnimationFrame(animateConfetti);
</script>
</body>
</html> 

