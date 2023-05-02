<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lofties Windows</title>
    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <style>
      body {
        color: #00b3b3;
        background-color: #800000;
        margin: 0;
        font-family: "Pacifico", cursive;
      }
      header {
        background-color: #800000;
        background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
        background-size: cover;
        background-position: center;
        color: #00b3b3;
        padding: 110px;
        position: relative;
        text-align: center;
        text-shadow: 2px 2px #800000;
      }
      #planet-system {
  position: absolute;
  top: 25%;
  right: 20%;
  transform: scale(0.4) translate(-50%, -50%);
  transform-origin: center center;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}.logo {
  position: absolute;
  bottom: 0;
  left: 0;
  margin: 0;
  display: flex;
  align-items: center;
}

.logo a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: #00b3b3;
}

.logo::after {
  content: "";
  position: absolute;
  bottom: 0px;
  left: -5px;
  height: 35px;
  width: 0;
  border-bottom: 70px solid transparent;
  border-right: 70px solid transparent;
  opacity: 0.8;
  transition: all 5s ease-in-out;
}

.logo:hover::after {
  content: "Its.The.Window Cleaner";
  position: absolute;
  bottom: 0px;
  left: -5px;
  height: 35px;
  width: 0;
  border-bottom: 70px solid #00b3b3;
  border-right: 70px solid transparent;
  opacity: 1;
  transition: all 3s ease-in-out;
  filter: hue-rotate(270deg) drop-shadow(2px 2px 2px #00b3b3)
          invert(19%) sepia(57%) saturate(6287%) hue-rotate(346deg)
          brightness(102%) contrast(102%);
}

.logo-text-container {
  transform: rotate(45deg);
  white-space: nowrap;
  position: relative;
  z-index: 1;
  top: -10px;
  left: -10px;
  transition: all 4s ease-in-out;
}

.logo:hover .logo-text-container {
  transform: rotate(360deg);
  transition: all 4s ease-in-out;
}

.logo-text {
  font-size: 14px;
  margin: 0 10px;
  text-shadow: 2px 2px #800000;
}

.logo2-text {
  font-size: 7px;
  position: absolute;
  top: 0;
  left: 0%;
  margin: 0 10px;
  text-shadow: 2px 2px #800000;
  animation: moveText 50s ease-in-out infinite;
}
.flash {
  animation: flash 14s infinite;
}

.header-text {
  position: absolute;
  top: 32%; 
  left: 32%;
  transform: translate(-50%, -50%);
  font-size: 44px;
}

p {
  font-size: 14px;
}
.sun {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			background-color: #00B3B3;
			border-radius: 50%;
			width: 100px;
			height: 100px;
		}

		.planet {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			border-radius: 50%;
			animation-timing-function: linear;
			animation-iteration-count: infinite;
			animation-name: flash14;
			animation-duration: 10s;
		}

		.mercury {
			width: 5px;
			height: 5px;
			background-color: #00B3B3;
			animation: orbit 39s linear infinite, flash14 2540s infinite;
		}

		.venus {
			width: 10px;
			height: 10px;
			background-color: #800000;
			animation: orbit 28s linear infinite, flash14 1540s infinite;
		}

		.earth {
			width: 12px;
			height: 12px;
			background-color: #00B3B3;
			animation: orbit 30s linear infinite, flash14 540s infinite;
		}

		.mars {
			width: 8px;
			height: 8px;
			background-color: #800000;
			animation: orbit 42s linear infinite, flash14 470s infinite;
		}

		.jupiter {
			width: 30px;
			height: 30px;
			background-color: #00B3B3;
			animation: orbit 55s linear infinite, flash14 630s infinite;
		}

		.saturn {
			width: 25px;
			height: 25px;
			background-color: #800000;
			animation: orbit 65s linear infinite, flash14 850s infinite;
		}

		.uranus {
			width: 20px;
			height: 20px;
			background-color: #00B3B3;
			animation: orbit 75s linear infinite, flash14 780s infinite;
		}

		.neptune {
			width: 18px;
			height: 18px;
			background-color: #800000;
			animation: orbit 85s linear infinite, flash14 580s infinite;
		}

		@keyframes orbit {
			from {
				transform: rotate(0deg) translateX(80px) rotate(0deg);
			}
			to {
				transform: rotate(360deg) translateX(80px) rotate(-360deg);
			}
		}

		@keyframes flash14 {
			0% {
				background-color: #00B3B3;
			}
			50% {
				background-color: #800000;
			}
			100% {
				background-color: #00B3B3;
			}
		}

			.planet {
			cursor: pointer;
		}
		.tooltip {
			position: absolute;
			background-color: #333;
			color: #fff;
			padding: 5px;
			border-radius: 5px;
		}





@keyframes moveText {
  0% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(400px);
  }
  100% {
    transform: translateX(0);
  }
}

