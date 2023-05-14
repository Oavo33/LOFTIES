<html><head>
  <style>
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=750&q=80");
      background-size: cover;
      background-position: center;
      padding: 60px;
    }.clock {
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
    }.container {
  position: absolute;
  top: 14px;
  left: 14px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.nav-item {
  background-color: #30b3b3;
  width: 30px; /* Adjusted width to fit mobile screens */
  height: 30px; /* Decreased height for mobile devices */
  color: white;
  text-align: center;
  font-size: 8px; /* Increased font size for mobile devices */
  font-family: Arial, sans-serif;
  cursor: pointer;
  transition: transform 0.5s, background-color 0.5s;
  overflow: hidden;
  border: 1px solid #800000;
  border-radius: 2px;box-sizing: border-box;
  margin-bottom: 2px;
}
.nav-item:nth-child(1) {
  top: 1px;
}
.nav-item:nth-child(2) {
  bottom: 1px;
}
.nav-item:hover:before {
  border-bottom: 2px solid #00b3b3; /* Adjusted border size for mobile devices */
  opacity: 1;
  transform: translate(-50%, -50%) rotate(45deg) scale(1.2);
}
.nav-item.clicked {
      transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
    }.nav-item:after {
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
    }.nav-item span.number {
      z-index: 3;
      color: black;
    }.nav-item .text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.nav-item i {
  font-size: 5px; /* Increased font size for mobile devices */
  position: relative;
  top: auto;
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
      width: 200px;
      padding: 20px;
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
      <h2>Planet Information</h2>
      <p>This is a fascinating planet with diverse ecosystems and rich history. Explore more to uncover its wonders!</p>
    </div>
  </div>
</header>
<body>
<script>function getRandomColor() {
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
