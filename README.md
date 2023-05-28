<html><head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lofties Astronauts</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');
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
    }
    .login-register {
      display: flex;
      justify-content: end;
    }
    .login-register a {
      margin-left: 10px;
      text-decoration: none;
      color: white;
      padding: 2px 5px;
      font-size: 0.8em;
      border-radius: 15px;
      background: linear-gradient(90deg, #ffffff, #00b3b3);
      transition: background .3s;
    }
    .login-register a:hover {
      background: linear-gradient(90deg, #00b3b3, #ffffff);
    }
    .header h1 {
      font-size: 45px;
      color: #ffffff;
      margin: 0;
    }
    .header p {
      font-size: 12px;
      color: #ffffff;
    }
    .social {
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
      margin-top: -73px;
      position: relative;
      z-index: 1;
    }
    .hub-card h1 {
      font-size: 18px;
      margin-top: 0;
      margin-bottom: 10px;
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
    .container {
      position: relative;
      width: 150px;
      height: 200px;
      margin: 20px auto;
    }
    .triangle {
      position: absolute;
      top: 50%;
      left: 40.5%;
      transform: translate(-50%, -50%);
      width: 0;
      height: 0;
      border-left: 30px solid transparent;
      border-right: 30px solid transparent;
      border-bottom: 60px solid #00b3b3;
      transition: all 1s ease;
    }
    #left-triangle {
      top: calc(50% - 30px);
      left: calc(50% - 60px);
      border-bottom-color: #008c8c;
    }
    #right-triangle {
      top: calc(50% + 30px);
      left: calc(50% - 60px);
      border-bottom-color: #00a6a6;
    }
    #center-triangle:hover {
      transform: translate(-50%, -50%) rotate(180deg) translateY(5px);
    }
    #center-triangle:hover ~ #left-triangle {
      transform: translate(-50%, -50%) translateX(46px) translateY(2px);
    }
    #center-triangle:hover ~ #right-triangle {
      transform: translate(-50%, -50%) translateX(46px) translateY(-58px);
    }
    .reflect-text {
      position: absolute;
      top: 49%;
      left: 60%;
      transform: translate(-50%, -50%) rotate(65deg);
      font-size: 13px;
      font-weight: bold;
      color: transparent;
      background: linear-gradient(45deg, red, orange, yellow, green, blue, indigo, violet, red);
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      transition: all 1s ease;
      z-index: 2;
    }
    .reflection {
      position: absolute;
      top: 70%;
      left: 43%;
      transform: translate(-50%, -50%) rotate(0.1deg);
      font-size: 13px;
      font-weight: bold;
      color: transparent;
      background: linear-gradient(45deg, red, orange, yellow, green, blue, indigo, violet, red);
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      transition: all 1s ease;
      z-index: 2;
    }
    #center-triangle:hover ~ .reflect-container .reflect-text {
      transform: translate(-50%, -50%) translateX(-25px) translateY(-45px) rotate(0.1deg);
    }
    #center-triangle:hover ~ .reflect-container .reflection {
      transform: translate(-50%, -50%) translateX(-2px) translateY(-28px);
    }
    .reflect-container:hover .reflection {
      opacity: 0.8;
    }
    .community-container {
      color: #00b3b3;
      text-align: center;
      position: relative;
      margin-bottom: 100px;
    }
    .community-heading,
    .community-description,
    .community-benefits,
    .community-cta,
    .community-benefits-list {
      color: #00b3b3;
      text-align: center;
    }
    .community-heading {
      font-size: 18px;
      margin-top: 20px;
    }
    .community-description {
      font-size: 14px;
      margin-bottom: 10px;
    }
    .community-benefits {
      font-size: 14px;
      font-weight: bold;
    }
    .community-benefits-list {
      margin-top: 5px;
      list-style-type: disc;
      margin-left: 15px;
      font-size: 17px;
    }
    .community-cta {
      font-style: italic;
      margin-top: 10px;
      font-size: 17px;
    }
    .grid-container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-gap: 20px;
      background: linear-gradient(to bottom, #00b3b3, #ffffff);
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
      padding: 15px;
      justify-items: center;
    }
    .grid-item {
      background-color: #00b3b3;
      color: #ffffff;
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2), 0 6px 6px rgba(0, 0, 0, 0.2);
      padding: 10px;
      text-align: center;
      position: relative;
      overflow: hidden;
      transition: transform 0.3s, box-shadow 0.3s;
      cursor: pointer;
      width: 100%;
    }
    .grid-item:hover {
      transform: translateY(-3px);
      box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3), 0 8px 8px rgba(0, 0, 0, 0.3);
    }
    footer {
      background: linear-gradient(to bottom, #ffffff, #00b3b3);
      padding: 15px;
      color: #ffffff;
      text-align: center;
      font-size: 14px;
    }
    .footer-container {
      max-width: 1200px;
      margin: 0 auto;
    }
  </style>
</head>
<body>
  <div class="header"><div class="login-register">
      <a href="#">Login</a>
      <a href="#">Register</a>
    </div>
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
  </div><div class="hub-card">
    <h1>Driving Growth Together: Empowering Businesses and Communities</h1>
    <p>Welcome to Collabor8, a community-driven hub that empowers businesses and fosters collaboration. Join us to unlock boundless growth opportunities and forge meaningful connections. With a focus on community involvement, we prioritize the 60/40 rule, giving the community a significant say in shaping the hub. Together, we challenge corporate dominance and redirect support towards local enterprises. Experience personalized exchanges, community services, and unique features like the engaging graffiti wall. Be part of our vibrant ecosystem, where businesses and communities thrive. Discover, connect, and create unforgettable experiences at Collabor8!</p><div class="dropdown-container">
    <div class="dropdown">
      <select>
        <option value="">Select a Local business</option>
        <option value="astronaut">Chippy</option>
        <option value="engineer">Window Cleaner</option>
        <option value="scientist">Hairdresser</option>
        <option value="pilot">RocketShip Parts</option>
      </select>
    </div>
  </div>
</div>
  <div class="container">
    <div id="center-triangle" class="triangle"></div>
    <div id="left-triangle" class="triangle"></div>
    <div id="right-triangle" class="triangle"></div>
    <div class="reflect-container">
      <div class="reflect-text">H<span>u</span><span>n</span><span>g</span><span>r</span><span>y</span><span>s</span></div>
      <div class="reflection">H<span>u</span><span>n</span><span>g</span><span>r</span><span>y</span><span>s</span></div>
    </div>
  </div>
  <h2 class="community-heading">Join Our Community</h2>
  <p class="community-description">
    Our mission is to establish a community-run hub that brings together the community and local businesses, with a strong focus on community involvement. We prioritize community empowerment through a 60/40 split, emphasizing community interests over business interests.
    
    The community holds a 60% say in determining the content and visual aspects of our hub. Whether it's choosing design elements, incorporating community-uploaded hand-drawn artwork, or selecting colors and bubbles, we value the community's vision. By actively involving both the community and small businesses, we aim to challenge corporate dominance and redirect support towards local enterprises. Over three years of collaboration, we envision an incredible hub created by the community.
    At the end of each year, the community will receive 60% of the profits generated by the hub. Together, we will identify areas for improvement and decide how to allocate funds for community projects. Our belief is that economic empowerment of the community leads to positive change. Rather than pursuing personal enrichment, our goal is to foster a strong sense of community spirit, drawing inspiration from the founder's upbringing in a council estate.
  </p>
  <p class="community-benefits">Benefits of joining our community:</p>
  <ul class="community-benefits-list">
    <li>Elderly Assistance: We approach elderly assistance with caution, gathering insights from local churches, elderly charities, and the wider community. Our goal is to provide targeted support, considering the unique needs of our senior community members. We are determined to make a positive impact while prioritizing their input.</li>
    <li>Personalized Exchange and Free Services: Unlike other platforms that offer unrealistic giveaways, we provide a more personalized service. Our window cleaner not only scans customers' backyards for unwanted items but also facilitates exchanges within the community. Additionally, we encourage builders to contribute to the hub by offering free services. This ensures that the community benefits from trustworthy assistance, alleviating concerns about previous negative experiences.</li>
    <li>Community Service: Community service is a collective effort involving our founder, their children, loyal customers, and anyone interested in making a difference. As we document and share pictures of these initiatives on the hub, we aim to inspire others to join in and foster a positive trend within our area.</li>
    <li>Personalized Web Pages: As a unique and innovative offering, we provide a full web page for lucky community members to commemorate important events in their lives. Whether it's celebrating a birth, wedding, or creating a memorial for a lost loved one, these individuals will have full responsibility for the page. We provide them with the password and login details, allowing them to curate the content within limits set by our platform.</li>
    <li>The Engaging Graffiti Wall: We introduce an interactive feature called the "graffiti wall." Community members can submit their chosen nicknames, which we proudly display on this wall. This idea, developed for the community, promotes engagement and allows individuals of all ages to have their names forever associated with our hub.</li>
    <li>Encouraging Young Entrepreneurship: Every year, we invite three young individuals from the community, regardless of age, to submit their business plans. As long as their proposals demonstrate clear direction and comply with legal requirements, we offer them the opportunity to start a business with full autonomy. They can invest in any legal stock or materials without requiring adult assistance. Take, for example, the story of a 12-year-old kid who wrote to an Australian scooter company and asked if he could sell their scooters in England. The Australian company agreed, and that 12-year-old kid has now made millions by moving stocks from A to B. It's a true story—Google it! We aim to inspire and support the entrepreneurial aspirations of our young community members, encouraging them to save pocket money and pursue their dreams.</li>
    <li>Monthly Prizes: We are considering implementing monthly prizes to further engage the community. While the details are still under consideration, our initial thoughts include hiding symbolic items like menus, scissors, or lucky chips on respective hub pages. However, we are mindful of ensuring that these items remain accessible within the hub and not taken away so we still need your feed back on this please.</li>
  </ul>
  <p class="community-cta">Don't miss out on the incredible opportunities awaiting you! As your hub grows, so does everything else related—helping more people, improvement to your area, better prizes, and more web pages developed. Instead of one every three months, it could be one every week! Instead of three entrepreneurs a year, we have 30 entrepreneurs a year. Imagine the possibilities! With 60% of profits going to the community, we can easily achieve this together. At Collabor8, we already have a team of 15 local people like you who want to make a change for the better after such a hard few years. Let's get our community back! Join our hub today and embark on a journey filled with discovery, connections, and memorable experiences.

Hopefully, you might be thinking, "Well, what can I do?" You can leave a review and tell us how you want the hub to look. Help us find a sufficient and effective way to assist the elderly. Make an application for the Graffiti wall or Web Page Design,  Visit the site daily to get the most recent updates. Send in a picture of an unwanted item. Join us in litter picking. And let's get the little ones started on their business plans as we enter prosperity.</p>
  <div class="grid-container community-container">
    <div class="grid-item community-item">
      <i class="community-icon">🏠</i>
      <p class="community-text">Community Exchange</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">🌞</i>
      <p class="community-text">Elderly Assistance</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">🌍</i>
      <p class="community-text">Community Service</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">🎉</i>
      <p class="community-text">Free Services</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">🏰</i>
      <p class="community-text">Encouraging Young Entrepreneurship</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">🎨</i>
      <p class="community-text">The Engaging Graffiti Wall</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">📢</i>
      <p class="community-text">Personalized Web Pages</p>
    </div>
    <div class="grid-item community-item">
      <i class="community-icon">🎁</i>
      <p class="community-text">Monthly Prizes</p>
    </div>
  </div><h3>Graffiti wall</h3>
  <footer>
    <div class="footer-container">
      <p>&copy; 2023 Lofties. All rights reserved.</p>
    </div>
  </footer>
  <script>
    const centerTriangle = document.getElementById('center-triangle');
    const leftTriangle = document.getElementById('left-triangle');
    const rightTriangle = document.getElementById('right-triangle');
    centerTriangle.addEventListener('mouseover', handleTriangleHover);
    centerTriangle.addEventListener('touchstart', handleTriangleHover);
    centerTriangle.addEventListener('mouseout', handleTriangleHover);
    centerTriangle.addEventListener('touchend', handleTriangleHover);
    function handleTriangleHover(event) {
      if (event.type === 'mouseover' || event.type === 'touchstart') {
        leftTriangle.style.transform = 'translate(-50%, -50%) translateX(46px) translateY(2px)';
        rightTriangle.style.transform = 'translate(-50%, -50%) translateX(46px) translateY(-58px)';
      } else if (event.type === 'mouseout' || event.type === 'touchend') {
        leftTriangle.style.transform = 'translate(-50%, -50%)';
        rightTriangle.style.transform = 'translate(-50%, -50%)';
      }
    }
  </script>
</body>
</html>
