<!DOCTYPE html>
<html>
<head>
    <style>
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
            height: 100px;
            overflow: hidden;
        }#triangle-container div {
            position: absolute;
            width: 10px;
            height: 10px;
            transform: skewX(-56deg);
        }@media (min-width: 768px) {
            #triangle-container {
                height: 200px; 
            }#triangle-container div {
                width: 20px;
                height: 20px; 
            }
        }
    </style>
</head>
<body>
    <header>
        <div id="triangle-container"></div>
        <h1>Header Content</h1>
    </header>
<script>
        var triangleContainer = document.getElementById("triangle-container");
        var numTriangles = Math.ceil(window.innerWidth / 10);
        var startColor = [128, 0, 0]; // Dark color in RGB (#800000)
        var endColor = [0, 179, 179]; // Light color in RGB (#00b3b3)
        var spacing = 2; // Adjust spacing between triangles
function generateTriangles() {
            triangleContainer.innerHTML = '';
for (var i = 0; i < numTriangles; i++) {var r = Math.round(startColor[0] + (endColor[0] - startColor[0]) * i / (numTriangles - 1));
                var g = Math.round(startColor[1] + (endColor[1] - startColor[1]) * i / (numTriangles - 1));
                var b = Math.round(startColor[2] + (endColor[2] - startColor[2]) * i / (numTriangles - 1));var color = 'rgb(' + r + ',' + g + ',' + b + ')';
    var startX = (i * (10 + spacing)); 
var triangle = document.createElement('div');
                triangle.style.left = startX + 'px';
                triangle.style.backgroundColor = color;
triangleContainer.appendChild(triangle);
            }
        }
        generateTriangles();
window.addEventListener('resize', function() {
            numTriangles = Math.ceil(window.innerWidth / 10);
            generateTriangles();
        });
    </script>
</body>
</html>


