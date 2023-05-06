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

