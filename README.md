<!DOCTYPE html>
<html>

<head>
  <title>My Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
  <style>
    header {
      background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
      background-size: cover;
      background-position: center;
      color: #00B3B3;
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

</html>
