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
      color: #fff;
      font-family: 'Pacifico', cursive;
      padding: 200px;
      text-shadow: 2px 2px #000;
      position: relative;
    }.logo {
  position: absolute;
  bottom: 0;
  left: 0;
  font-size: 40px;
  margin: 0;
}.logo-text {
  position: absolute;
  top: 30px;
  right: 30px;
  font-size: 30px;
  margin: 20px;
  text-shadow: 2px 2px #000;
}.logo:after {
  content: "LOFTIES";
  display: inline-block;
  height: 20px;
  width: 20px;
  border-top: 30px solid #800000;
  border-right: 30px solid transparent;
  transform: rotate(0deg);
  margin-left: 18px;
  color: #800000;
  font-family: 'Montserrat', sans-serif;
  font-size: 20px;
  line-height: 20px; /* Adjust this value */
  text-align: center;
}.logo:hover:after {
  border-top: 50px solid #00B3B3;
}
</style>
</head>
<body>
  <header>
    <div class="logo"></div>
    <div class="logo-text">windowcleaner</div>
  </header>
</body>
</html>
