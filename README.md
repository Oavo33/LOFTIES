<html lang="en-US">
  <head><meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Lofties Windows</title>
    <meta name="description" content="Loftie">
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <link rel="icon" type="image/png" href="/path/to/favicon.png">
    <link rel="stylesheet" href="/My.First.Site/assets/css/style.css?v=c61e1577585ebe24df4f8190e73674368a10cb67">
  </head>
  <body>
    <article>
      <header>
        <div class="triangle"></div>
        <div class="triangle-content">
          LOFTIES
        </div>
        <div class="logo-text">Lofties Windows</div>
      </header><h1 style="display: flex; flex-direction: column; align-items: center;">
        <span style="display: block; text-align: center; font-family: 'Pacifico', cursive;">LOFTIES</span>
        <span style="display: block; text-align: center; font-family: 'Pacifico', cursive;">WINDOWS</span>
      </h1>
      <ul class="social">
        <li>
          <a href="#">
            <i class="twitter"><img src="https://img.icons8.com/color/48/000000/twitter.png" alt="Twitter"></i>
          </a>
        </li>
        <li>
          <a href="#">
            <i class="facebook"><img src="https://img.icons8.com/color/48/000000/facebook.png" alt="Facebook"></i>
          </a>
        </li>
        <li>
          <a href="#">
            <i class="instagram"><img src="https://img.icons8.com/color/48/000000/instagram-new.png" alt="Instagram"></i>
          </a>
        </li>
      </ul>    
      <header>
        <article>
          <main>
            <section>
              <h2>About Us</h2>
              <p>Our work.</p>
            </section>
            <section>
              <h2>Our Services</h2>
              <ul>
                <li>Golf</li>
                <li>Gutter Cleaning</li>
              </ul>
            </section>
            <section>
              <h2>The Team</h2>
              <p>Old team.</p>
            </section><aside>
        <h2>Payment Methods</h2>
        <p>cards.</p>
      </aside>
    </main>
    <footer>
    <nav>
      <ul class="social">
        <li>
          <a href="#">
            <i class="twitter"><img src="https://img.icons8.com/color/48/000000/twitter.png" alt="Twitter"></i>
          </a>
        </li>
        <li>
          <a href="#">
      <i class="facebook"><img src="https://img.icons8.com/color/48/000000/facebook.png" alt="Facebook"></i>
    </a>
  </li>
  <li>
    <a href="#">
      <i class="instagram"><img src="https://img.icons8.com/color/48/000000/instagram-new.png" alt="Instagram"></i>
    </a>
  </li>
</ul>
      <h1>Lofties Hangman</h1>
          <p>Guess the word, Reload page to start again:</p>
          <p id="word"></p>
          <p>Guess a letter:</p>
          <input type="text" id="guessInput" />
          <button id="guessButton">Guess</button>
          <p id="guesses"></p>
          <p id="result"></p>
      <script>
        const words = ["birkenhead", "tranmererovers", "solarpower", "future", "LoftiesWindows", "windowcleaner", "football", "golf", "tennis", "car", "bus", "train", "wirralglobe", "paulogradyrip", "newbrighton", "rockferry", "artificialintelligence"];
        let chosenWord = words[Math.floor(Math.random() * words.length)];
        let wordToGuess = "";
        let guesses = "";
        let guessesRemaining = 10;
  function init() {
    for (let i = 0; i < chosenWord.length; i++) {
      wordToGuess += "_ ";
    }
    document.getElementById('word').innerText = wordToGuess;
    document.getElementById('guessButton').addEventListener('click', makeGuess);
  }
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
        correctGuess = true;}
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
      }}
  }
init();
      </script>
      <p>&copy; 2023 My Website. All rights reserved.</p>
    </footer>
<script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
>
</body>
</html>
<style>body {
    color: #00B3B3;
    background-color: #800000;
  }
header {
    background-color: #800000;
    background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
    background-size: cover;
    background-position: center;
    color: #00B3B3;
    font-family: 'Pacifico', cursive;
    padding: 100px;
    text-shadow: 2px 2px #800000;
    position: relative;
  }
h1 {
  font-size: 25px;
  text-align: center;
  letter-spacing: 14px;
  position: relative;
  top: -170px;
  left: -78px;
  transform: translateY(-50%);
  opacity: 0;
  animation: flash 14s infinite;
  text-shadow: 0px 0px 10px rgba(0,0,0,0.5);
  font-weight: bold;
  display: flex;
  align-items: center;
  -webkit-text-stroke: 1px #00B3B3;
  color: #800000;
}h1 span {
  margin: auto;
}@keyframes flash {
  0% { opacity: 0; }
  50% { opacity: 1; }
  100% { opacity: 0; }
}
 .triangle {
  width: 0;
  height: 0;
  border-top: 20px solid transparent;
  border-right: 20px solid #00B3B3;
  border-bottom: 20px solid transparent;
  border-left: 20px solid #00B3B3;
  transform: rotate(-45deg);
  position: absolute;
  bottom: 8;
  left: 8;
  z-index: 2;
}.triangle {
  width: 0;
  height: 0;
  border-top: 10px solid transparent;
  border-right: 10px solid #00B3B3;
  border-bottom: 10px solid transparent;
  border-left: 10px solid #00B3B3;
  transform: rotate(-45deg);
  position: absolute;
  bottom: 11px;
  left: 11px;
  z-index: 2;
}.triangle-content {
  position: absolute;
  top: 90%;
  left: 4.5%;
  transform: translate(-50%, -50%) rotate(-315deg);
  color: #800000;
  font-size: 10px;
  font-weight: bold;
  text-align: center;
  z-index: 3;
  background-color: transparent;
  text-shadow: none;
}.logo-text {
  position: absolute;
  top: 2px;
  left: 40px;
  font-size: 7px;
  font-weight: 100;
  color: #00B3B3;
  -webkit-text-stroke: 1px #00B3B3;
  animation: move 14s infinite alternate;
}@keyframes move {
  from {
    transform: translateX(-140);
  }
  to {
    transform: translateX(330px);
  }
}article {
    text-align: center;}
   ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;}
ul li:not(:last-child) {
    margin-right: 20px;}
footer {
    background-color: #333;
    color: #fff;
    padding: 20px;}
footer p {
    margin: 0;
  }
footer a {
    color: #fff;
    text-decoration: none;
  }
footer ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;}
footer ul li:not(:last-child) {
    margin-right: 20px;
  }
footer ul li a:hover {
    text-decoration: underline;
  }
.social {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 40px;
  }
.social li:not(:last-child) {
    margin-right: 20px;
  }
.social a {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #fff;
    border-radius: 50%;
    height: 40px;
    width: 40px;
    color: #800000;
    text-decoration: none;
    font-size: 20px;
  }.social a i:hover {
    color: #fff;
    background-color: #800000;
    border-radius: 50%;
  }
.social a i.twitter img {
    height: 100%;
    width: 100%;
    object-fit: contain;
  }
.social a i.facebook img {
    height: 100%;
    width: 100%;
    object-fit: contain;
  }
.social a i.instagram img {
    height: 100%;
    width: 100%;
    object-fit: contain;
  }
a {
    text-decoration: none;
  }
.section {
  border: !important none;}
</style>

