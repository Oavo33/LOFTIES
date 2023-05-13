<!DOCTYPE html>
<html>
<head>
    <title>Colorful Triangles</title>
    <style>@media only screen and (max-width: 600px)   {
        body {
            margin: 0;
            padding: 0;
        }header {
            position: relative;
            background-color: #f2f2f2;
            text-align: center;
            padding: 20px;
        }#triangle-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 30px;
        }#myCanvas {
            display: block;
            margin: 0 auto;
        }}
    </style>
</head>
<body>
    <header>
        <div id="triangle-container">
            <canvas id="myCanvas"></canvas>
        </div>
        <h1>Header Content</h1>
    </header>
<script>@media only screen and (max-width: 600px)   {
  .clock {
        var canvas = document.getElementById("myCanvas");
        var ctx = canvas.getContext("2d");
var startColor = [128, 0, 0]; // Dark color in RGB (#800000)
        var endColor = [0, 179, 179]; // Light color in RGB (#00b3b3)
var baseWidth = 7; // Change the size of the triangles here
based on the header width
        var numTriangles = Math.ceil(window.innerWidth / baseWidth);
// Adjust the canvas width based on the number of triangles
        canvas.width = baseWidth * numTriangles;
// Loop through and draw triangles
        for (var i = 0; i < numTriangles; i++) {
            // Calculate the color for the current triangle
            var r = Math.round(startColor[0] + (endColor[0] - startColor[0]) * i / (numTriangles - 1));
            var g = Math.round(startColor[1] + (endColor[1] - startColor[1]) * i / (numTriangles - 1));
            var b = Math.round(startColor[2] + (endColor[2] - startColor[2]) * i / (numTriangles - 1));
// Convert the RGB values to a CSS color string
            var color = 'rgb(' + r + ',' + g + ',' + b + ')';
 // Calculate the starting x position of the triangle
            var startX = i * baseWidth;
// Draw the triangle
            ctx.beginPath();
            ctx.moveTo(startX, 10);
            ctx.lineTo(startX + baseWidth / 2, 0);
            ctx.lineTo(startX + baseWidth, 14);
            ctx.closePath();// Set the fill color
            ctx.fillStyle = color;
// Fill the triangle with the calculated color
            ctx.fill();
        }}}
    </script>
</body></html>

