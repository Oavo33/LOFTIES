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
			box-sizing: border-box;
			margin: 0;
			padding: 0;
		}body {
			font-family: 'Montserrat', sans-serif;
			font-size: 16px;
			color: #333;
		}header {
			background-size: 100%;
			padding: 80px;
			display: flex;
      background-position: center 65%;
			justify-content: space-between;
			align-items: center;
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
			position: relative;
		}h1 {
			font-size: 32px;
			font-weight: 700;
		}.social {
			display: flex;
			align-items: center;
			position: absolute;
			top: 5px;
			left: 5px;
		}.social li {
			list-style: none;
			margin-right: 3px;
		}.social li:last-child {
			margin-right: 3px;
		}.social img {
			height: 21px;
			margin-right: 3px;
			filter: brightness(50%);
			transition: filter 0.9s ease-in-out;
		}.social img:hover {
			filter: brightness(100%);
		}.bottom-right {
        position: absolute;
        bottom: 1px;
        right: 1px;
        display: flex;
        gap: 2px;
      }.bottom-right jake {
        list-style: none;
      }.icon {
        font-size: 10px;
      }@media only screen and (max-width: 600px) {
        header {
          padding: 60px;
        }
      }
	</style>
</head>
<body>
	<header>
		<h1>Lofties Windows</h1>
		<ul class="social">
			<li><a href="https://www.facebook.com"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></a></li>
			<li><a href="https://www.discord.com"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></a></li>
			<li><a href="https://www.youtube.com"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></a></li>
		</ul>
      <ul class="bottom-right">
        <jake>
          <a href="#contact" class="video-tab">
            <span class="icon video-icon">&#x1F3A5;</span>
            Videos
          </a>
        </jake>
        <jake>
          <a href="#contact" class="music-tab">
            <span class="icon music-icon">&#x1F3B5;</span>
            Music
          </a>
        </jake>
        <jake>
          <a href="#contact" class="game-tab">
            <span class="icon game-icon">&#x1F3AE;</span>
            Games
          </a>
        </jake>
      </ul>
	</header></body>
</html>


