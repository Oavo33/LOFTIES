<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>CSS3 3D Cube</title>
    <style>@media only screen and (max-width: 600px) {
      body { margin: 0; padding: 0; }
      .container {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        perspective: 800px;
        width: 200px;
        height: 200px;
      }.cube {
        position: relative;
        transform-style: preserve-3d;
        width: 100%;
        height: 100%;
        transform: translateZ(-100px);
        animation: rotate 100s linear infinite;
      }.face {
        position: absolute;
        width: 150px;
        height: 150px;
        box-sizing: border-box;
        border-radius: 5px;
        clip-path: polygon(50% 0%, 63% 38%, 100% 38%, 69% 59%, 82% 100%, 50% 75%, 18% 100%, 31% 59%, 0% 38%, 37% 38%);
        transition: transform 0.5s ease;
        animation: fade-in 0.5s forwards;
        border: 10px solid transparent;
        background-image: linear-gradient(to right, #f00, #800000);
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
      }.front { transform: rotateY(0deg) translateZ(100px); }
      .back { transform: rotateY(180deg) translateZ(100px); }
      .left { transform: rotateY(-90deg) translateZ(100px); }
      .right { transform: rotateY(90deg) translateZ(100px); }
      .top { transform: rotateX(90deg) translateZ(100px); }
      .bottom { transform: rotateX(-90deg) translateZ(100px); }
      .cube:hover .face {
        transform: translateZ(100px) rotateX(360deg) rotateY(360deg) rotateZ(360deg);
        animation: fade-out 0.5s forwards;
      }@keyframes rotate {
        from { transform: rotateX(0) rotateY(0) rotateZ(0); }
        to { transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg); }
      }@keyframes fade-in {
        from { opacity: 0; }
        to { opacity: 1; }
      }@keyframes fade-out {
        from { opacity: 1; }
        to { opacity: 0.1; }
      }}
    </style>
  </head>
  <body>
    <div class="container">
      <div class="cube">
        <div class="face front">LOFTIES</div>
        <div class="face back">LOFTIES</div>
        <div class="face left">LOFTIES</div>
        <div class="face right">LOFTIES</div>
        <div class="face top">LOFTIES</div>
        <div class="face bottom">LOFTIES</div>
      </div>
    </div>
  </body>
</html>


