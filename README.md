<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Lofties Windows</title>
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
  <style>header {
      background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
      background-size: 100%;
      background-position: center 65%;
      padding: 100px;
      position: relative;
      text-align: center;}ul {
  list-style-type: none;
  overflow: hidden;
  display: flex;
  justify-content: flex-end;
  position: absolute;
  bottom: -14px;
  right: 0;}
    li a {
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      text-align: center;
      padding: 1px 1px;
      text-decoration: none;
      font-size: 10px;
      font-weight: bold;
      animation-duration: 5s;
      animation-fill-mode: forwards;
      animation-timing-function: ease-out;
    }
    li:nth-child(1) a {
      animation-name: fadeInLeft;
    }
    li:nth-child(2) a {
      animation-name: pop;
      animation-delay: 5s;
    }
    li:nth-child(3) a {
      animation-name: zoomInRight;
    }
    .icon {
      display: inline-block;
      font-size: 14px;
      margin-right: 0px;
      margin-left: 0px;
    }
    .video-icon {
      color: #f00;
    }
    .game-icon {
      color: #0f0;
    }
    .music-icon {
      color: #00f;
    }
    #space-info {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: #fff;
      padding: 20px;
      border: 1px solid #ccc;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
      visibility: hidden;
      z-index: 1;
      text-align: center;
      font-family: Arial, sans-serif;
      font-size: 1.2em;
      line-height: 1.5;
    }
    @keyframes fadeInLeft {
      0% {
        opacity: 0;
        transform: translateX(-100%);
      }
      100% {
        opacity: 1;
        transform: translateX(0);
      }
    }
    @keyframes pop {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.5);
      }
      100% {
        transform: scale(1);
      }
    }
    @keyframes zoomInRight {
      0% {
        opacity:: 0;
        transform: scale(0.1) translateX(200%);
      }
      100% {
        opacity: 1;
        transform: scale(1) translateX(0);
      }
    }@media only screen and (max-width: 600px) {
        header }</style>
  </head>
  <body>
    <header>
      <ul>
        <li>
          <a href="#contact" class="music-tab">
            <span class="icon music-icon">&#x1F3B5;</span>
            Music
          </a>
        </li>
        <li>
          <a href="#contact" class="video-tab">
            <span class="icon video-icon">&#x1F3A5;</span>
            Videos
          </a>
        </li>
        <li>
          <a href="#contact" class="game-tab">
            <span class="icon game-icon">&#x1F3AE;</span>
            Games
          </a>
        </li>
      </ul>
<div id="space-info">
		<h2>Did you know?</h2>
		<p>Space is vast and full of mysteries. There are countless stars, planets, and galaxies out there waiting to be explored. Some of the most fascinating space facts include:</p>
		<um>
			<li>The sun makes up 99.86% of the mass of the solar system.</li>
			<li>The largest volcano in the solar system is Olympus Mons on Mars. It is over 13 miles high.</li>
			<li>The Kuiper Belt is a region of the solar system beyond the orbit of Neptune that is home to dwarf planets like Pluto.</li>
			<li>Astronauts on the International Space Station see 16 sunrises and sunsets each day.</li>
			<li>The first living creature in space was a dog named Laika.</li>
		</um>
		<p>There is so much more to learn about space. Keep exploring!</p>
	</div>
    </header>
    <script>
    const spaceInfo = document.getElementById("space-info");
		const hoverText = document.querySelector('ul');
    hoverText.addEventListener('mouseover', () => {
			spaceInfo.style.visibility = 'visible';
		});
    hoverText.addEventListener('mouseout', () => {
			spaceInfo.style.visibility = 'hidden';
		});

</script>

</body>
</html>


