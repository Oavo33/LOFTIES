<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Lofties Windows</title>
	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
	<style>
		header {
			font-family: "UnifrakturMaguntia";
			background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
			background-size: cover;
			padding: 50px;
		}
    .triangle-container {
			position: relative;
			width: 100%;
			height: 100px;
			margin-bottom: 20px;
		}
		.canvas {
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
		}
		.tab-menu {
			list-style: none;
			margin: 0;
			padding: 0;position: absolute;
			bottom: 300px;
			left: 50px;
			display: flex;
		}
		.tab-menu li {
			margin-right: 10px;width: 10px;
			height: 10px;
			background-color: #fff;
			border-radius: 50%;
			display: flex;align-items: center;
			justify-content: center;
			font-size: 0;
			flex-shrink: 0;
			cursor: pointer;
		}
		.tab-menu li.active {
			background-color: #000;
		}
		.tab-menu li:hover .tab-hover {
			display: block;
		}
		.tab-menu li .tab-hover {
			display: none;
			position: absolute;
			top: 10%;
			left: 0;
			background-color: #000;
			color: #fff;
			padding: 5px;
			font-size: 14px;
			line-height: 1.5;
			z-index: 1;
			max-width: 200px;
			border-radius: 5px;
			opacity: 0.8;
		}
		.social-icons {
			list-style: none;
			margin: 0;
			padding: 0;
			position: absolute;
			top: 10px;
			right: 10px;
			display: flex;
			flex-direction: column;
			align-items: flex-end;
		}
		.social-icons li {
			margin-bottom: 10px;
		}
		.social-icons li:last-child {
			margin-bottom: 0;
		}
		.social-icons li a {
			display: block;
			width: 15px;
			height: 15px;
			background-size: cover;
		}
		.social-icons li a.facebook {
			background-image: url("https://img.icons8.com/clouds/32/000000/facebook.png");
		}
		.social-icons li a.discord {
			background-image: url("https://img.icons8.com/clouds/32/000000/discord-logo.png");
		}
		.social-icons li a.youtube {
			background-image: url("https://img.icons8.com/clouds/64/000000/youtube.png");
		}
	</style>
</script></head>
<body>
	<header>
		<div class="triangle-container">
			<canvas id="canvas"></canvas>
		</div>
		<h1><span>L</span><span>o</span><span>f</span><span>t</span><span>i</span><span>e</span><span>s</span><span>W</span><span>i</span><span>n</span><span>d</span><span>o</span><span>w</span><span>S</span></h1>
		<nav>
			<ul>
				<li><a href="#"><img src="https://img.icons8.com/clouds/32/000000/facebook.png" alt="Facebook"></a></li>
				<li><a href="#"><img src="https://img.icons8.com/clouds/32/000000/discord-logo.png" alt="Discord"></a></li>
				<li><a href="#"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></a></li>
			</ul>
		</nav>
	<ul class="tab-menu">
		<li>
			<img src="https://img.icons8.com/color/48/000000/controller.png" alt="Games">
			Games
			<div class="tab-hover">Why did the sun go to school? To get brighter!</div>
		</li>
		<li>
			<img src="https://img.icons8.com/color/48/000000/youtube-play.png" alt="Videos">
			Videos
			<div class="tab-hover">Why did the astronaut break up with his girlfriend? Because he needed his space!</div>
        </li>
        <li>
          <img src="https://img.icons8.com/color/48/000000/music.png" alt="Music">
          Music
          <div class="tab-hover">Why did the space cookie go to the doctor? Because it felt crummy!</div>
        </li>
    </ul><p id="typewriter-text"></p>
</header>
	<script>@media only screen and (max-width: 600px) {
		const text = "Attention all window lovers! Search our website for the squeegee and win a free clean!";
		let i = 0;
		function typeWriter() {
			if (i < text.length) {
				document.getElementById("typewriter-text").innerHTML += text.charAt(i);
				i++;
				setTimeout(typeWriter, Math.floor(Math.random() * 200) + 50); // randomize the typing speed
			}
		}
		typeWriter();}
	</script>
</body></html>