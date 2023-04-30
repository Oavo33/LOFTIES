<!DOCTYPE html>
<html>

<head>
  <title>My Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
  <style>
    body {
      color: #00B3B3;
      background-color: #800000;
    }header { 
  background-color: #800000;
  background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
  background-size: cover;
  background-position: center;
  color: #fff; /* change to white */
  font-family: 'Pacifico', cursive;
  padding: 140px;
  text-shadow: 2px 2px #800000;
  position: relative;
}

    .logo {
      position: absolute;
      bottom: 0;
      left: 0;
      font-size: 10px;
      margin: 0;
    }

    .logo-text {
  position: absolute;
  top: 1px;
  right: 34px;
  font-size: 30px;
  margin: 20px;
  text-shadow: 2px 2px #800000;
  color: #fff; /* add this line to set the color to white */
  animation-name: moveText;
  animation-duration: 7s;
  animation-direction: alternate;
  animation-iteration-count: infinite;
}

   .logo:after {
      content: "LOFTIES";
      position: absolute;
      bottom: 0;
      left: 0;
      height: 26;
      width: 0;
      border-bottom: 50px solid #800000;
      border-right: 50px solid transparent;
   }

    .logo:hover:after {
      border-bottom: 150px solid #00B3B3;
    }@keyframes moveText {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(50px);
  }
}
  </style>
</head>

<body>
  <header>
    <div class="logo"></div>
    <div class="logo-text">LoftiesWindows</div>
  </header>
</body>

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
       <section style="background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80'); background-repeat: no-repeat; background-size: 570px; background-position: center;">
        <h3>The Advantages of Old-Fashioned Window Cleaning Methods</h3>
        <p>Old-fashioned window cleaning methods have been around for decades and are still preferred by many because of their proven effectiveness. One of the biggest advantages of traditional window cleaning is the ability to clean difficult stains like bird droppings from windows and sills. The use of a squeegee and a chamois cloth ensures a streak-free finish, which is not always the case with new methods. Additionally, the amount of water used in traditional methods is typically less than that used in newer methods, resulting in a quicker drying time and less potential for damage to the surrounding property. Furthermore, the manual nature of traditional methods allows for more attention to detail and a higher level of quality control. Overall, old-fashioned window cleaning methods provide a time-tested and reliable approach to window cleaning that can deliver excellent results.</p>
      </section> </article>
    <aside>
      <h2>Payment Methods</h2>
      <p>We accept cash, cryptocurrency (you pay exchange fee), and all major credit cards.</p>
    </section></aside>
<head>
	<meta charset="utf-8">
	<title>Hangman</title>
</head>
<body>
	<h1>LoftiesHangman</h1>
	<p>Guess the word,Reload page to stat again:</p>
	<p id="word"></p>
	<p>Guess a letter :</p>
	<input type="text" id="guessInput">
	<button id="guessButton">Guess</button>
	<p id="guesses"></p>
	<p id="result"></p>
	<script>
		const words = ["birkenhead", "tranmererovers", "solarpower", "future", "loftieswindows", "windowcleaner", "football", "golf", "tennis", "car", "bus", "train", "wirralglobe", "paulogradyrip", "newbrighton", "rockferry", "artificialintelligence",];
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
   
  </body>
</html>
</html>
