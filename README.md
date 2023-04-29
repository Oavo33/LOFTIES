<!DOCTYPE html>
<html>
<head>
	<title>My Website</title>
	<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
	<style>
		header {
			background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
			background-size: cover;
			background-position: left;
			color: #fff;
			font-family: 'Montserrat', sans-serif;
			padding:90px;
			text-align: right;
			text-shadow: 2px 2px #000;
			position: relative; /* added */
		}
.triangle {
  width: 14vw;
  height: 10vw;
  background-color: #800000;
  position: absolute;
  bottom:55px;
  left: 10px;
  transform: translate(10%, 90%);
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 2;
}
.triangle-text {
color: #fff;
font-size: 10px;
text-align: center;
text-transform: uppercase;
letter-spacing: 2px;
padding: 10px;
position: absolute;
top: 90%;
left: 50%;
transform: translate(-50%, -50%);
}	.logo {
		font-size: 50px;
		margin: 0;
		display: flex;
		align-items: center;
		justify-content: center;
	}

		.logo span {
		background-color: rgba(255,255,255,0.8);
		border-radius: 50%;
		display: inline-block;
		height: 100px;
		width: 100px;
		display: flex;
		align-items: center;
		justify-content: center;
		margin-right: 10px;
		text-align: center;
		box-shadow: 2px 2px #000;
	}

		.logo span::before {
		content: "L";
		display: inline-block;
		font-size: 50px;
		font-weight: bold;
		transform: rotate(-20deg);
	}

		.logo span:hover {
		background-color: rgba(255,255,255,1);
		color: #000;
		box-shadow: 4px 4px #000;
	}

		.logo-text {
		font-size: 50px;
		margin: 0;
		text-shadow: 2px 2px #000;
		color: #fff;
		text-transform: uppercase;
		letter-spacing: 5px;
		padding-top: 20px;
		line-height: 1.2;
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
</header>
<script>
	const triangle = document.querySelector('.triangle');

	triangle.addEventListener('click', () => {
  		alert('your windows where cleaned today  !');
	});
</script>
</body>
</html>




