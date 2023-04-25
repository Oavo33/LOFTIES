# karl.github.io
karl!!!!1
<!DOCTYPE html>
<html>
  <head>
    <title>My Website</title><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>.planet {
		position: absolute;
		top:38%;
		left: 85%;
		transform: translate(-50%, -50%);
		border-radius: 70%;
	}

	.sun {
		position: absolute;
		top: 38%;
		left: 85%;
		transform: translate(-50%, -50%);
		background-color: #00ffff;
		width: 80px;
		height: 80px;
		border-radius: 70%;
	}

	.mercury {
		width: 10px;
		height: 10px;
		background-color: #8400ff;
		animation: orbit 5s linear infinite;
	}

	.venus {
		width: 15px;
		height: 15px;
		background-color: #eeff00;
		animation: orbit 10s linear infinite;
	}

	.earth {
		width: 20px;
		height: 20px;
		background-color: #00fd4c;
		animation: orbit 15s linear infinite;
	}

	.mars {
		width: 18px;
		height: 18px;
		background-color: #ff0000;
		animation: orbit 20s linear infinite;
		transform-origin: 0% 50%;
	}

	.jupiter {
		width: 30px;
		height: 30px;
		background-color: #0011ff;
		animation: orbit 25s linear infinite;
	}

	.saturn {
		width: 25px;
		height: 25px;
		background-color: #ff00ea;
		animation: orbit 35s linear infinite;
	}

	.uranus {
		width: 20px;
		height: 20px;
		background-color: #791414;
		animation: orbit 45s linear infinite;
	}

	.neptune {
		width: 18px;
		height: 18px;
		background-color: #000000;
		animation: orbit 55s linear infinite;
	}

	@keyframes orbit {
		from {
			transform: rotate(0deg) translateX(80px) rotate(0deg);
		}
		to {
			transform: rotate(360deg) translateX(80px) rotate(-360deg);
		}
	}
      body {background-color: #7c7c7c; font-family: Arial, sans-serif;}
      header {background-color: #00fff2; color: rgb(126, 126, 126); text-align: center; padding: 20px;}
      nav {background-color: #7e7e7e; padding: 10px;}
      nav ul {list-style-type: none; margin: 0; padding: 0; overflow: hidden;}
      nav li {display: inline-block; margin-right: 20px;}
      nav li a {display: block; color: #00ffff; text-align: center; padding: 10px;}
      nav li a:hover {background-color: #00eeff; color: rgb(122, 122, 122);}
      section {padding: 20px;}
      footer {background-color: #00ffff; color: rgb(122, 122, 122); text-align: center; padding: 20px;}
      .social-media a {
      display: inline-block;
      margin-right: 20px;
    }

    .social-media img {
      width: 40px;
      height: 40px;
      margin-right: 10px;
    }

    .social-media i {
      font-size: 30px;
      margin-right: 10px;
    }

    .social-media .facebook {
      color: #3B5998;
    }

    .social-media .twitter {
      color: #1DA1F2;
    }

    .social-media .instagram {
      color: #C13584;
    }</style>
  </head>
  <body>
	  <header style="text-align: center;">
		  <div style="display: flex; align-items: center; justify-content: center;">
			  <img src="C:\Users\DEMO\Downloads\site1.jpg" alt="Picture of Loftieswindows" style="width: 70px; height: auto;" />
			  <h1 style="margin: 0;">Loftieswindows</h1>
			  <img src="C:\Users\DEMO\Downloads\site2.jpg" alt="Picture of Loftieswindows" style="width: 70px; height: auto;" />
		  </div>
	  </header>
	  
	<div class="sun"></div>
	<div class="planet mercury"></div>
	<div class="planet venus"></div>
	<div class="planet earth"></div>
	<div class="planet mars"></div>
	<div class="planet jupiter"></div>
	<div class="planet saturn"></div>
	<div class="planet uranus"></div>
	<div class="planet neptune"></div>
  
	  <main>
<article>
			  <h2>About Us</h2>
	  <p>At Loftieswindows, we have been providing professional window cleaning for over 20 years.</p>
	</article>
  
	
	<article>
	  <h2>Services</h2>
	  <ul>
		<li>Residential Window Cleaning</li>
		<li>Gutter Cleaning</li>
	  </ul>
	  <h3>The Advantages of Old-Fashioned Window Cleaning Methods</h3>
	  <p>Old-fashioned window cleaning methods have been around for decades and are still preferred by many because of their proven effectiveness. One of the biggest advantages of traditional window cleaning is the ability to clean difficult stains like bird droppings from windows and sills. The use of a squeegee and a chamois cloth ensures a streak-free finish, which is not always the case with new methods. Additionally, the amount of water used in traditional methods is typically less than that used in newer methods, resulting in a quicker drying time and less potential for damage to the surrounding property. Furthermore, the manual nature of traditional methods allows for more attention to detail and a higher level of quality control. Overall, old-fashioned window cleaning methods provide a time-tested and reliable approach to window cleaning that can deliver excellent results.</p>
	</article>
    <head>
        <title>Dart Game</title>
        <style>
            #game-container-wrapper {
                position: absolute;
                top:86%;
                left: 41%;
                transform: translate(-50%, -50%);
            }
            #game-container {
                width:180px;
                height: 80px;
                position: relative;
                border: 1px solid black;
            }
            
            .dartboard {
                width: 135px;
                height: 50px;
                border-radius: 50%;
                border: 2px solid black;
                background-color: #00ffff;
                position: absolute;
                top:11px;
                left: 20px;
            }
            .dart {
                width: 9px;
                height: 9px;
                border-radius: 50%;
                background-color: #FF0000;
                position: absolute;
                top: 11.75px;
                left: 17.4px;
                display: none;
            }
            .prize {
                position: absolute;
                top: 14px;
                left:40px;
                font-size: 15px;
                font-weight: bold;
                color: #000000;
                display: none;
            }
            #throw-dart-button {
                position: absolute;
                top: 75px;
                left: 75px;
            }
            .social-media a {
                display: inline-block;
                margin-right: 10px;
            }

            .social-media img {
                width: 30px;
                height: 30px;
            }
        </style>
    </head>
    <body>
        
        <div id="game-container-wrapper">
            <div id="game-container">
                <div class="dartboard"></div>
                <div class="dart"></div>
                <div class="prize">Your windows where cleaned today Thanks!</div>
            </div>
        </div>
        <button onclick="throwDart()">Did you get a note?Press here if yes</button>
    
        <script>
            var dartboard = document.querySelector(".dartboard");
            var dart = document.querySelector(".dart");
            var prize = document.querySelector(".prize");
            var score = 0;
            var maxScore = 100;
    
            function throwDart() {
                var x = Math.floor(Math.random() * dartboard.offsetWidth);
                var y = Math.floor(Math.random() * dartboard.offsetHeight);
                dart.style.left = x + "px";
                dart.style.top = y + "px";
                dart.style.display = "block";
    
                if (x > 30 && x < 50 && y > 30 && y < 50) {
                    score += 50;
                } else if (x > 20 && x < 60 && y > 20 && y < 60) {
                    score += 25;
                } else if (x > 10 && x < 70 && y > 10 && y < 70) {
                    score += 10;
                } else {
                    score += 0;
                }
    
                if (score >= maxScore) {
                    prize.style.display = "block";
                }
    
                setTimeout(function() {
                    dart.style.display = "none";
                }, 1000);
            }
        </script>
	<aside>
	  <h2>Payment Methods</h2>
	  <p>We accept cash,cryptocurrency(you pay exchange fee), and all major credit cards.</p>
	</aside>
</article></main>
  <footer>
    <p>&copy; 2023 Loftieswindows. Connect with us:</p>
    <div class="social-media">
      <a href="https://www.facebook.com"><i class="fab fa-facebook-f facebook"></i></a>
      <a href="https://www.twitter.com"><i class="fab fa-twitter twitter"></i></a>
      <a href="https://www.instagram.com"><i class="fab fa-instagram instagram"></i></a>
    </div>
  </footer>
  </body>
  </html>