<html>
<head>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=750&q=80");
      background-size: cover;
      background-position: center;
      padding: 80px; /* Adjust the padding value as needed */
    }
    #wigz {
      height: 30%;
      display: inline-block;
      align-items: center;
      justify-content: center;
      position: absolute;
      top: 23%;
      left: 39%;
      transform: translate(-50%, -50%);
    }
    #wigz .heading {
      font-family: 'UnifrakturMaguntia', cursive;
      font-size: 17px;
      text-align: center;
      position: relative;
      text-shadow: #00b3b3;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
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
    }@keyframes move {
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
  right: 5px;
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
  top: 18px;
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
<header>
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