<!DOCTYPE html>
<html>
<head>
	<title>LoftiesWindows</title>
	<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
	<link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

	<style>
		header {
			background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
			background-size: cover;
			background-position: left;
			color:#800000;
			font-family: 'Dancing Script', cursive;
			padding: 90px;
			text-align: right;
			text-shadow: 2px 2px #000;
			position: relative;
		}
		
		.triangle {
			width: 10vw;
			height: 7vw;
			background-color: #800000;
			position: absolute;
			bottom: 55px;
			left: 10px;
			transform: translate(10%, 90%);
			clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
			display: flex;
			justify-content: center;
			align-items: center;
			z-index: 2;
			cursor: pointer;
			transition: all 0.3s ease;
		}
		
		.triangle:hover {
			background-color: #800000;
			transform: translate(10%, 80%);
			box-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
		}
		
		.triangle-text {
			color: #00B3B3;
			font-size: 8px;
			text-align: center;
			text-transform: uppercase;
			letter-spacing: 2px;
			padding: 10px;
			position: absolute;
			top: 90%;
			left: 50%;
			transform: translate(-50%, -50%);
		}
		
		.logo {
  font-size: 50px;
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 7s ease;
  position: absolute;
  left: 170px;
  top: 10px;
}

.logo:hover span {
  background-color: #800000;
  color: #00B3B3;
  box-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
}

.logo span {
  background-color: #00B3B3;
  border-radius: 50%;
  display: inline-block;
  height: 30px;
  width: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-right: 10px;
  text-align: center;
  box-shadow: 2px 2px black;
  transition: all 0.3s ease;
}

.logo span::before {
  content: "L";
  display: inline-block;
  font-size: 25px;
  font-weight: bold;
  transform: rotate(-20deg);
  transition: all 0.3s ease;
}

.logo-text {
  font-size: 20px;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 10px;
  margin: 0;
  padding: 0;
}
	
</style>
</head>
<body>
	<header>
  <div class="logo">
    <span></span>
    <div class="logo-text">LoftiesWindows</div>
  </div>
  <div class="triangle">
    <div class="triangle-text">&copyLOFTIES</div>
  </div>
</header></head>

<script>
	const triangle = document.querySelector('.triangle');

	triangle.addEventListener('click', () => {
  		alert('your windows where cleaned today  !');
	});
</script>
</body>
</html>




