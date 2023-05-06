<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lofties Windows</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: sans-serif;
    }.logo-container {
      display: inline-block;
      border: 1px solid #ff6600;
      border-radius: 10px;
      padding: 10px;
      margin: 20px;
      font-size: 3em;
      font-family: 'UnifrakturMaguntia', cursive;
      font-style: italic;
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
      font: bold 1.2rem sans-serif;
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
 ul {
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
        display: inline-block;
        margin-right: 8px;
        font-size: 24px;
      }.video-icon {
        color: red;
      }.game-icon {
        color: green;
      }.music-icon {
        color: blue;
      }
}@media screen and (max-width: 768px) {
      h1 {
        font-size: 1.5rem;
        padding: 10px;
      }
      ul.social li {
        margin: 0 5px;
      }
      button {
        margin-top: 30px;
        font-size: 1;
   }
    }</style>
    </head> 
    <body><header>
      <ul>
        <li><a href="#home"><span class="icon video-icon">&#x1F3A5;</span> Videos</a></li>
        <li><a href="#about"><span class="icon game-icon">&#x1F3AE;</span> Games</a></li>
        <li><a href="#contact"><span class="icon music-icon">&#x1F3B5;</span> Music</a></li>
      </ul>
    </header>
  <div class="logo-container">
    <span class="move">L</span>ofties<span class="move">W</span>indo<span class="move">w</span>s
  </div>
  <button>Click me!</button>
  <div class="ball"></div>
  <ul class="social">
    <li><a href="#"><i class="icon1"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></i></a></li>
    <li><a href="#"><i class="icon4"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></i></a></li>
    <li><a href="#"><i class="icon3"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></i></a></li>
    <li><a href="#"><i class="icon4"><img src="https://img.icons8.com/clouds/64/000000/tiktok.png" alt="TikTok"></i></a></li>
  </ul>
</body>
</html>


