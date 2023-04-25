
<html>
  <head>
    <title>My Website</title><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
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

  <footer>
    <p>&copy; 2023 Loftieswindows. Connect with us:</p>
    <div class="social-media">
      <a href="https://www.facebook.com"><i class="fab fa-facebook-f facebook"></i></a>
      <a href="https://www.twitter.com"><i class="fab fa-twitter twitter"></i></a>
      <a href="https://www.instagram.com"><i class="fab fa-instagram instagram"></i></a>
    </div>
  </footer>
  </body>
