<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=750&q=80");
      background-size: cover;
      background-position: center;
      padding: 80px; 
    }
    #jake {
      position: relative;
      margin-top: 30px;
    }
    #jake {
      position: absolute;
      bottom: 4px;
      left: 55%;
      transform: translateX(-50%);
      display: flex;
      align-items: center;
    }
    #jakey {
      width: 20px;
      height: 20px;
      border-radius: 50%;
      background-image: radial-gradient(#800000, #00b3b3);
      cursor: pointer;
      transition: background-image 0.3s;
    }
    #jakey:hover {
      background-color: #0056b8;
    }
    .message {
      color: #fff;
      font-family: Arial, sans-serif;
      font-size: 12px;
      opacity: 0;
      transition: opacity 0.3s;
      margin-left: 10px;
    }
    #jake:hover .message {
      opacity: 1;
    }
    #wigz {
      height: 20%;
      display: inline-block;
      align-items: center;
      justify-content: center;
      position: absolute;
      top: 30%;
      left: 41%;
      transform: translate(-50%, -50%);
    }
    #wigz .heading {
      font-family: 'UnifrakturMaguntia', cursive;
      font-size: 14px;
      text-align: center;
      position: relative;
      text-shadow: #00b3b3;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      width: 100%;
    }
    #wigz .heading span {
      display: inline-block;
      transition: transform 0.5s ease-in-out, color 0.5s ease-in-out;
      color: #00b3b3;
      border: 1px solid #800000;
      padding: 1px;
      margin: 1px;
      border-radius: 1px;
      box-shadow: 10px 10px 10px #00b3b3;
    }
    #wigz .heading span:hover {
      animation-name: move;
      animation-duration: 2s;
      animation-timing-function: ease-in-out;
      animation-iteration-count: infinite;
      color: yellow;
      background-color: #000;
      transform: rotate(440deg);
      box-shadow: #800000;
    }
    #subtitle {
      color: #00b3b3;
      font-family: Arial, sans-serif;
      font-size: 12px;
      text-align: center;
      margin-top: 5px;
    }
    @keyframes move {
      0% {
        transform: rotate(0) translateX(0);
      }
      50% {
        transform: rotate(180deg) translateX(40px);
      }
      100% {
        transform: rotate(0) translateX(0);
      }
    }
    .leah {
  display: inline-block;
  align-items: center;
  justify-content: center;
  height: 80vh;
  padding: 9px;
  position: absolute;
  top: 3px;
  right: 1px;
}
input[type="text"],
input[type="password"] {
  width: 40px;
  padding: 0px;
  margin-right: 0px;
  border-radius: 0px;
  background-color: #333;
  color: #fff;
  font-family: Arial, sans-serif;
  border: 1px dashed #800000;
  font-size: 6px;
}
input[type="text"]:focus,
input[type="password"]:focus {
  box-shadow: 0 0 3px #00b3b3;
  border: 1px dashed #800000;
}
.button:hover {
  transform: scale(2);
}
.button::before {
  content: "wer dat squeegee!";
  position: fixed;
  top: 19px;
  left: 50%;
  transform: translateX(-50%);
  background-color: #333;
  color: #fff;
  padding: 2px;
  border-radius: 2px;
  visibility: hidden;
  opacity: 0;
  transition: visibility 0s, opacity 0.5s linear;
  font-size: 10px;
  line-height: 1.2;
  z-index: 1000;
  white-space: nowrap;
  border: 1px dashed #800000;
  writing-mode: vertical-lr; /* Displays the text vertically */
  text-orientation: upright; /* Ensures upright orientation of characters */
}
.button:hover::before {
  visibility: visible;
  opacity: 1;
}
    .triangle-container {
      display: flex;
      justify-content: center;
      position: absolute;
      top: 0;
      left: 0;
      right: 340;
    }
    .triangle {
      width: 0;
      height: 0;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
      border-bottom: 10px solid #800000; /* Initial color */
      cursor: pointer;
      transition: background-color 0.5s, transform 0.5s;
    }
    .triangle.clicked {
      transform: translateX(200px); /* Adjust the desired distance */
    }
    .triangle:hover {
      background-color: #00b3b3;
    }
    .triangle:hover ~ .triangle {
      background-color: #800000;
    }
    .clock {
      position: absolute;
      top: 10px;
      left: 14px;
      font-size: 7px;
      cursor: pointer;
      color: white;
    }
    .clock {
      position: absolute;
      top: 10px;
      left: 14px;
      font-size: 7px;
      cursor: pointer;
      color: white;
    }
    .timer {
      position: absolute;
      top: 10px;
      left: 49px;
      font-size: 7px;
      color: white;
    }
    .button-container {
      position: absolute;
      top: 10.5px;
      left: 10px;
    }
    .button {
      display: inline-block;
      padding: 0px 0.5px;
      font-size: 5px;
      cursor: pointer;
      background: linear-gradient(to bottom, #800000, #00b3b3);
      color: #ffffff;
      border: none;
      border-radius: 0px;
      margin-right: 0px;
      margin-bottom: 0px;
    }
    .button:hover {
      background-color: #00b3b3;
      animation: pulse 1s infinite;
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }.nav-item {
  background-color: #30b3b3;
  width: 33px;
  height: 14px;
  color: white;
  text-align: center;
  font-size: 5px;
  font-family: Arial, sans-serif;
  cursor: pointer;
  transition: transform 0.5s, background-color 0.5s;
  overflow: hidden;
  border: 0.5px solid #800000;
  border-radius: 2px;
  box-sizing: border-box;
  margin-bottom: 2px;
  position: absolute;
}
.nav-item:nth-child(1) {
  top: 34px;
  left: 10px;
}
.nav-item:nth-child(2) {
  top: 50px;
  left: 10px;
}
.nav-item:hover:before {
  border-bottom: 2px solid #00b3b3; /* Adjusted border size for mobile devices */
  opacity: 1;
  transform: translate(-50%, -50%) rotate(45deg) scale(1.2);
}
.nav-item.clicked {
      transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
    }
    .nav-item:after {
      content: "";
      position: absolute;
      top: 10px;
      left: 10px;
      width: calc(100% - 4px);
      height: calc(100% - 4px);
      opacity: 0;
      border: 1px solid #00b3b3;
      transition: opacity 1.5s;
      pointer-events: none;
      mix-blend-mode: overlay;
    }
    .nav-item span.number {
      z-index: 3;
      color: black;
    }
    .nav-item .text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 1;
}
.nav-item i {
  font-size: 8px; /* Increased font size for mobile devices */
  position: relative;
  top: 18%;
  left: auto;
  transform: none;
    }
    #planet {
      position: absolute;
      bottom: 14;
      right: 14;
      width: 14px;
      height: 14px;
      border-radius: 50%;
      background: linear-gradient(#800000, #00b3b3);
      cursor: pointer;
      transition: transform 0.3s, right 0.3s, bottom 0.3s;
      box-shadow: 0px 0px 10px rgba(0, 88, 184, 0.5);
      transform-origin: center;
    }
    #planet:hover {
      transform: scale(1.2);
    }
    #popup {
      position: absolute;
      top: calc(100% + 20px);
      left: 50%;
      transform: translateX(-50%);
      width: 140px;
      padding: 1px;
      background: linear-gradient(#800000, #00b3b3);
      color: #ffffff;
      border-radius: 10px;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s, top 0.3s;
      text-align: center;
    }
    #planet:hover + #popup {
      opacity: 1;
      pointer-events: auto;
      top: calc(100% + 10px);
    }
    @media only screen and (max-width: 600px) {
    }@media screen and (max-width: 480px) {
      }@media only screen and (device-width: 375px) and (device-height: 812px) and (-webkit-device-pixel-ratio: 3) {
  }
@media only screen and (device-width: 360px) and (device-height: 800px) and (-webkit-device-pixel-ratio: 4) {
  }
  </style>
</head>
<header><div id="jake">
  <div id="jakey"></div>
  <div class="message">Hover me!</div></div>
<div id="wigz">
      <h1 class="heading">
        <span>L</span>
        <span>o</span>
        <span>f</span>
        <span>t</span>
        <span>i</span>
        <span>e</span>
        <span>s</span>
        <span>W</span>
        <span>i</span>
        <span>n</span>
        <span>d</span>
        <span>o</span>
        <span>w</span>
        <span>S</span>
      </h1>
      <div id="subtitle">Bringing Window Cleaning Online #LOFTIES</div>
    </div>
  <div class="leah">
    <div class="header-form">
      <input type="text" id="username" placeholder="Username" required>
      <input type="password" id="password" placeholder="Password" required>
      <button type="submit" id="login-button" class="button">Login</button>
      <button id="register-button" class="button">Register</button>
    </div>
  </div>
  <div class="triangle-container">
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
    <div class="triangle"></div>
  </div>
  <div id="clock" class="clock">00:00</div>
  <div id="timer" class="timer">00:00:00</div>
  <div class="button-container">
    <button id="format-toggle" class="button">Toggle Format</button>
    <button id="timer-start" class="button">Start</button>
    <button id="timer-reset" class="button">Reset</button>
  </div>
  <div class="container">
    <div class="nav-item" onclick="handleClick(event)">
      <i class="icon game-icon">&#x1F3AE;</i>
      <span class="text">LoftiesGames</span>
    </div>
    <div class="nav-item" onclick="handleClick(event)">
      <i class="icon video-icon">&#x1F3A5;</i>
      <span class="text">LoftiesVideos</span>
    </div>
  </div>
  <div id="container">
    <div id="planet" onclick="movePlanet()"></div>
    <div id="popup">
      <h2>Wer dat Squeegee</h2>
      <p>In cyberspace, a squeegee hides,
        Find its place, and luck abides.
        A window's gleam, the prize shall be,
        On this webpage, solve and see.</p>
    </div>
  </div>
