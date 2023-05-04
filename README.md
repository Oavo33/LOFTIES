<html lang="en"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Lofties Windows</title>
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Alex+Brush&display=swap" rel="stylesheet">
    <style>
      body {
        font-family: 'Pacifico', cursive;
        background-color: #333333;
        color: #f2f2f2;
      }
      header {
    font-family: 'Pacifico', cursive;
    background-color: #800000;
    background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
    background-size: 100%;
    background-position: center 65%;
    color: #00b3b3;
    padding: 70px;
    position: relative;
    text-align: center;
    text-shadow: 2px 2px #800000;
  }
.logo {
    position: absolute;
    bottom: 40;
    left: 20;
    margin: 0;
    display: flex;
    align-items: center;
  }.cube-container {
  position: absolute;
  width: 100px;
  height: 100px;
  top: 60%;
  left: -5%;
  transform: scale(0.1);
}
.cube {
    position: absolute;
    width: 140px;
    height: 140px;
    transform-style: preserve-3d;
    animation: rotate 10s infinite linear;
    cursor: pointer;
    animation-name: spin;
    animation-duration: 34s;
    animation-iteration-count: infinite;
    animation-timing-function: linear;
  }
.cube:hover {
    animation: spin-slow 20s infinite linear;
  }
.cube .side {
    position: absolute;
    width: 140px;
    height: 140px;
    background-color: #00B3B3;
    border: 2px solid #800000;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 50px;
    font-weight: bold;
    color: #800000;
    text-transform: uppercase;
    transform-style: preserve-3d;
    text-align: center;
    writing-mode: horizontal-tb;
  }
.cube .front {
  transform: rotateY(0deg) translateZ(100px);
}
.cube .back {
  transform: rotateY(180deg) translateZ(100px);
}
.cube .right {
  transform: rotateY(-90deg) translateZ(100px);
}
.cube .left {
  transform: rotateY(90deg) translateZ(100px);
}
.cube .top {
  transform: rotateX(90deg) translateZ(100px);
}
.cube .bottom {
  transform: rotateX(-90deg) translateZ(100px);
}
@keyframes rotate {
  from {
    transform: rotateY(0deg);
  }
  to {
    transform: rotateY(360deg);
  }}
@keyframes spin {
  from {
    transform: rotateX(0deg) rotateY(0deg);
  }
  to {
    transform: rotateX(360deg) rotateY(360deg);
  }}
@keyframes spin-slow {
  from {
    transform: rotateX(0deg) rotateY(0deg);
  }
  to {
    transform: rotateX(360deg) rotateY(360deg);
  }
}
.cube .front:hover::before,
.cube .back:hover::before,
.cube .right:hover::before,
.cube .left:hover::before,
.cube .top:hover::before,
.cube .bottom:hover::before {
  content: "LoftiesWindows";
  position: absolute;
  top: -40px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 20px;
  font-weight: bold;
  color: #fff;
  text-transform: uppercase;
  text-align: center;
  writing-mode: horizontal-tb;
}</style>
  </head>
  <body>
    <header>
     <h1>Your Brand Name</h1>
      </div><div class="cube-container">
    <div class="cube">
      <div class="side front">Lofties</div>
      <div class="side back">Lofties</div>
      <div class="side right">Lofties</div>
      <div class="side left">Lofties</div>
      <div class="side top">Lofties</div>
      <div class="side bottom">Lofties</div>
    </div>
  </div></header>
    <main>
      <section>
        <p>...........</p>
      </section>
    </main>
  </body>
</html>
