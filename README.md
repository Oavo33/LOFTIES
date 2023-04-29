<!DOCTYPE html>
<html>
  <head>
    <title>My Website</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <style>
      body {
        background-color: #800000;
        font-family: 'Pacifico', cursive;
        margin: 0;
      }

      header {
        background-image: url('https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80');
        background-size: cover;
        background-position: center;
        color: rgb(126, 126, 126);
        text-align: right;
        padding: 20vw;
        display: flex;
        justify-content: center;
        align-items: flex-end;
        position: relative;
        z-index: 1
      }


  

      .triangle {
        width: 20vw;
        height: 20vw;
        background-color: #800000;
        position: absolute;
        bottom: 0;
        right: 0;
        transform: translate(20%, 20%);
        clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
        display: flex;
        justify-content: center;
        align-items: center;
        z-index: 2;
      }
      .triangle::before {
        content: "";
        width: 0;
        height: 0;
        position: absolute;
        top: -40vw;
        left: -20vw;
        border-top: 60vw solid #800000;
        border-right: 20vw solid transparent;
        z-index: -1;
        transform: rotate(60deg);
      }

      .triangle::after {
        content: "";
        width: 0;
        height: 0;
        position: absolute;
        top: -40vw;
        right: -20vw;
        border-top: 60vw solid #800000;
        border-left: 20vw solid transparent;
        z-index: -1;
        transform: rotate(-60deg);
      }

 h1 {
        font-size: 8vw;
        text-align: center;
        margin: 0;
        padding: 0;
        line-height: 1;
        text-shadow: 2px 2px #800000;
        position: absolute;
        transform: translate(-50%, -50%);
        top: 20%;
        left: 50%;
        z-index: 1;
        background: linear-gradient(to right, black,white);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        animation: fade 3s ease-in-out infinite alternate;
      }

      @keyframes fade {
        from {
          opacity: 0.5;
        }
        
        to {
          opacity: 1;
        }
      }

    h1.title {
  font-size: 7vw;
  line-height: 1.5;
  margin: 0;
  padding: 0;
  text-shadow: 2px 2px #1C1C1C;
}

      @media only screen and (max-widthand) (max-width: 768px) {
header {
text-align: center;
padding: 10vw;
}    h1.title {
      font-size: 10vw;
    }

    .triangle {
      width: 40vw;
      height: 40vw;
      bottom: -20vw;
    }

    .triangle::before {
      top: -80vw;
      left: -40vw;
      border-top: 120vw solid #800000;
    }

    .triangle::after {
      top: -80vw;
      right: -40vw;
      border-top: 120vw solid #800000;
    }
  }
</style>
</head>
  <body>
    <header>
      <h1>LoftiesWindows</h1>
    </header>
    <section>
      <div class="container">
        <div class="triangle">
          <h1>&copyLOFTIES</h1>
        </div>
      </div>
    </section>
    
  </body>
</html>