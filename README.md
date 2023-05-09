<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lofties Windows</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>header {
  background-size:100%;
  padding:80px;
  display:flex;
  background-position:center 65%;
  font-family: 'UnifrakturMaguntia';
  justify-content:space-between;
  align-items:center;
  background-image:url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
  position:relative;
} canvas {
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 4;
} h1{
  color: #00b3b3;
  font-size: 30px;
  margin: 0 0 10px;
  animation: fade-in-out 2s infinite;
}  h1 span {
  display: inline-block;
  position: relative;
  transition: transform 1s ease-out;
}h1 span:hover {
  transform: translateX(30px);
}p {
  color: #00b3b3;
  font-size: 10px;
  margin: 0;
  padding: 5px;
  border: 1px solid #800000;
  transition: all 0.5s ease-out;
  position: relative;
}p:hover {
  color: #00b3b3;
  border: 2px solid #00b3b3;
  box-shadow: 0 0 10px #800000;
}p:hover .star {
  opacity: 1;
}.star {
  position: absolute;
  width: 14px;
  height: 14px;
  background-color: black;
  border-radius: 50%;
  opacity: 0;
  transition: all 1s ease-out;
}.star:hover {
  transform: scale(3);
}.star1 {
  top: 0%;
  left: 5%;
}.star2 {
  top: 50%;
  left: 45%;
}.social-icons-container {
  position: absolute;
  top: 14px;
  left: 14px;
  display: flex;
  flex-direction: column;
  gap: 2px;
}.social-icons-container img {
  height: 14px;
  width: 14px;
  margin: 3px;
  filter: brightness(60%);
  transition: filter 0.3s ease-in-out;
  display: flex;
  justify-content: center;
  align-items: center;
  border: none; 
}.social-icons-container img:hover {
  filter: brightness(100%);
}.bottom-right {
  position: absolute;
  bottom: 0;
  right: 0;
  display: flex;
  gap: 1px;
}.bottom-right li {
  list-style:none;
  }@keyframes fade-in-out {
        0% { opacity: 1; }
        50% { opacity: 0.5; }
        100% { opacity: 1; }          
	}@keyframes bounce {
        0% {
          left: 0%;
        }
        100% {
          left: 100%;
        }
      }@keyframes fadeInLeft {
      0% {
        opacity: 0;
        transform: translateX(-100%);
      }
      100% {
        opacity: 1;
        transform: translateX(0);
      }
    }@keyframes pop {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.5);
      }
      100% {
        transform: scale(1);
      }
    }@keyframes zoomInRight{
      0% {
        opacity: 0;
        transform: scale(0.1) translateX(200%);
      }
      100% {
        opacity: 1;
        transform: scale(1) translateX(0);
      } @media only screen and (max-width: 600px) {
  }}</style>
</head>
<body>
  <header><canvas id="canvas"></canvas><div class="social-icons-container">
      <a href="https://www.facebook.com"><img src="https://img.icons8.com/clouds/64/000000/facebook.png" alt="Facebook"></a>
      <a href="https://www.discord.com"><img src="https://img.icons8.com/clouds/64/000000/discord-logo.png" alt="Discord"></a>
      <a href="https://www.youtube.com"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></a>
    </div>
    <ul class="bottom-right">
      <jake><a href="#contact" class="video-tab"><span class="icon video-icon">&#x1F3A5;</span>Videos</a></jake>
      <jake><a href="#contact" class="music-tab"><span class="icon music-icon">&#x1F3B5;</span>Music</a></jake>
      <jake><a href="#contact" class="game-tab"><span class="icon game-icon">&#x1F3AE;</span>Games</a></jake>
    </ul><h1><span>L</span>ofties<span>W</span>indows</h1>
      <p>Attention all window lovers! Search our website for the squeegee and win a free clean!
        <span class="star star1">&#9733;</span>
        <span class="star star2">&#9733;</span>
        <span class="star star3">&#9733;</span>
      </p>
  </header><script>
      window.addEventListener('load', () => {
        const canvas = document.getElementById('canvas');
        const context = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = 100;
        const numOfTriangles = 14;
        const triangleWidth = canvas.width / numOfTriangles;
        const triangleHeight = Math.sqrt(0.2) / 2 * triangleWidth;
        const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
        for (let i = 0; i < numOfTriangles; i++) {
          context.beginPath();
          context.moveTo(i * triangleWidth, 0);
          context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
          context.lineTo((i + 1) * triangleWidth, 0);
          context.closePath();
          context.fillStyle = triangleColors[i % triangleColors.length];
          context.fill();
		  window.addEventListener('load', () => {
        const canvas = document.getElementById('canvas');
        const context = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
        const numOfTriangles = 14;
        const triangleWidth = canvas.width / numOfTriangles;
        const triangleHeight = Math.sqrt(0.5) / 2 * triangleWidth;
        const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
        for (let i = 0; i < numOfTriangles; i++) {
          context.beginPath();
          context.moveTo(i * triangleWidth, 0);
          context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
          context.lineTo((i + 1) * triangleWidth, 0);
          context.closePath();
          context.fillStyle = triangleColors[i % triangleColors.length];
          context.fill();
        }
      });
        }
      });
    </script>
  </body>
</html>