</header>
<body>
<script>var jakey = document.getElementById("jakey");
    var message = document.querySelector(".message");
    jakey.addEventListener("click", function() {
      var randomColor = getRandomColor();
      jakey.style.backgroundImage = `radial-gradient(${randomColor}, #00b3b3)`;
    });
    function getRandomColor() {
      var letters = "0123456789ABCDEF";
      var color = "#";
      for (var i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }
document.getElementById("login-button").addEventListener("click", function() {
      var username = document.getElementById("username").value;
      var password = document.getElementById("password").value;
      // Perform login authentication logic here
      if (username === "admin" && password === "password") {
        alert("Login successful!");
        // Redirect to user dashboard or personalized page
      } else {
        alert("Invalid username or password. Please try again.");
      }
    });
// Redirect to sign up page
    document.getElementById("register-button").addEventListener("click", function() {
      window.location.href = "signup.html"; // Replace with your sign up page URL
    });
const triangles = document.querySelectorAll('.triangle');
triangles.forEach((triangle, index) => {
      triangle.addEventListener('click', () => {
        triangle.classList.toggle('clicked');
      });
    });
function getRandomColor() {
  var letters = "0123456789ABCDEF";
  var color = "#";
  for (var i = 0; i < 6; i++) {
    color += letters[Math.floor(Math.random() * 16)];
  }
  return color;
}
var buttons = document.getElementsByClassName("button");
for (var i = 0; i < buttons.length; i++) {
  buttons[i].addEventListener("mouseover", function() {
    this.style.backgroundColor = getRandomColor();
  });
  buttons[i].addEventListener("mouseout", function() {
    this.style.backgroundColor = "#800000";
  });
}
function getRandomColor() {
      var letters = "0123456789ABCDEF";
      var color = "#";
      for (var i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }
// Get all the buttons with the "button" class
    var buttons = document.getElementsByClassName("button");
// Loop through each button and attach event listeners for mouseover and mouseout
    for (var i = 0; i < buttons.length; i++) {
      buttons[i].addEventListener("mouseover", function() {
        this.style.backgroundColor = getRandomColor();
      });
buttons[i].addEventListener("mouseout", function() {
        this.style.backgroundColor = "#800000"; // Restores the default background color
      });
    }
var clock = document.getElementById("clock");
var timer = document.getElementById("timer");
var formatToggle = document.getElementById("format-toggle");
var timerStart = document.getElementById("timer-start");
var timerReset = document.getElementById("timer-reset");
formatToggle.addEventListener("click", function() {
  clock.classList.toggle("timer");
  timer.classList.toggle("clock");
});
timerStart.addEventListener("click", function() {
  });
timerReset.addEventListener("click", function() {
 });
function updateClock() {
  const clockElement = document.getElementById("clock");
  const date = new Date();
  let hours = date.getHours();
  let minutes = date.getMinutes();
  let ampm = "";
  if (is24HourFormat()) {
    hours = padZero(hours);
  } else {
    hours = convertTo12Hour(hours);
    ampm = hours >= 12 ? "PM" : "AM";
  }
  minutes = padZero(minutes);
  const time = `${hours}:${minutes} ${ampm}`;
  clockElement.textContent = time;
  clockElement.className = "clock";
}
function is24HourFormat() {
  return localStorage.getItem("format") === "24";
}
function toggleFormat() {
  const formatToggle = document.getElementById("format-toggle");
  formatToggle.addEventListener("click", function() {
    const currentFormat = localStorage.getItem("format");
    const newFormat = currentFormat === "24" ? "12" : "24";
    localStorage.setItem("format", newFormat);
    updateClock();
  });
}
function padZero(value) {
  return value.toString().padStart(2, "0");
}
function convertTo12Hour(hours) {
  return hours > 12 ? hours - 12 : hours;
}
let timerInterval;
let timerSeconds = 0;
function startTimer() {
  const timerElement = document.getElementById("timer");
  const timerStartButton = document.getElementById("timer-start");
  const timerResetButton = document.getElementById("timer-reset");
  timerStartButton.addEventListener("click", function() {
    if (timerInterval) {
      clearInterval(timerInterval);
      timerInterval = null;
      timerStartButton.textContent = "Start";
    } else {
      timerInterval = setInterval(function() {
        timerSeconds++;
        const hours = Math.floor(timerSeconds / 3600);
        const minutes = Math.floor((timerSeconds % 3600) / 60);
        const seconds = timerSeconds % 60;
        const time = `${padZero(hours)}:${padZero(minutes)}:${padZero(seconds)}`;
        timerElement.textContent = time;
      }, 1000);
      timerStartButton.textContent = "Pause";
    }
  });
  timerResetButton.addEventListener("click", function() {
    clearInterval(timerInterval);
    timerInterval = null;
    timerSeconds = 0;
    timerElement.textContent = "00:00:00";
    timerStartButton.textContent = "Start";
  });
}
function initializeClock() {
    localStorage.removeItem('format');
  updateClock();
  toggleFormat();
  startTimer();
}
initializeClock();
 var clickCount = 0;
function handleClick(event) {
      event.stopPropagation();
      clickCount++;
      var navItem = event.target.closest('.nav-item');
      var number = document.createElement('span');
      switch (clickCount) {
        case 1: number.textContent = 'Games'; break;
        case 2: number.textContent = 'Are'; break;
        case 3: number.textContent = 'Coming'; break;
        case 4: number.textContent = 'Soon'; break;
        case 5: number.textContent = 'I Hope'; break;
        default: number.textContent = clickCount; break;
      }
      number.className = 'number';
      navItem.innerHTML = '';
      navItem.appendChild(document.createElement('i')).className = 'icon';
      navItem.appendChild(number);
      animateNavItem(navItem);
      if (clickCount >= 5) window.location.href = "https://example.com";
    }
function animateNavItem(navItem) {
      navItem.classList.add('clicked');
      setTimeout(function() {
        navItem.classList.remove('clicked');
      }, 500);
    }
    function getRandomColor() {
      var letters = "0123456789ABCDEF";
      var color = "#";
      for (var i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }
    function movePlanet() {
      var planet = document.getElementById("planet");
      var currentPosition = parseInt(planet.style.left) || 0;
      var newPosition = currentPosition + 10;
      planet.style.left = newPosition + "px";
    }
    function getRandomPosition() {
      var headerWidth = document.querySelector('header').offsetWidth;
      var planetWidth = 50;
      var maxLeft = headerWidth - planetWidth;
      var randomLeft = Math.floor(Math.random() * maxLeft);
      return { left: randomLeft };
    }
    window.onload = function() {
      var planet = document.getElementById("planet");
      var popup = document.getElementById("popup");
      planet.style.backgroundColor = getRandomColor();
      var position = getRandomPosition();
      planet.style.right = position.right + "px";
      planet.style.bottom = position.bottom + "px";
      planet.onclick = function() {
        movePlanet();
        planet.style.backgroundColor = getRandomColor();
      };
    };
</script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lofties Windows</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>
    ul{list-style:none;}
    ul.social li{display:inline-block;margin:0 10px;}
    button{position:relative;font:bold 1.2rem sans-serif;color:#fff;background:#ff6600;border:none;border-radius:25px;padding:15px 30px;cursor:pointer;}
    .ball{width:50px;height:50px;border-radius:50%;background:#ffa500;opacity:0;position:absolute;left:14%;top:82%;transform:translate(-50%,-50%);z-index:-1;transition:all .5s ease-in-out;}
    .move{display:inline-block;color:transparent;text-shadow:0 0 5px #ffa500;}
    .move:hover{text-shadow:none;animation:move-text 14s ease-in-out;}
    @keyframes move-text{0%{transform:translate(0,0) rotate(0deg);}25%{transform:translate(100px,100px) rotate(90deg);}50%{transform:translate(-100px,100px) rotate(180deg);}75%{transform:translate(-100px,-100px) rotate(270deg);}100%{transform:translate(100px,-100px) rotate(360deg);}}
    button:focus+.ball{opacity:1;animation:move-ball 2s linear infinite;--x:.1;--y:.1;}
    @keyframes move-ball{to{transform:move-ball(calc(200vw * var(--x)),calc(200vh * var(--y)));}}
  </style>
</head>
<body>
  <h1><span class="move">L</span>of</span>ties<span class="move">W</span>indo<span class="move">w</span>s</h1>
  <button>Click me!</button>
  <div class="ball"></div>
  <ul class="social">
    <li><a href="#"><i class="icon1"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></i></a></li>
    <li><a href="#"><i class="icon4"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></i></a></li>
    <li><a href="#"><i class="icon3"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></i></a></li>
    <li><a href="#"><i class="icon4"><img src="https://img.icons8.com/clouds/64/000000/tiktok.png" alt="TikTok"></i></a></li>
  </ul></body>
</html>
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

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lofties Windows</title>
    <link
      rel="stylesheet"
      href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap"
    />
    <style>
      header {
        background-size: 100%;
        padding: 80px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-position: center 65%;
        font-family: "UnifrakturMaguntia";
        background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
        position: relative;
      }

      .triangle-container {
        display: flex;
        justify-content: center;
        align-items: flex-start;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        overflow: hidden;
      }

      .triangle {
        width: 9vw;
        height: 10vw;
        background-color: #FF0000;
        transform: rotate(45deg);
        margin: 0.0vw;
      }

      h1 {
        color: #00b3b3;
        font-size: 60px;
        margin: 0 0 10px;
        animation: fade-in-out 2s infinite;
      }

      h1 span {
        display: inline-block;
        position: relative;
        transition: transform 1s ease-out;
      }

      h1 span:hover {
        transform: translateX(30px);
      }

      p {
        color: #00b3b3;
        font-size: 20px;
        margin: 0;
        padding: 5px;
        border: 1px solid #800000;
        transition: all 0.5s ease-out;
        position: relative;
      }

      p:hover {
        color: #00b3b3;
        border: 2px solid #00b3b3;
        box-shadow: 0 0 10px #800000;
      }

      p:hover .star {
        opacity: 1;
      }

      .star {
        position: absolute;
        width: 14px;
        height: 14px;
        background-color: black;
        border-radius: 50%;
        opacity: 0;
        transition: all 1s ease-out;
      }

      .star:hover {
        transform: scale(3);
      }

      .star1 {
        top: 0%;
        left: 5%;
      }

      .star2 {
        top: 50%;
        left: 45%;
      }
    </style>
  </head>
  <body>
    <header>
      <div class="triangle-container">
        <canvas id="canvas"></canvas>
      </div>
      <h1><span>L</span>ofties<span>W</span>indows</h1>
      <p>
        Attention all window lovers! Search our website for the squeegee and win a
        free clean!
        <span class="star star1">&#9733;</span>
        <span class="star star2">&#9733;</span>
<span class="star star3">★</span>
</p>
</header>
<script>
      window.addEventListener('load', () => {
        const canvas = document.getElementById('canvas');
        const context = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = 100;
        const numOfTriangles = 14;
        const triangleWidth = canvas.width / numOfTriangles;
        const triangleHeight = Math.sqrt(0.2) / 2 * triangleWidth;
        const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
        for (let i = 0; i < numOfTriangles; i++) {
          context.beginPath();
          context.moveTo(i * triangleWidth, 0);
          context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
          context.lineTo((i + 1) * triangleWidth, 0);
          context.closePath();
          context.fillStyle = triangleColors[i % triangleColors.length];
          context.fill();
		  window.addEventListener('load', () => {
        const canvas = document.getElementById('canvas');
        const context = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
        const numOfTriangles = 14;
        const triangleWidth = canvas.width / numOfTriangles;
        const triangleHeight = Math.sqrt(0.5) / 2 * triangleWidth;
        const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
        for (let i = 0; i < numOfTriangles; i++) {
          context.beginPath();
          context.moveTo(i * triangleWidth, 0);
          context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
          context.lineTo((i + 1) * triangleWidth, 0);
          context.closePath();
          context.fillStyle = triangleColors[i % triangleColors.length];
          context.fill();
        }
      });
        }
      });
    </script>
  </body>
</html>

<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lofties Windows</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>header {
  background-size:100%;
  padding:80px;
  display:flex;
  background-position:center 65%;
  font-family: 'UnifrakturMaguntia';
  justify-content:space-between;
  align-items:center;
  background-image:url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
  position:relative;
} canvas {
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 4;
} h1{
  color: #00b3b3;
  font-size: 30px;
  margin: 0 0 10px;
  animation: fade-in-out 2s infinite;
}  h1 span {
  display: inline-block;
  position: relative;
  transition: transform 1s ease-out;
}h1 span:hover {
  transform: translateX(30px);
}p {
  color: #00b3b3;
  font-size: 10px;
  margin: 0;
  padding: 5px;
  border: 1px solid #800000;
  transition: all 0.5s ease-out;
  position: relative;
}p:hover {
  color: #00b3b3;
  border: 2px solid #00b3b3;
  box-shadow: 0 0 10px #800000;
}p:hover .star {
  opacity: 1;
}.star {
  position: absolute;
  width: 14px;
  height: 14px;
  background-color: black;
  border-radius: 50%;
  opacity: 0;
  transition: all 1s ease-out;
}.star:hover {
  transform: scale(3);
}.star1 {
  top: 0%;
  left: 5%;
}.star2 {
  top: 50%;
  left: 45%;
}.social-icons-container {
  position: absolute;
  top: 14px;
  left: 14px;
  display: flex;
  flex-direction: column;
  gap: 2px;
}.social-icons-container img {
  height: 14px;
  width: 14px;
  margin: 3px;
  filter: brightness(60%);
  transition: filter 0.3s ease-in-out;
  display: flex;
  justify-content: center;
  align-items: center;
  border: none; 
}.social-icons-container img:hover {
  filter: brightness(100%);
}.bottom-right {
  position: absolute;
  bottom: 0;
  right: 0;
  display: flex;
  gap: 1px;
}.bottom-right li {
  list-style:none;
  }@keyframes fade-in-out {
        0% { opacity: 1; }
        50% { opacity: 0.5; }
        100% { opacity: 1; }          
	}@keyframes bounce {
        0% {
          left: 0%;
        }
        100% {
          left: 100%;
        }
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
    }@keyframes zoomInRight{
      0% {
        opacity: 0;
        transform: scale(0.1) translateX(200%);
      }
      100% {
        opacity: 1;
        transform: scale(1) translateX(0);
      } @media only screen and (max-width: 600px) {
  }}</style>
</head>
<body>
  <header><canvas id="canvas"></canvas><div class="social-icons-container">
      <a href="https://www.facebook.com"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></a>
      <a href="https://www.discord.com"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></a>
      <a href="https://www.youtube.com"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></a>
    </div>
    <ul class="bottom-right">
      <jake><a href="#contact" class="video-tab"><span class="icon video-icon">&#x1F3A5;</span>Videos</a></jake>
      <jake><a href="#contact" class="music-tab"><span class="icon music-icon">&#x1F3B5;</span>Music</a></jake>
      <jake><a href="#contact" class="game-tab"><span class="icon game-icon">&#x1F3AE;</span>Games</a></jake>
    </ul><h1><span>L</span>ofties<span>W</span>indows</h1>
      <p>Attention all window lovers! Search our website for the squeegee and win a free clean!
        <span class="star star1">&#9733;</span>
        <span class="star star2">&#9733;</span>
        <span class="star star3">&#9733;</span>
      </p>
  </header><script>
      window.addEventListener('load', () => {
        const canvas = document.getElementById('canvas');
        const context = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = 100;
        const numOfTriangles = 14;
        const triangleWidth = canvas.width / numOfTriangles;
        const triangleHeight = Math.sqrt(0.2) / 2 * triangleWidth;
        const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
        for (let i = 0; i < numOfTriangles; i++) {
          context.beginPath();
          context.moveTo(i * triangleWidth, 0);
          context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
          context.lineTo((i + 1) * triangleWidth, 0);
          context.closePath();
          context.fillStyle = triangleColors[i % triangleColors.length];
          context.fill();
		  window.addEventListener('load', () => {
        const canvas = document.getElementById('canvas');
        const context = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
        const numOfTriangles = 14;
        const triangleWidth = canvas.width / numOfTriangles;
        const triangleHeight = Math.sqrt(0.5) / 2 * triangleWidth;
        const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
        for (let i = 0; i < numOfTriangles; i++) {
          context.beginPath();
          context.moveTo(i * triangleWidth, 0);
          context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
          context.lineTo((i + 1) * triangleWidth, 0);
          context.closePath();
          context.fillStyle = triangleColors[i % triangleColors.length];
          context.fill();
        }
      });
        }
      });
    </script>
  </body>
</html>

<html><head>
  <style>
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=750&q=80");
      background-size: cover;
      background-position: center;
      padding: 90px;
    }.leah {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      justify-content: flex-start;
      height: 80vh;
      background-color: #f5f5f5;
      padding: 10px;
    }
    .header-form {
      display: flex;
      align-items: flex-start;
      justify-content: flex-end;
      height: 60px;
      position: absolute;
      top: 5;
      right: 5;
      padding: 2px;
      box-sizing: border-box;
    }
    input[type="text"],
    input[type="password"] {
      width: 50px;
      padding: 1px;
      margin-right: 1px;
      border-radius: 1px;
      background-color: #333;
      color: #fff;
      font-family: Arial, sans-serif;
      border: 1px dashed #800000;
      font-size: 8px;
    }
    input[type="text"]:focus,
    input[type="password"]:focus {
      box-shadow: 0 0 3px #00b3b3;
      border: 1px dashed #800000;
    }
    .button {
      padding: 1px 3px;
      color: #fff;
      border: 1px double #800000;
      border-radius: 8px;
      cursor: pointer;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #800000, #00b3b3);
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.2);
      position: relative;
      font-size: 7.5px;
    }
    .button:hover {
      transform: scale(1.05);
    }
    .button::before {
      content: "Scrub away your worries and find the perfect squeegee for a crystal-clear view!";
      position: absolute;
      top: 18px;
      left: 50%;
      transform: translateX(-95%);
      background-color: #333;
      color: #fff;
      padding: 0px;
      border-radius: 4px;
      visibility: hidden;
      opacity: 0;
      transition: visibility 0s, opacity 0.5s linear;
      font-size: 10px;
      line-height: 1.2;
      white-space: nowrap;
      border: 1px dashed #800000;
    }
    .button:hover::before {
      visibility: visible;
      opacity: 1;
    }
    .triangle-container {
      display: flex;
      justify-content: center;
      position: absolute;
      top: 0;
      left: 0;
      right: 340;
    }
    .triangle {
      width: 0;
      height: 0;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
      border-bottom: 10px solid #800000; /* Initial color */
      cursor: pointer;
      transition: background-color 0.5s, transform 0.5s;
    }
    .triangle.clicked {
      transform: translateX(200px); /* Adjust the desired distance */
    }
    .triangle:hover {
      background-color: #00b3b3;
    }
    .triangle:hover ~ .triangle {
      background-color: #800000;
    }
    .clock {
      position: absolute;
      top: 10px;
      left: 14px;
      font-size: 7px;
      cursor: pointer;
      color: white;
    }
    .clock {
      position: absolute;
      top: 10px;
      left: 14px;
      font-size: 7px;
      cursor: pointer;
      color: white;
    }
    .timer {
      position: absolute;
      top: 10px;
      left: 49px;
      font-size: 7px;
      color: white;
    }
    .button-container {
      position: absolute;
      top: 10.5px;
      left: 10px;
    }
    .button {
      display: inline-block;
      padding: 0px 0.5px;
      font-size: 5px;
      cursor: pointer;
      background-color: #00b3b3;
      color: #ffffff;
      border: none;
      border-radius: 0px;
      margin-right: 0px;
      margin-bottom: 0px;
    }
    .button:hover {
      background-color: #00b3b3;
      animation: pulse 1s infinite;
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }.nav-item {
  background-color: #30b3b3;
  width: 33px;
  height: 14px;
  color: white;
  text-align: center;
  font-size: 5px;
  font-family: Arial, sans-serif;
  cursor: pointer;
  transition: transform 0.5s, background-color 0.5s;
  overflow: hidden;
  border: 0.5px solid #800000;
  border-radius: 2px;
  box-sizing: border-box;
  margin-bottom: 2px;
  position: absolute;
}
.nav-item:nth-child(1) {
  top: 34px;
  left: 10px;
}
.nav-item:nth-child(2) {
  top: 50px;
  left: 10px;
}
.nav-item:hover:before {
  border-bottom: 2px solid #00b3b3; /* Adjusted border size for mobile devices */
  opacity: 1;
  transform: translate(-50%, -50%) rotate(45deg) scale(1.2);
}
.nav-item.clicked {
      transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
    }
    .nav-item:after {
      content: "";
      position: absolute;
      top: 10px;
      left: 10px;
      width: calc(100% - 4px);
      height: calc(100% - 4px);
      opacity: 0;
      border: 1px solid #00b3b3;
      transition: opacity 1.5s;
      pointer-events: none;
      mix-blend-mode: overlay;
    }
    .nav-item span.number {
      z-index: 3;
      color: black;
    }
    .nav-item .text {
  position: absolute;
  top: 14%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.nav-item i {
  font-size: 7px; /* Increased font size for mobile devices */
  position: relative;
  top: 28%;
  left: auto;
  transform: none;
    }
    #planet {
      position: absolute;
      bottom: 14;
      right: 14;
      width: 14px;
      height: 14px;
      border-radius: 50%;
      background: linear-gradient(#800000, #00b3b3);
      cursor: pointer;
      transition: transform 0.3s, right 0.3s, bottom 0.3s;
      box-shadow: 0px 0px 10px rgba(0, 88, 184, 0.5);
      transform-origin: center;
    }
    #planet:hover {
      transform: scale(1.2);
    }
    #popup {
      position: absolute;
      top: calc(100% + 20px);
      left: 50%;
      transform: translateX(-50%);
      width: 140px;
      padding: 1px;
      background: linear-gradient(#800000, #00b3b3);
      color: #ffffff;
      border-radius: 10px;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s, top 0.3s;
      text-align: center;
    }
    #planet:hover + #popup {
      opacity: 1;
      pointer-events: auto;
      top: calc(100% + 10px);
    }
    @media only screen and (max-width: 600px) {
    }
  </style>
</head>
<header><div class="leah">
    <div class="header-form">
      <input type="text" id="username" placeholder="Username" required>
      <input type="password" id="password" placeholder="Password" required>
      <button type="submit" id="login-button" class="button">Login</button>
      <button id="register-button" class="button">Register</button>
    </div>
  </div>
<div class="triangle-container">
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
    </div>
  <div id="clock" class="clock">00:00</div>
  <div id="timer" class="timer">00:00:00</div>
  <div class="button-container">
    <button id="format-toggle" class="button">Toggle Format</button>
    <button id="timer-start" class="button">Start</button>
    <button id="timer-reset" class="button">Reset</button>
  </div>
  <div class="container">
    <div class="nav-item" onclick="handleClick(event)">
      <i class="icon game-icon">&#x1F3AE;</i>
      <span class="text">LoftiesGames</span>
    </div>
    <div class="nav-item" onclick="handleClick(event)">
      <i class="icon video-icon">&#x1F3A5;</i>
      <span class="text">LoftiesVideos</span>
    </div>
  </div>
  <div id="container">
    <div id="planet" onclick="movePlanet()"></div>
    <div id="popup">
      <h2>Wer dat Squeegee</h2>
      <p>In cyberspace, a squeegee hides,
Find its place, and luck abides.
A window's gleam, the prize shall be,
On this webpage, solve and see.</p>
    </div>
  </div>
</header>
<body>
<script>document.getElementById("login-button").addEventListener("click", function() {
      var username = document.getElementById("username").value;
      var password = document.getElementById("password").value;
      // Perform login authentication logic here
      if (username === "admin" && password === "password") {
        alert("Login successful!");
        // Redirect to user dashboard or personalized page
      } else {
        alert("Invalid username or password. Please try again.");
      }
    });
// Redirect to sign up page
    document.getElementById("register-button").addEventListener("click", function() {
      window.location.href = "signup.html"; // Replace with your sign up page URL
    });
const triangles = document.querySelectorAll('.triangle');
triangles.forEach((triangle, index) => {
      triangle.addEventListener('click', () => {
        triangle.classList.toggle('clicked');
      });
    });
function getRandomColor() {
  var letters = "0123456789ABCDEF";
  var color = "#";
  for (var i = 0; i < 6; i++) {
    color += letters[Math.floor(Math.random() * 16)];
  }
  return color;
}
var buttons = document.getElementsByClassName("button");
for (var i = 0; i < buttons.length; i++) {
  buttons[i].addEventListener("mouseover", function() {
    this.style.backgroundColor = getRandomColor();
  });
  buttons[i].addEventListener("mouseout", function() {
    this.style.backgroundColor = "#800000";
  });
}
function getRandomColor() {
  var letters = "0123456789ABCDEF";
  var color = "#";
  for (var i = 0; i < 6; i++) {
    color += letters[Math.floor(Math.random() * 16)];
  }
  return color;
}
var buttons = document.getElementsByClassName("button");
for (var i = 0; i < buttons.length; i++) {
  buttons[i].addEventListener("mouseover", function() {
    this.style.backgroundColor = getRandomColor();
  });
  buttons[i].addEventListener("mouseout", function() {
    this.style.backgroundColor = "#800000";
  });
}
var clock = document.getElementById("clock");
var timer = document.getElementById("timer");
var formatToggle = document.getElementById("format-toggle");
var timerStart = document.getElementById("timer-start");
var timerReset = document.getElementById("timer-reset");
formatToggle.addEventListener("click", function() {
  clock.classList.toggle("timer");
  timer.classList.toggle("clock");
});
timerStart.addEventListener("click", function() {
  });
timerReset.addEventListener("click", function() {
 });
function updateClock() {
  const clockElement = document.getElementById("clock");
  const date = new Date();
  let hours = date.getHours();
  let minutes = date.getMinutes();
  let ampm = "";
  if (is24HourFormat()) {
    hours = padZero(hours);
  } else {
    hours = convertTo12Hour(hours);
    ampm = hours >= 12 ? "PM" : "AM";
  }
  minutes = padZero(minutes);
  const time = `${hours}:${minutes} ${ampm}`;
  clockElement.textContent = time;
  clockElement.className = "clock";
}
function is24HourFormat() {
  return localStorage.getItem("format") === "24";
}
function toggleFormat() {
  const formatToggle = document.getElementById("format-toggle");
  formatToggle.addEventListener("click", function() {
    const currentFormat = localStorage.getItem("format");
    const newFormat = currentFormat === "24" ? "12" : "24";
    localStorage.setItem("format", newFormat);
    updateClock();
  });
}
function padZero(value) {
  return value.toString().padStart(2, "0");
}
function convertTo12Hour(hours) {
  return hours > 12 ? hours - 12 : hours;
}
let timerInterval;
let timerSeconds = 0;
function startTimer() {
  const timerElement = document.getElementById("timer");
  const timerStartButton = document.getElementById("timer-start");
  const timerResetButton = document.getElementById("timer-reset");
  timerStartButton.addEventListener("click", function() {
    if (timerInterval) {
      clearInterval(timerInterval);
      timerInterval = null;
      timerStartButton.textContent = "Start";
    } else {
      timerInterval = setInterval(function() {
        timerSeconds++;
        const hours = Math.floor(timerSeconds / 3600);
        const minutes = Math.floor((timerSeconds % 3600) / 60);
        const seconds = timerSeconds % 60;
        const time = `${padZero(hours)}:${padZero(minutes)}:${padZero(seconds)}`;
        timerElement.textContent = time;
      }, 1000);
      timerStartButton.textContent = "Pause";
    }
  });
  timerResetButton.addEventListener("click", function() {
    clearInterval(timerInterval);
    timerInterval = null;
    timerSeconds = 0;
    timerElement.textContent = "00:00:00";
    timerStartButton.textContent = "Start";
  });
}
function initializeClock() {
    localStorage.removeItem('format');
  updateClock();
  toggleFormat();
  startTimer();
}
initializeClock();
 var clickCount = 0;
function handleClick(event) {
      event.stopPropagation();
      clickCount++;
      var navItem = event.target.closest('.nav-item');
      var number = document.createElement('span');
      switch (clickCount) {
        case 1: number.textContent = 'Games'; break;
        case 2: number.textContent = 'Are'; break;
        case 3: number.textContent = 'Coming'; break;
        case 4: number.textContent = 'Soon'; break;
        case 5: number.textContent = 'I Hope'; break;
        default: number.textContent = clickCount; break;
      }
      number.className = 'number';
      navItem.innerHTML = '';
      navItem.appendChild(document.createElement('i')).className = 'icon';
      navItem.appendChild(number);
      animateNavItem(navItem);
      if (clickCount >= 5) window.location.href = "https://example.com";
    }
function animateNavItem(navItem) {
      navItem.classList.add('clicked');
      setTimeout(function() {
        navItem.classList.remove('clicked');
      }, 500);
    }
    function getRandomColor() {
      var letters = "0123456789ABCDEF";
      var color = "#";
      for (var i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }
    function movePlanet() {
      var planet = document.getElementById("planet");
      var currentPosition = parseInt(planet.style.left) || 0;
      var newPosition = currentPosition + 10;
      planet.style.left = newPosition + "px";
    }
    function getRandomPosition() {
      var headerWidth = document.querySelector('header').offsetWidth;
      var planetWidth = 50;
      var maxLeft = headerWidth - planetWidth;
      var randomLeft = Math.floor(Math.random() * maxLeft);
      return { left: randomLeft };
    }
    window.onload = function() {
      var planet = document.getElementById("planet");
      var popup = document.getElementById("popup");
      planet.style.backgroundColor = getRandomColor();
      var position = getRandomPosition();
      planet.style.right = position.right + "px";
      planet.style.bottom = position.bottom + "px";
      planet.onclick = function() {
        movePlanet();
        planet.style.backgroundColor = getRandomColor();
      };
    };
</script>
</body>
</html>



<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Exo:100,200,400,italic">

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    
    body {
      font-family: 'Exo', sans-serif;
      background: linear-gradient(135deg, #ffffff, #00b3b3);
    }
    
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
      background-size: cover;
      padding: 40px;
      text-align: center;
      color: #FFF;
      margin: 0;
    }
    
    #clock {
      font-size: 9px;
      position: absolute;
      top: 2px;
      left: 2px;
    }
    
    #date {
      font-size: 9px;
      position: absolute;
      top: 14px;
      left: 2px;
    }
    
    #launch {
      color: #00b3b3;
      text-shadow: 1px 1px 2px #00b3b3;
      border: 1px solid #00b3b3;
      border-radius: 8px;
      padding: 1px;
      font-size: 9px;
      position: absolute;
      top: 28px;
      left: 2px;
    }
    
    #countdown-text {
      font-size: 10px;
      position: absolute;
      top: 55px;
      left: 35px;
      opacity: 0; 
      transition: opacity 0.3s ease-in-out;
    }
    
    #countdown:hover #countdown-text {
      opacity: 1; 
    }
    
    #space-x-logo {
      color: #00b3b3;
      text-shadow: 1px 1px 2px #00b3b3;
      border: 1px solid #00b3b3;
      border-radius: 8px;
      padding: 1px;
      max-width: 40px;
      position: absolute;
      top: 45px;
      left: 10px;
    }
    
    .login-register {
      background-color: white;
      padding: 2px;
      font-size: 10px;
      position: absolute;
      top: 10px;
      right: 8px;
      border-radius: 2px;
      box-shadow: 0px 0px 5px #00b3b3;
    }
    
    .login-register a {
      color: #1abc9c;
      text-decoration: none;
      margin-left: 1px;
    }
    
    .login-register a:hover {
      color: #2ecc71;
    }
    
    .letter {
      display: inline-block;
      cursor: pointer;
      transition: transform 0.5s;
    }
    
    .letter.active {
      animation-name: neon-glow;
      animation-duration: 2s;
      animation-iteration-count: infinite;
      animation-fill-mode: forwards;
    }
    
    .heading {
      text-align: center;
      font-size: 14px;
      -webkit-text-stroke: 0.7px white;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #00b3b3, #00b3b3, #00b3b3);
      -webkit-background-clip: text;
      padding: 5px;
      transition: all 0.5s ease;
      margin-bottom: -20px;
      font-weight: bold;
      letter-spacing: 1px;
      line-height: 1;
      animation: neon-glow 2s ease-in-out infinite alternate;
    }
    
    .heading:hover {
      transform: scale(1.1);
      text-shadow: 0px 5px 10px rgba(0, 0, 0, 0.5), 0px 0px 20px #00b3b3;
    }
    
    .subheading {
      text-align: center;
      font-size: 20px;
      -webkit-text-stroke: 0.2px #000;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #FF0066, #FF00FF, #6600FF, #00CCFF, #00FF66, #FFFF00, #FF0066);
      -webkit-background-clip: text;
      padding: 10px;
      transition: all 0.5s ease;
      margin-top: 20px;
      font-weight: normal;
      letter-spacing: 1px;
      cursor: pointer;
      line-height: 1.2;
      text-shadow: 0px 0px 20px rgba(255, 255, 255, 0.8), 0px 0px 40px rgba(255, 255, 255, 0.8);
    }
    
    .subheading:hover {
      transform: scale(1.1);
      text-shadow: 0px 5px 10px rgba(0, 0, 0, 0.5), 0px 0px 30px #00b3b3, 0px 0px 50px rgba(255, 255, 255, 0.8);
    }
    
    .social {
      list-style: none;
      position: absolute;
      padding: 1px;
      bottom: 2px;
      left: 5px;
    }
    
    .social li {
      display: flex;
      align-items: center;
      margin-bottom: 5px; 
    }
    
    .social li a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: black;
      transition: transform 0.3s ease-in-out;
      position: relative;
    }
    
    .social li a:hover {
      transform: scale(1.7);
    }
    
    .social li a img {
      display: inline-block;
      vertical-align: middle;
      transition: transform 0.3s ease-in-out;
      background: transparent;
      width: 18px;
      height: 18px;
      margin-right: 4px;
      filter: brightness(1);
    }
    
    .text-box {
      position: absolute;
      text-align: center;
      font-size: 8px;top: -10px;
      left: 7px;
      -webkit-text-stroke: 0.2px #000;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #FF0066, #FF00FF, #6600FF, #00CCFF, #00FF66, #FFFF00, #FF0066);
      -webkit-background-clip: text;
      padding: 2px;
      transition: all 0.5s ease;
      white-space: nowrap;
      display: none; 
    }
    
    .social li a:hover .text-box {
      text-align: center;
      font-size: 8px;
      position: absolute;
      top: -10px;
      left: 7px;
      -webkit-text-stroke: 0.2px #000;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #FF0066, #FF00FF, #6600FF, #00CCFF, #00FF66, #FFFF00, #FF0066);
      -webkit-background-clip: text;
      padding: 10px;
      transition: all 0.5s ease;
      display: block; 
      opacity: 1;
    }

    .competition {
      position: absolute;
      bottom: 2px;
      right: 2px;
      padding: 5px;
      border-radius: 5px;
      color: #00b3b3;
      cursor: pointer;
      font-size: 13px;
      font-weight: bold;
      font-style: italic;
      font-family: 'Exo 2', sans-serif;
      transition: background-color 0.9s, transform 0.9s;
    }
    
    .competition:hover {
      background-color: #FFF;
      transform: scale(1);
      transition: background-color 0.9s, transform 0.9s;
    }
    
    .competition:hover .competition-text {
      display: block;
      animation: pulse 7.5s infinite;
    }
    
    .competition-text {
      display: none;
      background-color: #FFF;
      font-size: 9px;
      border-radius: 5px;
      transition: background-color 0.9s, transform 0.9s;
    }

    @keyframes pulse {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.1);
      }
      100% {
        transform: scale(1);
      }
    }

   .side-menu {
      position: fixed;
      width: 0;
      height: 100%;
      background: linear-gradient(135deg, #00b3b3, #ffffff);
      z-index: 2;
      overflow-x: hidden;
      transition: width 0.3s;
    }

    .menu-button {
      width: 0;
      height: 0;
      border-style: solid;
      border-width: 28px 0 28px 28px;
      border-color: transparent transparent transparent #00b3b3;
      transition: border-color 0.3s;
      cursor: pointer;
      transform-origin: center center;
      position: fixed;
      z-index: 3;
    }

    .menu-button:before {
      content: "";
      position: absolute;
      top: -28px;
      left: -28px;
      width: 0;
      height: 0;
      border-style: solid;
      border-width: 28px 0 28px 28px;
      border-color: transparent transparent transparent #00b3b3;
      transition: border-color 0.3s;
      transform-origin: center center;
      transform: rotate(-90deg);
      z-index: -1;
    }

    .menu-button:after {
      content: "";
      position: absolute;
      bottom: -28px;
      left: -28px;
      width: 0;
      height: 0;
      border-style: solid;
      border-width: 28px 0 28px 28px;
      border-color: transparent transparent transparent #00b3b3;
      transition: border-color 0.3s;
      transform-origin: center center;
      transform: rotate(90deg);
      z-index: -1;
    }

    .menu-button:hover,
    .menu-button:before,
    .menu-button:after {
      border-color: transparent transparent transparent #ffffff;
    }

    .menu-button.right {
      transform: rotate(180deg);
      right: 0;
    }

    .left-side-menu {
      left: 0;
    }

    .right-side-menu {
      right: 0;
    }

    .side-menu-content {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100%;
    }
    
    .side-menu-content button {
      background-color: #00b3b3;
      color: #ffffff;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 5px;
      margin-top: 20px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    
    .side-menu-content button:hover {
      background-color: #008080;
    }
    
    .side-menu-content button:focus {
      outline: none;
    }

    .left-side-menu .close-button,
    .right-side-menu .close-button {
      position: absolute;
      top: 10px;
      font-size: 24px;
      color: #ffffff;
      background-color: transparent;
      border: none;
      cursor: pointer;
      transition: transform 0.3s;
    }

    .left-side-menu .close-button:before,
    .right-side-menu .close-button:before {
      content: "×";
    }

    .left-side-menu .close-button:hover,
    .right-side-menu .close-button:hover {
      transform: rotate(90deg);
    }

    .left-side-menu .close-button:focus,
    .right-side-menu .close-button:focus {
      outline: none;
    }

    .left-side-menu .close-button:focus:before,
    .right-side-menu .close-button:focus:before {
      transform: rotate(0);
    }.section-container {
      max-width: 800px;
      margin: 0 auto;
      padding: 40px;
      background-color: transparent;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    h1 {
      font-size: 48px;
      font-weight: bold;
      color: #ffffff;
      text-align: center;
      margin-bottom: 40px;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    }

    .paragraph-wrapper {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

    .paragraph {
      font-size: 18px;
      color: #ffffff;
      text-align: justify;
      line-height: 1.8;
      padding: 10px;
      background-color: rgba(0, 179, 179, 0.2);
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .body-button {
      display: block;
      margin: 30px auto;
      padding: 18px 36px;
      background-color: #ffffff;
      color: #00b3b3;
      font-size: 20px;
      font-weight: bold;
      border-radius: 30px;
      text-align: center;
      text-decoration: none;
      transition: background-color 0.3s;
      border: none;
      cursor: pointer;
      outline: none;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    .body-button:hover {
      background-color: #e5e5e5;
    }

    .additional-items {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 30px;
      margin-top: 40px;
    }

    .additional-item {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 10px;
    }

    .additional-icon {
      font-size: 36px;
      color: #ffffff;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    }

    .additional-text {
      font-size: 16px;
      color: #ffffff;
      font-weight: bold;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    }
  
  footer {
    background-color: #222;
    padding: 30px 0;
    color: #FFF;
    text-align: center;
  }

  .footer-container {
    max-width: 800px;
    margin: 0 auto;
  }

  .footer-info,
  .footer-links,
  .footer-social {
    width: 33.33%;
    display: inline-block;
    text-align: center;
  }

  .footer-info h3,
  .footer-links h3,
  .footer-social h3 {
    font-size: 9px;
    margin-bottom: 10px;
  }

  .footer-links ul {
    list-style: none;
    padding-left: 0;
  }

  .footer-links li {
    margin-bottom: 5px;
  }

  .footer-links a {
    color: #CCC;
    text-decoration: none;
  }

  .footer-links a:hover {
    color: #FFF;
  }

  .footer-social ul {
    list-style: none;
    padding-left: 0;
  }

  .footer-social li {
    display: inline-block;
    margin-right: 10px;
  }

  .footer-social img {
    width: 30px;
    height: 30px;
  }

  .footer-bottom {
    background-color: #111;
    padding: 10px 0;
    text-align: center;
  }

  .footer-bottom p {
    margin: 0;
    font-size: 9px;
  }
  </style>
</head>
<body>
  <header>
    <div id="countdown">
      <div id="clock"></div>
      <div id="date"></div>
      <div id="launch"></div>
      <div id="countdown-text">Space-X Countdown to Next Take-Off<br>Mars Soon</div>
    </div>
    <div class="social">
      <ul> 
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
            <div class="text-box">
              <p>Check out our YouTube channel for clues on the squeegee hunt!</p>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/discord-logo.png" alt="Discord">
            <div class="text-box">
              <p>Join our Discord server and collaborate to uncover the squeegee!</p>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
            <div class="text-box">
              <p>Follow our Facebook page to find the elusive squeegee adventure!</p>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram">
            <div class="text-box">
              <p>Explore our Instagram feed for hints leading to the squeegee treasure!</p>
            </div>
          </a>
        </li>
      </ul>
    </div>
    <img id="space-x-logo" src="https://upload.wikimedia.org/wikipedia/commons/d/de/SpaceX-Logo.svg" alt="SpaceX Logo">
    <div class="login-register">
      <a href="#">Login</a>
      <a href="#">Register</a>
    </div>
    <h1 class="heading">LoftieswindowS</h1>
    <div class="subheading">Bringing Window Cleaning Online #Lofties</div>
    <div id="planet"></div><div class="competition">
      <span>🌟Free Window Clean🌟</span>
      <div class="competition-text">Unleash your inner adventurer,<br> hunt the elusive squeegee on our webpage ,<br> and unlock a FREE window clean! Are you ready?<br> Let the pursuit begin!</div>
    </div>
  </header>
  <div class="menu-button left" onclick="openSideMenu('left')"></div>

  <div class="menu-button right" onclick="openSideMenu('right')"></div>

  <div id="left-side-menu" class="side-menu left-side-menu">
    <div class="side-menu-content">
      <i class="fas fa-window-cleaner"></i>
      <h2>Window Cleaning Services</h2>
      <p>We specialize in high-quality window cleaning services. Our experienced team uses traditional methods with a ladder and bucket to ensure sparkling clean windows for your home or business.</p>
      <p>With meticulous attention to detail, we are able to clean even the window sills, providing a thorough cleaning experience.</p>
      <p>As a bonus, we've hidden a squeegee somewhere on this webpage. Can you find it behind the words or the planets and stars?</p>
      <button class="book-now-button">Book Now</button>
      <button class="close-button" onclick="closeSideMenu('left')">&times;</button>
    </div>
  </div>

  <div id="right-side-menu" class="side-menu right-side-menu">
    <div class="side-menu-content">
      <i class="fas fa-gutter-cleaning"></i>
      <h2>Gutter Cleaning Services</h2>
      <p>In addition to window cleaning, we also offer gutter cleaning services to keep your property well-maintained. Our professional team ensures your gutters are free from debris and functioning optimally.</p>
      <p>By maintaining clean and clear gutters, you can prevent potential damage to your roof, walls, and foundation.</p>
      <p>Protect your investment and maintain the integrity of your property by scheduling regular gutter cleanings with us.</p>
      <button class="get-quote-button">Get a Quote</button>
      <button class="close-button" onclick="closeSideMenu('right')">&times;</button>
    </div>
  </div>
  
<section class="section-container">
    <h1>Discover Sparkling Windows</h1>
    <div class="paragraph-wrapper">
      <div class="paragraph">Experience a window cleaning service like no other. Our dedicated team of professionals goes above and beyond to make your windows shine.</div>
      <div class="paragraph">With our advanced techniques and attention to detail, we leave no streaks or smudges behind. Enjoy crystal-clear views and let the natural light brighten up your space.</div>
      <div class="paragraph">From residential to commercial properties, our top-notch service is tailored to meet your specific needs. We take pride in delivering exceptional results and ensuring your complete satisfaction.</div>
      <div class="paragraph">Transform your windows into sparkling portals that radiate beauty and elegance. Discover the transformative power of clean windows with our reliable and professional service.</div>
    </div>
    <a href="#" class="body-button">Get a Free Quote</a>
    <div class="additional-items">
      <div class="additional-item">
        <i class="additional-icon">✨</i>
        <span class="additional-text">Magical Results</span>
      </div>
      <div class="additional-item">
        <i class="additional-icon">🔮</i>
        <span class="additional-text">Enchanting Service</span>
      </div>
      <div class="additional-item">
        <i class="additional-icon">🌟</i>
        <span class="additional-text">Stellar Quality</span>
      </div>
    </div>
  </section>
<footer>
  <div class="footer-container">
    <div class="footer-info">
      <h3>Contact Us</h3>
      <p>123 Street, City, Country</p>
      <p>Phone: +1 234 567890</p>
      <p>Email: info@yourbusiness.com</p>
    </div>
    <div class="footer-links">
      <h3>Quick Links</h3>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>
    <div class="footer-social">
      <h3>Follow Us</h3>
      <ul>
        <li><a href="#"><img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook"></a></li>
        <li><a href="#"><img src="https://img.icons8.com/office/30/FF0000/twitter.png" alt="Twitter"></a></li>
        <li><a href="#"><img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram"></a></li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <p>&copy; 2023 Your Business. All rights reserved.</p>
  </div>
</footer>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/110/three.min.js"></script>
  <script>let leftMenuButton = document.querySelector('.menu-button.left');
    let rightMenuButton = document.querySelector('.menu-button.right');
    let leftSideMenu = document.querySelector('.left-side-menu');
    let rightSideMenu = document.querySelector('.right-side-menu');
function openSideMenu(side) {
      if (side === 'left') {
        leftSideMenu.style.width = '250px';
     } else if (side === 'right') {
        rightSideMenu.style.width = '250px';
      }
    }
function closeSideMenu(side) {
      if (side === 'left') {
        leftSideMenu.style.width = '0';
      } else if (side === 'right') {
        rightSideMenu.style.width = '0';
      }
    }
function updateClock() {
      var now = new Date();
      var hours = now.getHours();
      var minutes = now.getMinutes();
      var day = now.getDate();
      var month = now.getMonth() + 1;
      var year = now.getFullYear();
      hours = hours < 10 ? "0" + hours : hours;
      minutes = minutes < 10 ? "0" + minutes : minutes;
      day = day < 10 ? "0" + day : day;
      month = month < 10 ? "0" + month : month;
      var time = hours + ":" + minutes;
      var date = day + "/" + month + "/" + year;
      document.getElementById("clock").innerHTML = time;
      document.getElementById("date").innerHTML = date;
      setTimeout(updateClock, 1000);
    }
    function countdownToLaunch() {
      var launchDate = new Date("2023-06-30T00:00:00"); 
      setInterval(function() {
        var now = new Date();
        var diff = launchDate - now;
        var hours = Math.floor(diff / (1000 * 60 * 60));
        var minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((diff % (1000 * 60)) / 1000);
        hours = hours < 10 ? "0" + hours : hours;
        minutes = minutes < 10 ? "0" + minutes : minutes;
        seconds = seconds < 10 ? "0" + seconds : seconds;
        document.getElementById("launch").innerHTML = "Next Launch in " + hours + ":" + minutes + ":" + seconds;
      }, 1000);
    }
    window.onload = function() {
      updateClock();
      countdownToLaunch();
    };
    var subheading = document.querySelector('.subheading');
    var texts = [
      "Bringing window cleaning online #lofties",
      "Did you really think you'd have to click each letter here too?",
      "Guess what? There's more clicking in store for you!",
      "Just kidding! Enjoy the hunt for the squeegee and win a chance for a free clean!"
    ];
    var index = 0;
    function changeText() {
      index = (index + 1) % texts.length;
      subheading.textContent = texts[index];
    }
    subheading.addEventListener('click', changeText);
    var heading = document.querySelector('.heading');
    var letters = heading.textContent.split('');
    heading.textContent = '';
    letters.forEach(function(letter) {
      var span = document.createElement('span');
      span.textContent = letter;
      span.className = 'letter';
      heading.appendChild(span);
    });
    function getRandomNumber(min, max) {
      return Math.random() * (max - min) + min;
    }
    function animateLetter(letter) {
      letter.classList.add('active');
      var rotation = getRandomNumber(-360, 360);
      var xTranslation = getRandomNumber(-100, 100);
      var yTranslation = getRandomNumber(-100, 100);
      var scale = getRandomNumber(0.8, 1.2);
      letter.style.transform = `rotate(${rotation}deg) translate(${xTranslation}px, ${yTranslation}px) scale(${scale})`;
      setTimeout(function() {
        letter.classList.remove('active');
        letter.style.transform = '';
      }, 1000);
    }
    var spans = document.querySelectorAll('.letter');
    spans.forEach(function(span) {
      span.addEventListener('click', function() {
        animateLetter(span);
      });
    });
    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
    const renderer = new THREE.WebGLRenderer({ alpha: true });
    renderer.setSize(100, 100);
    document.getElementById('planet').appendChild(renderer.domElement);
    const planetGeometry = new THREE.SphereGeometry(4, 64, 64);
    const planetMaterial = new THREE.MeshStandardMaterial({
      color: 0x00b3b3,
      metalness: 0.2,
      roughness: 0.5
    });
    const planetMesh = new THREE.Mesh(planetGeometry, planetMaterial);
    const textureLoader = new THREE.TextureLoader();
    textureLoader.load('planet_texture.jpg', (texture) => {
      planetMaterial.map = texture;
      planetMaterial.needsUpdate = true;
    });
    scene.add(planetMesh);
    const light = new THREE.PointLight(0xffffff, 1);
    light.position.set(-10, 10, 10);
    scene.add(light);
    camera.position.z = 15;
    document.addEventListener('click', () => {
      planetMesh.position.x -= 1;
    });
    function animate() {
      requestAnimationFrame(animate);
      renderer.render(scene, camera);
    }
    animate();
  </script>
</body>

</html>

<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Exo:100,200,400,italic">

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    
    body {
      font-family: 'Exo', sans-serif;
      background: #3399cc;
      color: #CCC;
      overflow-x: hidden;
    }
    
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
      background-size: cover;
      padding: 40px;
      text-align: center;
      color: #FFF;
      margin: 0;
    }
    
    #clock {
      font-size: 9px;
      position: absolute;
      top: 2px;
      left: 2px;
    }
    
    #date {
      font-size: 9px;
      position: absolute;
      top: 14px;
      left: 2px;
    }
    
    #launch {
      color: #00b3b3;
      text-shadow: 1px 1px 2px #00b3b3;
      border: 1px solid #00b3b3;
      border-radius: 8px;
      padding: 1px;
      font-size: 9px;
      position: absolute;
      top: 28px;
      left: 2px;
    }
    
    #countdown-text {
      font-size: 10px;
      position: absolute;
      top: 55px;
      left: 35px;
      opacity: 0; 
      transition: opacity 0.3s ease-in-out;
    }
    
    #countdown:hover #countdown-text {
      opacity: 1; 
    }
    
    #space-x-logo {
      color: #00b3b3;
      text-shadow: 1px 1px 2px #00b3b3;
      border: 1px solid #00b3b3;
      border-radius: 8px;
      padding: 1px;
      max-width: 40px;
      position: absolute;
      top: 45px;
      left: 10px;
    }
    
    .login-register {
      background-color: white;
      padding: 2px;
      font-size: 10px;
      position: absolute;
      top: 10px;
      right: 8px;
      border-radius: 2px;
      box-shadow: 0px 0px 5px #00b3b3;
    }
    
    .login-register a {
      color: #1abc9c;
      text-decoration: none;
      margin-left: 1px;
    }
    
    .login-register a:hover {
      color: #2ecc71;
    }
    
    .letter {
      display: inline-block;
      cursor: pointer;
      transition: transform 0.5s;
    }
    
    .letter.active {
      animation-name: neon-glow;
      animation-duration: 2s;
      animation-iteration-count: infinite;
      animation-fill-mode: forwards;
    }
    
    .heading {
      text-align: center;
      font-size: 14px;
      -webkit-text-stroke: 0.7px white;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #00b3b3, #00b3b3, #00b3b3);
      -webkit-background-clip: text;
      padding: 5px;
      transition: all 0.5s ease;
      margin-bottom: -20px;
      font-weight: bold;
      letter-spacing: 1px;
      line-height: 1;
      animation: neon-glow 2s ease-in-out infinite alternate;
    }
    
    .heading:hover {
      transform: scale(1.1);
      text-shadow: 0px 5px 10px rgba(0, 0, 0, 0.5), 0px 0px 20px #00b3b3;
    }
    
    .subheading {
      text-align: center;
      font-size: 20px;
      -webkit-text-stroke: 0.2px #000;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #FF0066, #FF00FF, #6600FF, #00CCFF, #00FF66, #FFFF00, #FF0066);
      -webkit-background-clip: text;
      padding: 10px;
      transition: all 0.5s ease;
      margin-top: 20px;
      font-weight: normal;
      letter-spacing: 1px;
      cursor: pointer;
      line-height: 1.2;
      text-shadow: 0px 0px 20px rgba(255, 255, 255, 0.8), 0px 0px 40px rgba(255, 255, 255, 0.8);
    }
    
    .subheading:hover {
      transform: scale(1.1);
      text-shadow: 0px 5px 10px rgba(0, 0, 0, 0.5), 0px 0px 30px #00b3b3, 0px 0px 50px rgba(255, 255, 255, 0.8);
    }
    
    .social {
      list-style: none;
      position: absolute;
      padding: 1px;
      bottom: 2px;
      left: 5px;
    }
    
    .social li {
      display: flex;
      align-items: center;
      margin-bottom: 5px; 
    }
    
    .social li a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: black;
      transition: transform 0.3s ease-in-out;
      position: relative;
    }
    
    .social li a:hover {
      transform: scale(1.7);
    }
    
    .social li a img {
      display: inline-block;
      vertical-align: middle;
      transition: transform 0.3s ease-in-out;
      background: transparent;
      width: 18px;
      height: 18px;
      margin-right: 4px;
      filter: brightness(1);
    }
    
    .text-box {
      position: absolute;
      text-align: center;
      font-size: 8px;top: -10px;
      left: 7px;
      -webkit-text-stroke: 0.2px #000;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #FF0066, #FF00FF, #6600FF, #00CCFF, #00FF66, #FFFF00, #FF0066);
      -webkit-background-clip: text;
      padding: 2px;
      transition: all 0.5s ease;
      white-space: nowrap;
      display: none; 
    }
    
    .social li a:hover .text-box {
      text-align: center;
      font-size: 8px;
      position: absolute;
      top: -10px;
      left: 7px;
      -webkit-text-stroke: 0.2px #000;
      -webkit-text-fill-color: transparent;
      background-image: linear-gradient(to right, #FF0066, #FF00FF, #6600FF, #00CCFF, #00FF66, #FFFF00, #FF0066);
      -webkit-background-clip: text;
      padding: 10px;
      transition: all 0.5s ease;
      display: block; 
      opacity: 1;
    }

    .competition {
      position: absolute;
      bottom: 2px;
      right: 2px;
      padding: 5px;
      border-radius: 5px;
      color: #00b3b3;
      cursor: pointer;
      font-size: 13px;
      font-weight: bold;
      font-style: italic;
      font-family: 'Exo 2', sans-serif;
      transition: background-color 0.9s, transform 0.9s;
    }
    
    .competition:hover {
      background-color: #FFF;
      transform: scale(1);
      transition: background-color 0.9s, transform 0.9s;
    }
    
    .competition:hover .competition-text {
      display: block;
      animation: pulse 7.5s infinite;
    }
    
    .competition-text {
      display: none;
      background-color: #FFF;
      font-size: 9px;
      border-radius: 5px;
      transition: background-color 0.9s, transform 0.9s;
    }

    @keyframes pulse {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.1);
      }
      100% {
        transform: scale(1);
      }
    }

   section {
    padding: 40px 0;
    text-align: center;
    color: #FFF;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }

  .section-container {
    max-width: 800px;
    margin: 0 auto;
  }

  h2 {
    font-size: 9px;
    margin-bottom: 20px;
  }

  p {
    font-size: 9px;
    margin-bottom: 10px;
  }

  .competition-info {
    margin-top: 30px;
  }

  h3 {
    font-size: 9px;
    margin-bottom: 10px;
  }

  .btn {
    display: inline-block;
    background-color: #00b3b3;
    color: #FFF;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s;
  }

  .btn:hover {
    background-color: #00a3a3;
  }

  
  footer {
    background-color: #222;
    padding: 30px 0;
    color: #FFF;
    text-align: center;
  }

  .footer-container {
    max-width: 800px;
    margin: 0 auto;
  }

  .footer-info,
  .footer-links,
  .footer-social {
    width: 33.33%;
    display: inline-block;
    text-align: center;
  }

  .footer-info h3,
  .footer-links h3,
  .footer-social h3 {
    font-size: 9px;
    margin-bottom: 10px;
  }

  .footer-links ul {
    list-style: none;
    padding-left: 0;
  }

  .footer-links li {
    margin-bottom: 5px;
  }

  .footer-links a {
    color: #CCC;
    text-decoration: none;
  }

  .footer-links a:hover {
    color: #FFF;
  }

  .footer-social ul {
    list-style: none;
    padding-left: 0;
  }

  .footer-social li {
    display: inline-block;
    margin-right: 10px;
  }

  .footer-social img {
    width: 30px;
    height: 30px;
  }

  .footer-bottom {
    background-color: #111;
    padding: 10px 0;
    text-align: center;
  }

  .footer-bottom p {
    margin: 0;
    font-size: 9px;
  }
  </style>
</head>
<body>
  <header>
    <div id="countdown">
      <!-- Countdown Section -->
      <div id="clock"></div>
      <div id="date"></div>
      <div id="launch"></div>
      <div id="countdown-text">Space-X Countdown to Next Take-Off<br>Mars Soon</div>
    </div>
<!-- Social Media Links -->
    <div class="social">
      <ul> 
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
            <div class="text-box">
              <p>Check out our YouTube channel for clues on the squeegee hunt!</p>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/discord-logo.png" alt="Discord">
            <div class="text-box">
              <p>Join our Discord server and collaborate to uncover the squeegee!</p>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
            <div class="text-box">
              <p>Follow our Facebook page to find the elusive squeegee adventure!</p>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram">
            <div class="text-box">
              <p>Explore our Instagram feed for hints leading to the squeegee treasure!</p>
            </div>
          </a>
        </li>
      </ul>
    </div>
<!-- SpaceX Logo -->
    <img id="space-x-logo" src="https://upload.wikimedia.org/wikipedia/commons/d/de/SpaceX-Logo.svg" alt="SpaceX Logo">
<!-- Login/Register Links -->
    <div class="login-register">
      <a href="#">Login</a>
      <a href="#">Register</a>
    </div>
<!-- Headings -->
    <h1 class="heading">LoftieswindowS</h1>
    <div class="subheading">Bringing Window Cleaning Online #Lofties</div>
    <div id="planet"></div><div class="competition">
      <span>🌟Free Window Clean🌟</span>
      <div class="competition-text">Unleash your inner adventurer,<br> hunt the elusive squeegee on our webpage ,<br> and unlock a FREE window clean! Are you ready?<br> Let the pursuit begin!</div>
    </div>
  </header>
  <section>
  <div class="section-container">
    <h2>About Our Business</h2>
    <p>Quality service. Customer satisfaction guaranteed.</p>
    <p>Experienced professionals. Affordable pricing options.</p>
  </div>
</section>
<section>
  <div class="section-container">
    <h2>Competition</h2>
    <p>Join our exciting contest now!</p>
    <p>Win amazing prizes and recognition.</p>
    <div class="competition-info">
      <h3>Learn More</h3>
      <p>Participate and showcase your talents!</p>
      <a href="#" class="btn">Click Here</a>
    </div>
  </div>
</section>
<footer>
  <div class="footer-container">
    <div class="footer-info">
      <h3>Contact Us</h3>
      <p>123 Street, City, Country</p>
      <p>Phone: +1 234 567890</p>
      <p>Email: info@yourbusiness.com</p>
    </div>
    <div class="footer-links">
      <h3>Quick Links</h3>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>
    <div class="footer-social">
      <h3>Follow Us</h3>
      <ul>
        <li><a href="#"><img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook"></a></li>
        <li><a href="#"><img src="https://img.icons8.com/office/30/FF0000/twitter.png" alt="Twitter"></a></li>
        <li><a href="#"><img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram"></a></li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <p>&copy; 2023 Your Business. All rights reserved.</p>
  </div>
</footer>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/110/three.min.js"></script>
  <script>
    function updateClock() {
      var now = new Date();
      var hours = now.getHours();
      var minutes = now.getMinutes();
      var day = now.getDate();
      var month = now.getMonth() + 1;
      var year = now.getFullYear();
      hours = hours < 10 ? "0" + hours : hours;
      minutes = minutes < 10 ? "0" + minutes : minutes;
      day = day < 10 ? "0" + day : day;
      month = month < 10 ? "0" + month : month;
      var time = hours + ":" + minutes;
      var date = day + "/" + month + "/" + year;
      document.getElementById("clock").innerHTML = time;
      document.getElementById("date").innerHTML = date;
      setTimeout(updateClock, 1000);
    }
    function countdownToLaunch() {
      var launchDate = new Date("2023-06-30T00:00:00"); 
      setInterval(function() {
        var now = new Date();
        var diff = launchDate - now;
        var hours = Math.floor(diff / (1000 * 60 * 60));
        var minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((diff % (1000 * 60)) / 1000);
        hours = hours < 10 ? "0" + hours : hours;
        minutes = minutes < 10 ? "0" + minutes : minutes;
        seconds = seconds < 10 ? "0" + seconds : seconds;
        document.getElementById("launch").innerHTML = "Next Launch in " + hours + ":" + minutes + ":" + seconds;
      }, 1000);
    }
    window.onload = function() {
      updateClock();
      countdownToLaunch();
    };
    var subheading = document.querySelector('.subheading');
    var texts = [
      "Bringing window cleaning online #lofties",
      "Did you really think you'd have to click each letter here too?",
      "Guess what? There's more clicking in store for you!",
      "Just kidding! Enjoy the hunt for the squeegee and win a chance for a free clean!"
    ];
    var index = 0;
    function changeText() {
      index = (index + 1) % texts.length;
      subheading.textContent = texts[index];
    }
    subheading.addEventListener('click', changeText);
    var heading = document.querySelector('.heading');
    var letters = heading.textContent.split('');
    heading.textContent = '';
    letters.forEach(function(letter) {
      var span = document.createElement('span');
      span.textContent = letter;
      span.className = 'letter';
      heading.appendChild(span);
    });
    function getRandomNumber(min, max) {
      return Math.random() * (max - min) + min;
    }
    function animateLetter(letter) {
      letter.classList.add('active');
      var rotation = getRandomNumber(-360, 360);
      var xTranslation = getRandomNumber(-100, 100);
      var yTranslation = getRandomNumber(-100, 100);
      var scale = getRandomNumber(0.8, 1.2);
      letter.style.transform = `rotate(${rotation}deg) translate(${xTranslation}px, ${yTranslation}px) scale(${scale})`;
      setTimeout(function() {
        letter.classList.remove('active');
        letter.style.transform = '';
      }, 1000);
    }
    var spans = document.querySelectorAll('.letter');
    spans.forEach(function(span) {
      span.addEventListener('click', function() {
        animateLetter(span);
      });
    });
    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
    const renderer = new THREE.WebGLRenderer({ alpha: true });
    renderer.setSize(100, 100);
    document.getElementById('planet').appendChild(renderer.domElement);
    const planetGeometry = new THREE.SphereGeometry(4, 64, 64);
    const planetMaterial = new THREE.MeshStandardMaterial({
      color: 0x00b3b3,
      metalness: 0.2,
      roughness: 0.5
    });
    const planetMesh = new THREE.Mesh(planetGeometry, planetMaterial);
    const textureLoader = new THREE.TextureLoader();
    textureLoader.load('planet_texture.jpg', (texture) => {
      planetMaterial.map = texture;
      planetMaterial.needsUpdate = true;
    });
    scene.add(planetMesh);
    const light = new THREE.PointLight(0xffffff, 1);
    light.position.set(-10, 10, 10);
    scene.add(light);
    camera.position.z = 15;
    document.addEventListener('click', () => {
      planetMesh.position.x -= 1;
    });
    function animate() {
      requestAnimationFrame(animate);
      renderer.render(scene, camera);
    }
    animate();
  </script>
</body>

</html>
