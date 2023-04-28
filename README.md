<!DOCTYPE html>
<html>
<head>
	<title>My Website</title>
	<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
	<style>
		header {
			background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
			background-size: cover;
			background-position: center;
			color: #fff;
			font-family: 'Pacifico', cursive;
			padding: 20px;
			text-align: center;
			text-shadow: 2px 2px #000;
		}

		.logo {
			font-size: 40px;
			margin: 0;
		}

		.logo span {
			background-color: rgba(255,255,255,0.8);
			border-radius: 5px;
			display: inline-block;
			height: 50px;
			line-height: 50px;
			margin-right: 10px;
			text-align: center;
			width: 50px;
		}

		.logo span::before {
			content: "L";
			display: inline-block;
			font-size: 30px;
			font-weight: bold;
			transform: rotate(-20deg);
		}

		.logo span:hover {
			background-color: rgba(255,255,255,1);
			color: #000;
		}

		.logo-text {
			font-size: 30px;
			margin: 0;
			text-shadow: 2px 2px #000;
		}
	</style>
</head>
<body>
	<header>
		<div class="logo">
			<span></span>
			<div class="logo-text">Lofties</div>
		</div>
	</header>
</body>
</html>

