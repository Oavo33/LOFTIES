<!DOCTYPE html>
<html>
  <head>
    <title>Modern Bucket</title>
    <style>
      body {
        background-color: #800000;
      }
      
      .bucket {
        width: 300px;
        height: 300px;
        border-radius: 0 0 50% 50%;
        border: 8px solid #006400;
        margin: 80px auto;
        position: relative;
        overflow: hidden;
        transition: all 4s ease-out;
        transform-origin: bottom center;
      }

      .bucket:before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 1%;
        background-color: black;
      }
      
      .bucket .water {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 0;
        background-color: #F7DC6F;
        transition: height 0.5s ease-in-out;
        border-radius: 0 0 50% 50%;
        border: 8px solid #F7DC6F;
        border-top: none;
      }

      .bucket:hover .water {
        height: 95%;
      }

      .bucket:hover {
        animation: shake 8s ease-in-out 0s 2 alternate;
      }

      @keyframes shake {
        0% {
          transform: rotate(-14deg);
        }
        100% {
          transform: rotate(14deg);
        }
      }
      
    </style>
  </head>
  <body>
    <div class="bucket">
      <div class="water"></div>
    </div>
  </body>
</html>

