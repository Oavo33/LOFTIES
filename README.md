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
			padding: 120px;
			text-align: right;
			text-shadow: 2px 2px #000;
			position: relative;
                        animation: fade-in 5s ease-in-out;
		}
		
		.triangle {
			width: 9vw;
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
			z-index: 3;
		}
		
		.triangle-text {
			color: #00B3B3;
			font-size:7px;
			text-align: center;
			text-transform: uppercase;
			letter-spacing: 2px;
			padding: 10px;
			position: absolute;
			top: 90%;
			right:-9%;
			transform: translate(0, -50%);
			z-index: 3;
		}

		header:hover .logo-text {
			color: #00B3B3;
		}
		
		.logo {
			position: absolute;
			top: 10px;
			right: 10px;
		}@keyframes fade-in {
  from { opacity: 0; }
  to { opacity: 1; }
}

      h1 {
        margin: 0;
      }
      p {
        margin-bottom: 0;
      }
      .container {
        margin: 20px auto;
        max-width: 800px;
        padding: 0 20px;
      }
      ul {
        list-style: none;
        margin: 0;
        padding: 0;
      }
      li {
        margin-bottom: 10px;
      }
      label {
        display: block;
        margin-bottom: 5px;
      }
      input[type=text], input[type=email], textarea {
        border: none;
        border-bottom: 2px solid #CCCCCC;
        padding: 10px;
        width: 100%;
        transition: border-bottom-color 0.2s ease-in-out;
      }
      input[type=text]:focus, input[type=email]:focus, textarea:focus {
        outline: none;
        border-bottom-color: #2C3E50;
      }
      input[type=submit] {
        background-color: #2C3E50;
        border: none;
        color: #FFFFFF;
        cursor: pointer;
        margin-top: 10px;
        padding: 10px 20px;
        border-radius: 5px;
      }
      input[type=submit]:hover {
        background-color: #7C92D3;
      }
      .error-message {
        color: #FF0000;
        margin-bottom: 10px;
      }
      .section {
        background-color: #F1F1F1;
        border: 2px solid #CCCCCC;
        border-radius: 10px;
        padding: 20px;
        margin-bottom: 20px;
        transition: border-color 0.2s ease-in-out;
      }
      .section:hover {
        border-color: #2C3E50;
      }
      .section h2 {
        font-size: 24px;
        margin-top: 0;
        margin-bottom: 20px;
      }
      .section ul {
        margin-bottom: 0;
      }
      .section li {
        margin-bottom: 5px;
      }
	
	</style>
</head>
<body>
	<header>
		<div class="logo">
			<span></span>
			<div class="logo-text" style="font-size: 72px;">LoftiesWindows</div>
		</div>
		<div class="triangle">
			<div class="triangle-text">&copy;LOFTIES</div>
		</div>
	</header>
</body>
</html>






