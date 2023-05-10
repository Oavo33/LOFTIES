<html lang="en"><head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Lofties Windows</title>
	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
	<style>header {
			background-size: 100%;
			padding: 50px;
			display: flex;
			flex-direction: column;
			background-position: center 65%;
			font-family: "UnifrakturMaguntia";
			background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
			position: relative;
		}.triangle-container {
			display: flex;
			justify-content: center;
			align-items: flex-start;
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			overflow: hidden;
		}.triangle {
			width: 9vw;
			height: 10vw;
			background-color: #FF0000;
			transform: rotate(45deg);
			margin: 0.0vw;
		}nav {
			position: absolute;
			top: 20;
			left: -72;
			display: flex;
			align-items: center;
			padding: 0 80px;
			height: 50px;
			background-color: none;
		}nav ul {
			list-style: none;
			margin: 0;
			padding: 0;
			display: flex;
			flex-direction: column;
			align-items: center;
			height: 100%;
			justify-content: space-around;
		}nav li {
			margin-bottom: 1px;
			animation: zoomIn 2s ease forwards;
		}nav li:nth-child(1) img {
			filter: invert(100%) sepia(0%) saturate(1%) hue-rotate(280deg) brightness(104%) contrast(105%);
			transition: filter 2s ease;
		}nav li:nth-child(2) img {
			filter: invert(100%) sepia(0%) saturate(44%) hue-rotate(336deg) brightness(105%) contrast(98%);
			transition: filter 2s ease;
		}nav li:nth-child(3) img {
			filter: invert(100%) sepia(0%) saturate(12%) hue-rotate(110deg) brightness(105%) contrast(100%);
			transition: filter 2s ease;
		}nav img {
			height: 18px;
			transition: transform 0.5s ease;
		}nav li:hover img {
			transform: scale(2);
			filter: invert(0%) sepia(0%) saturate(100%) hue-rotate(0deg) brightness(100%) contrast(100%);
		}@keyframes zoomIn {
			from {
				transform: scale(0.1);
				opacity: 0;
			}
			to {
				transform: scale(1);
				opacity: 1;
			}
		}.tab-menu {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    height: 1%;
    position: absolute;
    bottom: 5;
    right: 2;
    margin: 0;
    padding: 0px;
  text-align: center;
    color: #800000;
}.tab-menu li {
    list-style: none;
    margin: 0 0px;
    position: relative;
    cursor: pointer;
    font-size: 10px;
    color: #00b3b3;
}.tab-menu li:hover .tab-hover {
    display: block;
}.tab-menu li .tab-hover {
    display: none;
    position: absolute;
    top: calc(100% + 10px);
    left: 50%;
    transform: translateX(-50%);
    background-color: #00b3b3;
    color: #800000;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 0 10px #800000;
    z-index: 1;
    text-align: center;
    font-size: 8px;
}.tab-menu li:nth-child(1) .tab-hover {
    width: 100px;
}.tab-menu li:nth-child(2) .tab-hover {
    width: 120px;
}.tab-menu li:nth-child(3) .tab-hover {
    width: 90px;
}.tab-menu li img {
    height: 14px;
    margin-right: 0px;
    vertical-align: middle;
}h1 {
			color: #00b3b3;
			font-size: 25px;
			transform: translateY(40px);
			animation: fade-in-out 20s infinite;
			text-shadow: 0 0 5px #800000, 0 0 10px #9c2222, 0 0 20px #b83f3f, 0 0 30px #d35c5c, 0 0 40px #ed7979, 0 0 50px #00b3b3;
			letter-spacing: 4px;
			 position: absolute;
  top: -30px;
  right: 200px;
		}h1 span {
			display: inline-block;
			position: relative;
			transition: transform 1s ease-out;
		}h1 span:hover {
			transform: translateX(20px);
		}#typewriter-text {
    font-size: 9px;
    text-align: center;
    font-family: Arial, sans-serif;
    color: #00b3b3;
    position: relative;
    display: left;
    border-radius: 5px;
    animation: typing 6s steps(30, end) forwards, blink-caret .5s step-end infinite;
    top: 58px;
    right: 68px;
}@keyframes typing {
			from {
				width: 0;
			}
			to {
				width: 100%;
			}
		}@keyframes blink-caret {
			from, to {
				border-color: transparent;
			}
			50% {
				border-color: #333;
			}
		}@keyframes fade-in-out {
			0% {
				opacity: 0;
			}
			50% {
				opacity: 1;
			}
			100% {
				opacity: 0;
			}
		}@media only screen and (max-width: 600px) {
        header {
          padding: 50px;
        }
      }
  </style>
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
			const length = Math.min(numOfTriangles, triangleColors.length);
			for (let i = 0; i < length; i++) {
				context.beginPath();
				context.moveTo(i * triangleWidth, 0);
				context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
				context.lineTo((i + 1) * triangleWidth, 0);
				context.closePath();
				context.fillStyle = triangleColors[i];
				context.fill();
			}
		});
	</script>
	
</head>
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
	<script>
		const text = "Attention all window lovers! Search our website for the squeegee and win a free clean!";
		let i = 0;
		function typeWriter() {
			if (i < text.length) {
				document.getElementById("typewriter-text").innerHTML += text.charAt(i);
				i++;
				setTimeout(typeWriter, Math.floor(Math.random() * 200) + 50); // randomize the typing speed
			}
		}
		typeWriter();
	</script>
</body></html>