@keyframes flash {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
    </style>
  </head>
  <body>
    <header>
      <div class="logo">
        <div class="logo-text-container">
          <div class="logo-text">Lofties</div>
        </div>
      </div>
      <div class="logo2">
        <div class="logo2-text-container">
          <div class="logo2-text">LoftiesWindows</div>
        </div>
        <div class="header-text">
          <div class="flash">LoftiesWindows</div>
          <p>See the world clearly, call us, we clean your windows!</p>
        </div>
      </div>
<div id="planet-system">
		<div class="sun"></div>
		<div class="planet mercury" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Mercury is the smallest planet in the solar system and is located closest to the Sun. It has a diameter of about 4,880 kilometers, which is roughly one-third the size of Earth. Despite its small size, Mercury is a dynamic and active planet with a surface that is heavily cratered, similar to that of our moon.

One day on Mercury lasts about 59 Earth days, while one year on Mercury is equivalent to just 88 Earth days. This means that Mercury has the shortest year of any planet in the solar system. Due to its proximity to the Sun, the temperatures on Mercury can reach extreme highs of up to 800 degrees Fahrenheit (430 degrees Celsius) during the day, while dropping to -290 degrees Fahrenheit (-180 degrees Celsius) at night.

Mercury has no known moons and no significant atmosphere, which means that its surface is constantly bombarded by meteoroids and solar radiation. Despite its proximity to the Sun, Mercury is not the hottest planet in the solar system, as its lack of atmosphere means that it cannot retain heat. Nevertheless, the planet's proximity to the Sun has made it a target for exploration, with several spacecraft visiting Mercury to study its surface, composition, and geology."></div>

	<div class="planet venus" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Venus is the second planet from the Sun and the brightest object in the night sky after the Moon. It has a thick atmosphere composed mostly of carbon dioxide, with clouds of sulfuric acid that create a dense, reflective layer that helps trap heat, making Venus the hottest planet in the solar system.

Venus is similar in size and composition to Earth, and is often referred to as Earth's twin. However, its extreme greenhouse effect and lack of magnetic field have led to a very different environment from our own. The surface of Venus is dry and barren, with a temperature hot enough to melt lead, and pressures that are 90 times greater than those on Earth.

Despite its inhospitable conditions, Venus has been the subject of many missions by space agencies around the world, including the Soviet Venera program and NASA's Mariner, Pioneer, and Magellan missions. These missions have provided valuable information about the planet's atmosphere, surface features, and geological history, and have helped scientists better understand the formation and evolution of rocky planets in our solar system."></div>
	<div class="planet earth" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Earth is the third planet from the Sun and is the only planet known to support life. It has a diameter of approximately 12,742 kilometers and a mass of about 5.97 x 10^24 kilograms. Earth has a complex system of geological activity, including tectonic plate movements, volcanoes, and earthquakes.

One of the most distinctive features of Earth is its atmosphere, which is composed of about 78% nitrogen, 21% oxygen, and small amounts of other gases, such as carbon dioxide and argon. The atmosphere plays a crucial role in regulating the planet's temperature and protecting it from harmful radiation.

Earth has one natural satellite, the Moon, which is about one-quarter the size of Earth. It takes about 27.3 days for the Moon to orbit the Earth. The planet is also home to a vast variety of living organisms, including humans, animals, and plants, and has a rich history of cultural and technological development."></div>
	<div class="planet mars" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Mars is the fourth planet from the Sun and is often referred to as the "Red Planet" because of its reddish appearance in the night sky. It is a rocky planet with a thin atmosphere composed mostly of carbon dioxide, and has the largest volcano in the solar system, Olympus Mons, and the deepest canyon, Valles Marineris.

Mars has a diameter of about 6,779 kilometers, roughly half the size of Earth, and a mass about one-tenth of Earth's. It has two small moons, Phobos and Deimos, which are thought to be captured asteroids. Mars is known for its striking geological features, including the polar ice caps, which are composed of frozen carbon dioxide and water.

Mars has been the focus of numerous robotic missions, including rovers and orbiters, seeking to study the planet's geology, climate, and potential for habitability. These missions have revealed evidence of past water on the planet, suggesting that Mars may have had a more hospitable environment in the past. Plans are also underway for future crewed missions to Mars, with the goal of establishing a permanent human presence on the planet in the coming decades."></div>
	<div class="planet jupiter" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Jupiter is the largest planet in the solar system and the fifth planet from the Sun. It is named after the Roman king of the gods and has been known since ancient times. Jupiter is a gas giant, composed mostly of hydrogen and helium, with small amounts of other elements.

Jupiter has the shortest day of any planet in the solar system, taking just under 10 hours to complete one rotation. It also has the strongest magnetic field of any planet, which creates intense radiation belts around the planet. Jupiter has a system of rings, although they are not as prominent as those of Saturn, and at least 79 known moons, the largest of which is Ganymede, the largest moon in the solar system.

Jupiter's atmosphere is known for its distinctive features, including its colorful bands of clouds and the Great Red Spot, a gigantic storm that has been raging for over 300 years. Jupiter also experiences frequent and intense storms, with lightning bolts that are up to 1,000 times more powerful than those on Earth. In 1995, the Galileo spacecraft arrived at Jupiter and provided valuable information about its atmosphere, moons, and magnetic field."></div>
	<div class="planet saturn" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Saturn is the sixth planet from the Sun and is known for its spectacular system of rings, which are made up of billions of ice particles ranging in size from tiny grains to boulders several meters across. It takes about 29 Earth years for Saturn to complete one orbit around the Sun.

Saturn is the second-largest planet in the solar system, with a diameter of about 116,460 kilometers and a mass roughly 95 times that of Earth. Like Jupiter, it is classified as a gas giant, composed mostly of hydrogen and helium, with small amounts of other elements.

Saturn rotates quickly, taking about 10.7 hours to complete one rotation. Its rotational axis is tilted at an angle of 26.73 degrees, which is similar to Earth's tilt. Saturn also has at least 82 known moons and a complex system of rings that extend out more than 280,000 kilometers from the planet's center."></div>
        <div class="planet uranus" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Uranus is the seventh planet from the Sun and takes about 84 Earth years to complete one orbit around it. It was discovered by William Herschel in 1781 and is unique in the solar system for its extreme tilt. Its rotational axis is tilted at an angle of 97.77 degrees, which means that it essentially rolls around the Sun on its side.

Uranus is also known for its pale blue-green color, which comes from the methane in its atmosphere. It has a diameter of about 50,724 kilometers and a mass roughly 14.5 times that of Earth. Like Jupiter and Saturn, Uranus is classified as a gas giant, composed mostly of hydrogen and helium, with small amounts of other elements.

Uranus has 27 known moons and a system of rings, although they are not as visible or prominent as those of Saturn. Uranus rotates slowly, taking about 17.2 hours to complete one rotation. Its magnetic field is also unique, being tilted at an angle of about 60 degrees to its rotational axis. Uranus has been visited by only one spacecraft, Voyager 2, which flew by the planet in 1986 and provided valuable information about its atmosphere, moons, and rings.

        <div class="planet neptune" title="Don't move the cursor or the info will go,Stay still and read, let your knowledge grow:Neptune is the eighth planet from the Sun and takes about 165 Earth years to complete one orbit around it. It was discovered in 1846 by astronomers John Couch Adams and Urbain Le Verrier based on mathematical predictions. Neptune is a gas giant, like Jupiter, Saturn, and Uranus, and has a diameter of about 49,244 kilometers, making it the fourth-largest planet in the solar system.

Neptune is known for its beautiful blue color, which comes from the methane in its atmosphere. It has a mass roughly 17 times that of Earth and is composed mostly of hydrogen and helium, with small amounts of other elements. Neptune has 14 known moons and a system of rings, although they are not as prominent as those of Saturn.

Neptune's rotational axis is tilted at an angle of about 28 degrees, which is similar to Earth's. It rotates quickly, taking about 16 hours to complete one rotation. Its magnetic field is also unique, being tilted at an angle of about 47 degrees to its rotational axis. Neptune has been visited by only one spacecraft, Voyager 2, which flew by the planet in 1989 and provided valuable information about its atmosphere, moons, and rings."></div>
</div><script>
// add event listeners to planets to display title on hover
const planets = document.querySelectorAll('.planet');
planets.forEach(planet => {
planet.addEventListener('mouseover', () => {
const title = planet.getAttribute('title');
const tooltip = document.createElement('div');
tooltip.classList.add('tooltip');
tooltip.textContent = title;
document.body.appendChild(tooltip);
});
planet.addEventListener('mousemove', (event) => {
const tooltip = document.querySelector('.tooltip');
tooltip.style.top = event.pageY - 10 + 'px';
tooltip.style.left = event.pageX + 10 + 'px';
});
planet.addEventListener('mouseout', () => {
const tooltip = document.querySelector('.tooltip');
document.body.removeChild(tooltip);
});
});
</script>
    </header>
    <main>
      <section>
        <p>...........</p>
      </section>
    </main>
  </body>
</html>

