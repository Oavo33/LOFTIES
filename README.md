 <!DOCTYPE html>
<html>
  <head>
    <title>Lofties Windows</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
      /* Global styles */
      :root {
        --primary-color: #214E34;
        --secondary-color: #F7D6BF;
        --tertiary-color: #F8EEE7;
        --accent-color: #FF7F11;
        --font-family: Arial, sans-serif;
      }

      * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
      }

      /* Typography */
      body {
        font-family: var(--font-family);
        font-size: 16px;
        line-height: 1.5;
        color: var(--primary-color);
        background-color: var(--tertiary-color);
      }

      h1, h2, h3 {
        font-family: var(--font-family);
        font-weight: bold;
        color: var(--primary-color);
        margin-bottom: 20px;
      }

      h1 {
        font-size: 48px;
        text-align: center;
        margin-top: 30px;
      }

      h2 {
        font-size: 36px;
      }

      h3 {
        font-size: 24px;
        margin-top: 30px;
      }

      p, ul, li {
        font-family: var(--font-family);
        font-size: 16px;
        line-height: 1.5;
        color: var(--primary-color);
      }

      /* Layout */
      header {
        background-color: var(--primary-color);
        color: var(--secondary-color);
        text-align: center;
        padding: 20px;
        box-shadow: 0px 0px 10px #888888;
      }

      nav {
        background-color: var(--secondary-color);
        padding: 10px;
        display: flex;
        justify-content: center;
      }

      nav ul {
        list-style: none;
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 800px;
        width: 100%;
        margin: 0 auto;
      }

      nav li {
        margin: 0 10px;
      }

      article {
        background-color: var(--secondary-color);
        padding: 40px;
        margin-top: 20px;
        border-radius: 10px;
        box-shadow: 0px 0px 10px #888888;
      }

      ul {
        margin-left: 20px;
        margin-bottom: 20px;
      }

      li {
        margin-bottom: 10px;
      }

      footer {
        background-color: var(--primary-color);
        color: var(--secondary-color);
        text-align: center;
        padding: 20px;
        box-shadow: 0px 0px 10px #888888;
      }

      .social-media {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 20px;
      }  .social-media a {
    color: var(--secondary-color);
    font-size: 20px;
    margin: 0 10px;
  }

  .social-media a:hover {
    color: var(--accent-color);
  }

  /* Responsive */
  @media only screen and (max-width: 768px) {
    h1 {
      font-size: 36px;
    }

    h2 {
      font-size: 28px;
    }

    h3 {
      font-size: 20px;
    }

    article {
      padding: 20px;
    }

    nav ul {
      flex-direction: column;
    }

    nav li {
      margin: 10px 0;
    }
  }
</style></head>
  <body>
    <header>
      <h1>Lofties Windows</h1>
    </header><nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Products</a></li>
    <li><a href="#">About Us</a></li>
    <li><a href="#">Contact Us</a></li>
  </ul>
</nav>

<article>
  <h2>Welcome to Lofties Windows</h2>

  <p>stylish.</p>

  <h3>Our Products</h3>

  <ul>
    <li>Double-Hung Windows</li>
    <li>Sliding Windows</li>
    <li>Casement Windows</li>
    <li>Bay Windows</li>
    <li>Bow Windows</li>
  </ul>

  <p>99666.</p>

  <div class="social-media">
    <a href="#"><i class="fab fa-facebook-square"></i></a>
    <a href="#"><i class="fab fa-twitter-square"></i></a>
    <a href="#"><i class="fab fa-instagram-square"></i></a>
  </div>
</article>

<footer>
  <p>&copy; 2023 Lofties Windows. All rights reserved.</p>
</footer>
  </body>
</html>

