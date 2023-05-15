<!DOCTYPE html>
<html>
<head>
  <title>User Login/Registration</title>
  <style>
    body {
      margin: 0;
      padding: 0;
    }
    .header-form {
      display: flex;
      align-items: flex-start;
      justify-content: flex-end;
      height: 60px;
      padding: 5px;
      box-sizing: border-box;
    }
input[type="text"],
    input[type="password"] {
      width: 50px;
      padding: 2px;
      margin-right: 2px;
      border-radius: 4px;
      background-color: #333;
      color: #fff;
      font-family: Arial, sans-serif;
      border: 1px dashed #800000;
      font-size: 10px;
    } 
    input[type="text"]:focus,
    input[type="password"]:focus {
      box-shadow: 0 0 3px #00b3b3;
      border: 1px dashed #800000;
    }
    .button {
      padding: 2px 4px;
      color: #fff;
      border: 1px double #800000;
      border-radius: 12px;cursor: pointer;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #800000, #00b3b3);
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.2);
      position: relative;
      font-size: 10px;
    }
.button:hover {
      transform: scale(1.05);
    }
.button::before {
      content: "Scrub away your worries and find the perfect squeegee for a crystal-clear view!";
      position: absolute;
      top: 18px;
      left: 50%;
      transform: translateX(-95%);
      background-color: #333;
      color: #fff;
      padding: 0px;
      border-radius: 4px;
      visibility: hidden;
      opacity: 0;
      transition: visibility 0s, opacity 0.5s linear;
      font-size: 10px;
      line-height: 1.2;
      white-space: nowrap;
      border: 1px dashed #800000;
    }
.button:hover::before {
      visibility: visible;
      opacity: 1;}
  </style>
</head>
<body>
  <div class="header-form">
    <input type="text" id="username" placeholder="Username" required>
    <input type="password" id="password" placeholder="Password" required>
    <button type="submit" id="login-button" class="button">Login</button>
    <button id="register-button" class="button">Register</button>
  </div>
<script>
    // Simulating user login functionality
    document.getElementById("login-button").addEventListener("click", function() {
      var username = document.getElementById("username").value;
      var password = document.getElementById("password").value;
      // Perform login authentication logic here
      if (username === "admin" && password === "password") {
        alert("Login successful!");
        // Redirect to user dashboard or personalized page
      } else {
        alert("Invalid username or password. Please try again.");
      }
    });
// Redirect to sign up page
    document.getElementById("register-button").addEventListener("click", function() {
      window.location.href = "signup.html"; // Replace with your sign up page URL
    });</script>
</body>
</html>
