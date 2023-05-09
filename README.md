<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lofties Windows</title>
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing:border-box;
      margin:0;
      padding:0;
    }
    body {
      font-family:'Montserrat',sans-serif;
      font-size:16px;
      color:#333;
    }
    header {
      background-size:100%;
      padding:80px;
      display:flex;
      background-position:center 65%;
      justify-content:space-between;
      align-items:center;
      background-image:url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
      position:relative;
    }
    h1 {
      font-size:32px;
      font-weight:700;
    }
    .social-icons-container {
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
    }.bottom-right jake {
      list-style:none;
    }.icon {
      font-size:10px;
    }@media only screen and (max-width: 600px) {
  .social-icons-container {
    top: 10px;
    left: 10px;
    background: none;
  }
}
  </style>
</head>
<body>
  <header>
    <div class="social-icons-container">
      <a href="https://www.facebook.com"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></a>
      <a href="https://www.discord.com"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></a>
      <a href="https://www.youtube.com"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></a>
    </div>
    <h1>Lofties Windows</h1><ul class="bottom-right">
      <jake><a href="#contact" class="video-tab"><span class="icon video-icon">&#x1F3A5;</span>Videos</a></jake>
      <jake><a href="#contact" class="music-tab"><span class="icon music-icon">&#x1F3B5;</span>Music</a></jake>
      <jake><a href="#contact" class="game-tab"><span class="icon game-icon">&#x1F3AE;</span>Games</a></jake>
    </ul>
  </header>
</body>
</html>


