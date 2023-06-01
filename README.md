<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Hub</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Your-Graffiti-Font&display=swap');
    body {
      font-family: 'Space Mono', monospace;
      font-size: 14px;
      background-color: #f2f2f2;
      color: #333333;
    }
    .header {
      background: linear-gradient(to bottom, #00b3b3, #008080);
      padding: 20px;
      text-align: center;
      position: relative;
    }
    .header h1 {
      font-size: 45px;
      color: #ffffff;
      margin: 0;
    }.social {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
    }
    .social div {
      margin-bottom: 5px;
    }
    .social div a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: black;
    }
    .social div a img {
      width: 15px;
      height: 15px;
    }
    .hub-card {
      background: linear-gradient(to bottom, #008080, #00b3b3);
      border-radius: 10px;
      border: 2px solid #ffffff;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
      padding: 20px;
      text-align: center;
      max-width: 500px;
      width: 70%;
      margin: 0 auto;
      margin-top: -93px;
      position: relative;
      z-index: 2;
    }
    .hub-card h1 {
      font-size: 18px;
      margin-top: 0px;
      margin-bottom: 0px;
      color: #ffffff;
    }
    .hub-card p {
      font-size: 12px;
      margin-bottom: 10px;
      color: #ffffff;
    }
    .dropdown-container {
      text-align: center;
      margin-top: 20px;
    }
    .dropdown {
      display: inline-block;
      position: relative;
    }
    .dropdown select {
      font-family: 'Space Mono', monospace;
      font-size: 14px;
      padding: 5px 10px;
      border-radius: 5px;
      border: 2px solid #ffffff;
      background-color: #008080;
      color: #ffffff;
      appearance: none;
      outline: none;
    }
    .dropdown::after {
      content: '\25BC';
      position: absolute;
      top: 50%;
      right: 10px;
      transform: translateY(-50%);
      font-size: 10px;
      color: #ffffff;
    }
    .graffiti-left,
    .graffiti-right {
  position: absolute;
  top: 50%;
  left: 50%; /* Add this line to center horizontally */
  transform: translate(-50%, -50%); /* Add this line to center vertically and horizontally */
  font-family: 'Your-Graffiti-Font', cursive;
  font-size: 10px;
  color: #00b3b3;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  z-index: 1;
}
.graffiti-left {
      left: 0px;
      transform: rotate(-7deg);
      top: 80%
      }
      .graffiti-right {
      right: -35px;
      transform: rotate(7deg);
      top: 80%
    }
  </style>
</head>
<body>
  <div class="header">
    <div class="login-register">
      <a href="#">Login</a>
      <a href="#">Register</a>
    </div><div class="graffiti-left">This is your Hub !<br> Want to change it ?<br>Submit Request <br>Here</div>
    <div class="graffiti-right">This whole Hub<br> Has been organized by <br>Local Small Business<br>And You ,We Need You !</div>
    <h1>Collabor8</h1>
    <div class="social">
      <div>
        <a href="#">
          <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
        </a>
      </div>
      <div>
        <a href="#">
          <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
        </a>
      </div>
      <div>
        <a href="#">
          <img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram">
        </a>
      </div>
      <div>
        <a href="#">
          <img src="https://img.icons8.com/office/30/FF0000/twitter.png" alt="Twitter">
        </a>
      </div>
    </div>
  </div>
  <div class="hub-card"><div class="dropdown-container">
    <div class="dropdown"><h1>60% Community + 40% Local Business = Success</h1>
    <p>Hiyas, welcome to Collabor8! Think of us as your friendly neighborhood hub.</p>
  </div>
  <select>
        <option value="">Select a Local business</option>
        <option value="astronaut">Chippy</option>
        <option value="engineer">Window Cleaner</option>
        <option value="scientist">Hairdresser</option>
        <option value="pilot">RocketShip Parts</option>
      </select>
    </div>
  </div></body>
</html>
