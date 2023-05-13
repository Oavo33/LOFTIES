<head><style>
    header {
      position: relative;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=750&q=80");
      background-size: cover;
      background-position: center;
      padding: 100px;
    }.clock {
      position: absolute;
      top: 20px;
      left: 20px;
      font-size: 8px;
      cursor: pointer;
      color: white;
    }.timer {
      position: absolute;
      top: 20px;
      left: 61px;
      font-size: 8px;
      color: white;
    }.button-container {
      position: absolute;
      top: 21px;
      left: 20px;
      }.button {
      display: inline-block;
      padding: 1px 1px;
      font-size: 5px;
      cursor: pointer;
      background-color: #00b3b3;
      color: #ffffff;
      border: none;
      border-radius: 1px;
      margin-right: 1px;
      margin-bottom: 1px;
    }.button:hover {
      background-color: #00b3b3;
      animation: pulse 1s infinite;}@keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }@media only screen and (max-width: 600px) {
      }
  </style></head>
<header>
  <div id="clock" class="clock">00:00</div><div id="timer" class="timer">00:00:00</div>
  <div class="button-container">
    <button id="format-toggle" class="button">Toggle Format</button><button id="timer-start" class="button">Start</button>
    <button id="timer-reset" class="button">Reset</button>
  </div>
</header>
<script>
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
      buttons[i].addEventListener("mouseover", function () {
        this.style.backgroundColor = getRandomColor();
      });
      buttons[i].addEventListener("mouseout", function () {
        this.style.backgroundColor = "#800000";
      });
    }
var clock = document.getElementById("clock");
    var timer = document.getElementById("timer");
    var formatToggle = document.getElementById("format-toggle");
    var timerStart = document.getElementById("timer-start");
    var timerReset = document.getElementById("timer-reset");
formatToggle.addEventListener("click", function () {
      clock.classList.toggle("timer");
      timer.classList.toggle("clock");
    });
timerStart.addEventListener("click", function () {
    });
timerReset.addEventListener("click", function () {
    });
function updateClock() {
      const clockElement = document.getElementById("clock");
      const date = new Date();
      let hours = date.getHours();
      let minutes = date.getMinutes();
      let ampm='';
if(is24HourFormat()){
    hours=padZero(hours);
  }else{
    hours=convertTo12Hour(hours);
    ampm=hours>=12?'PM':'AM';
  }
minutes=padZero(minutes);
  const time=`${hours}:${minutes} ${ampm}`;
  clockElement.textContent=time;
}function is24HourFormat(){
  return localStorage.getItem('format')==='24';
}
function toggleFormat(){
  const formatToggle=document.getElementById('format-toggle');
  formatToggle.addEventListener('click',function(){
    const currentFormat=localStorage.getItem('format');
    const newFormat=currentFormat==='24'?'12':'24';
    localStorage.setItem('format',newFormat);
    updateClock();
  });
}
function padZero(value){
  return value.toString().padStart(2,'0');
}
function convertTo12Hour(hours){
  return hours>12?hours-12:hours;
}
let timerInterval;
let timerSeconds=0;
function startTimer(){
  const timerElement=document.getElementById('timer');
  const timerStartButton=document.getElementById('timer-start');
  const timerResetButton=document.getElementById('timer-reset');
timerStartButton.addEventListener('click',function(){
    if(timerInterval){
      clearInterval(timerInterval);
      timerInterval=null;
      timerStartButton.textContent='Start';
    }else{
      timerInterval=setInterval(function(){
        timerSeconds++;
        const hours=Math.floor(timerSeconds/3600);
        const minutes=Math.floor((timerSeconds%3600)/60);
        const seconds=timerSeconds%60;
        const time=`${padZero(hours)}:${padZero(minutes)}:${padZero(seconds)}`;
        timerElement.textContent=time;
      },1000);
      timerStartButton.textContent='Pause';
    }
  });
timerResetButton.addEventListener('click',function(){
    clearInterval(timerInterval);
    timerInterval=null;
    timerSeconds=0;
    timerElement.textContent='00:00:00';
    timerStartButton.textContent='Start';
  });
}
function initializeClock(){
  localStorage.removeItem('format');
  updateClock();
  toggleFormat();
  startTimer();
}
initializeClock();
</script>
</body>
</html>


