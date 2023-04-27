<!DOCTYPE html>
<html>
<head>
  <title>Modern Sleek Look</title>
  <style>
    body {
      font-family: 'Roboto', sans-serif;
      background-color: #f2f2f2;
      color: #333;
      margin: 0;
    }
    header {
      background-color: #5bc0de;
      color: #fff;
      text-align: center;
      padding: 1rem;
      font-size: 2rem;
      letter-spacing: 2px;
      text-transform: uppercase;
      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
    }
    nav {
      background-color: #5bc0de;
      padding: 0.5rem;
      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
    }
    nav ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      overflow: hidden;
      text-align: center;
    }
    nav li {
      display: inline-block;
    }
    nav li a {
      display: block;
      color: #fff;
      text-align: center;
      padding: 0.5rem;
      text-decoration: none;
      font-weight: bold;
      font-size: 1.2rem;
      letter-spacing: 1px;
      text-transform: uppercase;
      transition: all 0.2s ease-in-out;
    }
    nav li a:hover {
      background-color: #fff;
      color: #5bc0de;
    }
    section {
      padding: 2rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
    }
    .card {
      width: 300px;
      margin: 1rem;
      padding: 1rem;
      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
      border-radius: 10px;
      background-color: #fff;
      transition: all 0.2s ease-in-out;
    }
    .card:hover {
      box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.3);
      transform: translateY(-5px);
    }
    .card img {
      width: 100%;
      border-radius: 10px;
    }
    .card h3 {
      margin-top: 1rem;
      font-size: 1.5rem;
      text-align: center;
      color: #333;
      letter-spacing: 1px;
    }
    footer {
      background-color: #88292f;
      color: #fff;
      text-align: center;
      padding: 1rem;
      font-size: 1.2rem;
      letter-spacing: 1px;
      text-transform: uppercase;
      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
    }
    .social-media {
      display: flex;
      justify-content: center;
      margin-top: 1rem;
    }
    .social-media a {
      display: inline-block;
      margin-right: 1rem;
      color: #fff;
      font-size: 1.5rem;
      transition: all 0.2s ease-in}
.social-media a:hover {
  color: #5bc0de;
}
/* update to light shade of bright blue and a cool shade of dark maroon */
header,
nav {
  background-color: #66b3ff;
}
nav li a:hover {
  background-color: #88292f;
  color: #fff;
}
footer {
  background-color: #660000;
}
 </style>
</head>
<body>
  <header>
    <h1>Modern Sleek Look</h1>
  </header>
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
  <section>
    <div class="card">
      <img src="https://picsum.photos/id/237/300/200" alt="Random Image">
      <h3>Card 1</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi error recusandae voluptas adipisci quas dolorem asperiores tempora eum quod maiores?</p>
    </div>
    <div class="card">
      <img src="https://picsum.photos/id/238/300/200" alt="Random Image">
      <h3>Card 2</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi error recusandae voluptas adipisci quas dolorem asperiores tempora eum quod maiores?</p>
    </div>
    <div class="card">
      <img src="https://picsum.photos/id/239/300/200" alt="Random Image">
      <h3>Card 3</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi error recusandae voluptas adipisci quas dolorem asperiores tempora eum quod maiores?</p>
    </div>
  </section>
  <footer>
    <p>&copy; 2023 Modern Sleek Look</p>
    <div class="social-media">
      <a href="#"><i class="fab fa-facebook"></i></a>
      <a href="#"><i class="fab fa-twitter"></i></a>
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-linkedin"></i></a>
    </div>
  </footer>
</body>
</html>
