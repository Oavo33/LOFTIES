<!DOCTYPE html>
<html lang="en">
  <head>
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XMY3P6EP78"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XMY3P6EP78');
</script>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lofties Windows</title>
    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <style>
      body {
        color: #00b3b3;
        background-color: #800000;
        margin: 0;
        font-family: "Pacifico", cursive;
      }
      header {
        background-color: #800000;
        background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
        background-size: cover;
        background-position: center;
        color: #00b3b3;
        padding: 110px;
        position: relative;
        text-align: center;
        text-shadow: 2px 2px #800000;
      }
      #planet-system {
  position: absolute;
  top: 25%;
  right: 20%;
  transform: scale(0.4) translate(-50%, -50%);
  transform-origin: center center;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}.logo {
  position: absolute;
  bottom: 0;
  left: 0;
  margin: 0;
  display: flex;
  align-items: center;
}.logo a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: #00b3b3;
}.logo::after {
  content: "";
  position: absolute;
  bottom: 0px;
  left: -5px;
  height: 35px;
  width: 0;
  border-bottom: 70px solid transparent;
  border-right: 70px solid transparent;
  opacity: 0.8;
  transition: all 5s ease-in-out;
}.logo:hover::after {
  content: "Its.The.Window Cleaner";
  position: absolute;
  bottom: 0px;
  left: -5px;
  height: 35px;
  width: 0;
  border-bottom: 70px solid #00b3b3;
  border-right: 70px solid transparent;
  opacity: 1;
  transition: all 3s ease-in-out;
  filter: hue-rotate(270deg) drop-shadow(2px 2px 2px #00b3b3)
          invert(19%) sepia(57%) saturate(6287%) hue-rotate(346deg)
          brightness(102%) contrast(102%);
}.logo-text-container {
  transform: rotate(45deg);
  white-space: nowrap;
  position: relative;
  z-index: 1;
  top: -10px;
  left: -10px;
  transition: all 4s ease-in-out;
}.logo:hover .logo-text-container {
  transform: rotate(360deg);
  transition: all 4s ease-in-out;
}.logo-text {
  font-size: 14px;
  margin: 0 10px;
  text-shadow: 2px 2px #800000;
}.logo2-text {
  font-size: 7px;
  position: absolute;
  top: 0;
  left: 0%;
  margin: 0 10px;
  text-shadow: 2px 2px #800000;
  animation: moveText 50s ease-in-out infinite;
}
.flash {
  animation: flash 14s infinite;
}.header-text {
  position: absolute;
  top: 32%; 
  left: 32%;
  transform: translate(-50%, -50%);
  font-size: 44px;
}p {
  font-size: 14px;
}
.sun {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
background-color: #00B3B3;
border-radius: 50%;
width: 100px;
height: 100px;
}.planet {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
border-radius: 50%;
animation-timing-function: linear;
animation-iteration-count: infinite;
animation-name: flash14;
animation-duration: 1s;
}.mercury {
width: 5px;
height: 5px;
background-color: #00B3B3;
animation: orbit 5s linear infinite, flash14 254s infinite;
}.venus {
width: 10px;
height: 10px;
background-color: #800000;
animation: orbit 8s linear infinite, flash14 154s infinite;
}
.earth {
width: 12px;
height: 12px;
background-color: #00B3B3;
animation: orbit 10s linear infinite, flash14 54s infinite;
}
.mars {
width: 8px;
height: 8px;
background-color: #800000;
animation: orbit 12s linear infinite, flash14 47s infinite;
}
.jupiter {
width: 30px;
height: 30px;
background-color: #00B3B3;
animation: orbit 25s linear infinite, flash14 63s infinite;
}
.saturn {
width: 25px;
height: 25px;
background-color: #800000;
animation: orbit 35s linear infinite, flash14 85s infinite;
}
.uranus {
width: 20px;
height: 20px;
background-color: #00B3B3;
animation: orbit 45s linear infinite, flash14 78s infinite;
}
.neptune {
width: 18px;
height: 18px;
background-color: #800000;
animation: orbit 55s linear infinite, flash14 58s infinite;
}
@keyframes orbit {
from {
transform: rotate(0deg) translateX(80px) rotate(0deg);
}
to {
transform: rotate(360deg) translateX(80px) rotate(-360deg);
}
}
@keyframes flash14 {
0% {
background-color: #00B3B3;
}
50% {
background-color: #800000;
}
100% {
background-color: #00B3B3;
}
}@keyframes moveText {
  0% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(400px);
  }
  100% {
    transform: translateX(0);
  }
}@keyframes flash {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
    </style>
  </head>
  <body>
    <header>
      <div class="logo">
        <div class="logo-text-container">
          <div class="logo-text">Lofties</div>
        </div>
      </div>
      <div class="logo2">
        <div class="logo2-text-container">
          <div class="logo2-text">LoftiesWindows</div>
        </div>
        <div class="header-text">
          <div class="flash">LoftiesWindows</div>
          <p>See the world clearly, call us, we clean your windows!</p>
        </div>
      </div>
<div id="planet-system">
		<div class="sun"></div>
		<div class="planet mercury"></div>
		<div class="planet venus"></div>
		<div class="planet earth"></div>
		<div class="planet mars"></div>
		<div class="planet jupiter"></div>
		<div class="planet saturn"></div>
<div class="planet uranus"></div>
<div class="planet neptune"></div>
</div>
    </header>
    <main>
      <section>
        <p>...........</p>
      </section>
    </main>
  </body>
</html>

