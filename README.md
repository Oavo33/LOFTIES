<!DOCTYPE html>
<html>
<head>
  <title>Star Tunnel Background</title>
  <style>
    canvas { position: fixed; z-index: -1; background: black; }
  </style>
</head>
<body>
  <canvas id="canvas"></canvas>
  <script>
    var canvas = document.getElementById('canvas');
    var ctx = canvas.getContext('2d');
    var width = window.innerWidth;
    var height = window.innerHeight;
    var stars = [];
    var speed = 0.1;
    var maxSpeed = 5;
    var starFrequency = 100;
canvas.width = width;
    canvas.height = height;
function Star() {
      this.x = Math.random() * width;
      this.y = Math.random() * height;
      this.radius = Math.random() * 1.2;
      this.color = '#fff';
      this.speed = (Math.random() * (maxSpeed - speed) + speed);
    }
for (var i = 0; i < 10; i++) {
      stars.push(new Star());
    }
function drawStars() {
      for (var i = 0; i < stars.length; i++) {
        var star = stars[i];
        star.x += (width / 2 - star.x) * (star.speed / -1000);
        star.y += (height / 2 - star.y) * (star.speed / -1000);
        if (star.x < 0 || star.x > width || star.y < 0 || star.y > height) {
          stars[i] = new Star();
        }
        ctx.beginPath();
        ctx.fillStyle = star.color;
        ctx.arc(star.x, star.y, star.radius, 0, Math.PI * 2);
        ctx.fill();
      }
    }function addStar() {
      stars.push(new Star());
    }
setInterval(addStar, starFrequency);
function animate() {
      ctx.clearRect(0, 0, width, height);
      drawStars();
      requestAnimationFrame(animate);
    }

    animate();
  </script>
</body>
</html>

