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

		.logo-text {
			font-size: 30px;
			margin: 0;
			text-shadow: 2px 2px #000;
		}
        
        .logo:after {
			content: "";
			display: inline-block;
			height: 0;
			width: 0;
			border-top: 50px solid #800000;
			border-right: 50px solid transparent;
			transform: rotate(-45deg);
            margin-left: 10px;
		}

		.logo:hover:after {
			border-top: 50px solid #00B3B3;
		}
	</style>
</head>
<body>
	<header>
		<div class="logo">
			<div class="logo-text">Lofties<div>
		</div>
	</header>
</body>
</html>
