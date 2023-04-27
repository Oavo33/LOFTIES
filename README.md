<!DOCTYPE html>
<html>
  <head>
    <title>Loftieswindows</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
      body {
        background-color: #7c7c7c;
        font-family: Arial, sans-serif;
      }

      header {
        background-color: #00fff2;
        color: rgb(126, 126, 126);
        text-align: center;
        padding: 20px;
        height: 400px;
        background-image: url('https://picsum.photos/id/1064/1200/400');
        background-size: cover;
        background-position: center;
        display: flex;
        justify-content: center;
        align-items: center;
      }

      nav {
        background-color: #7e7e7e;
        padding: 10px;
      }

      nav ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        overflow: hidden;
      }

      nav li {
        display: inline-block;
        margin-right: 20px;
      }

      nav li a {
        display: block;
        color: #00ffff;
        text-align: center;
        padding: 10px;
      }

      nav li a:hover {
        background-color: #00eeff;
        color: rgb(122, 122, 122);
      }

      section {
        padding: 20px;
      }

      footer {
        background-color: #00ffff;
        color: rgb(122, 122, 122);
        text-align: center;
        padding: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
      }

      .social-media {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
      }

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
      }

      h2 {
        font-size: 32px;
        color: #00ffff;
        margin-bottom: 20px;
      }

      h3 {
        font-size: 24px;
        color: #00ffff;
        margin-bottom: 10px;
      }
    </style>
  </head>

  <body>
    <header>
      <h1>Loftieswindows</h1>
    </header>

    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About Us</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
    </nav>

    <section>
     
<h2>Welcome to Loftieswindows</h2>
  <h3>About Us</h3>
  <p>At Loftieswindows, we have been providing professional window cleaning for over 20 years.</p>

  <h3>Our Services</h3>
  <ul>
    <li>Residential Window Cleaning</li>
        <li>Gutter Cleaning</li>
  </ul>

  <h3>The Advantages of Old-Fashioned Window Cleaning Methods</h3>
      <p>Old-fashioned window cleaning methods have been around for decades and are still preferred by many because of their proven effectiveness. One of the biggest advantages of traditional window cleaning is the ability to clean difficult stains like bird droppings from windows and sills. The use of a squeegee and a chamois cloth ensures a streak-free finish, which is not always the case with new methods. Additionally, the amount of water used in traditional methods is typically less than that used in newer methods, resulting in a quicker drying time and less potential for damage to the surrounding property. Furthermore, the manual nature of traditional methods allows for more attention to detail and a higher level of quality control. Overall, old-fashioned window cleaning methods provide a time-tested and reliable approach to window cleaning that can deliver excellent results.</p>
    </article>
    <aside>
      <h2>Payment Methods</h2>
      <p>We accept cash, cryptocurrency (you pay exchange fee), and all major credit cards.</p>
    </aside>
<head>
	<meta charset="utf-8">
	<title>Hangman</title>
</head>
<body>
	<h1>Hangman</h1>
	<p>Guess the word:</p>
	<p id="word"></p>
	<p>Guess a letter:</p>
	<input type="text" id="guessInput">
	<button id="guessButton">Guess</button>
	<p id="guesses"></p>
	<p id="result"></p>
	<script>
		const words = ["birkenhead", "tranmererovers", "solarpower", "future", "loftieswindows", "windowcleaner", "football", "golf", "tennis", "car", "bus", "train", "wirralglobe", "paulogradyrip", "newbrighton", "rockferry", "artificialintelligence", "supercalifragilisticexpialidocious"];
		let chosenWord = words[Math.floor(Math.random() * words.length)];
		let wordToGuess = "";
		let guesses = "";
		let guessesRemaining = 10;

		// Initialize the game
		function init() {
			for (let i = 0; i < chosenWord.length; i++) {
				wordToGuess += "_ ";
			}
			document.getElementById('word').innerText = wordToGuess;
			document.getElementById('guessButton').addEventListener('click', makeGuess);
		}

		// Make a guess
		function makeGuess() {
			let guess = document.getElementById('guessInput').value.toLowerCase();
			if (guess.length !== 1 || !guess.match(/[a-z]/i)) {
				alert("Please enter a single letter.");
				return;
			}
			if (guesses.includes(guess)) {
				alert("You already guessed that letter.");
				return;
			}
			guesses += guess;
			document.getElementById('guesses').innerText = "Guesses: " + guesses;
			let wordToGuessArray = wordToGuess.split(" ");
			let correctGuess = false;
			for (let i = 0; i < chosenWord.length; i++) {
				if (chosenWord[i] === guess) {
					wordToGuessArray[i] = guess;
					correctGuess = true;
				}
			}
			wordToGuess = wordToGuessArray.join(" ");
			document.getElementById('word').innerText = wordToGuess;
			if (!wordToGuess.includes("_")) {
				document.getElementById('result').innerText = "You win!";
				document.getElementById('guessButton').removeEventListener('click', makeGuess);
			} else if (!correctGuess) {
				guessesRemaining--;
				if (guessesRemaining === 0) {
					document.getElementById('result').innerText = "You lose! The word was " + chosenWord + ".";
					document.getElementById('guessButton').removeEventListener('click', makeGuess);
				} else {
					document.getElementById('result').innerText = "Wrong guess. " + guessesRemaining + " guesses remaining.";
				}
			}
		}

		init();
	</script>
</body>
    <footer>
      <p>&copy; 2023 Loftieswindows. Connect with us:</p>
      <div class="social-media">
  <a href="https://www.facebook.com"><i class="fab fa-facebook-f facebook"></i></a>
  <a href="https://www.twitter.com"><i class="fab fa-twitter twitter"></i></a>
  <a href="https://www.instagram.com"><i class="fab fa-instagram instagram"></i></a>
  <a href="https://www.youtube.com"><i class="fab fa-youtube youtube"></i></a>
  <a href="https://www.tiktok.com"><i class="fab fa-tiktok tiktok"></i></a>
</div>
    </footer>
  </body>
</html>