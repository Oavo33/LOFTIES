<!DOCTYPE html>
<html>
<head><style>@media only screen and (max-width: 600px) {
       .container {
            display: flex;
        }
        .button {
            background-color: #30b3b3;
            position: relative;
            width: 200px;
            height: 50px;
            color: #30b3b3;
            text-align: center;
            line-height: 50px;
            font-size: 20px;
            font-family: Arial, sans-serif;
            cursor: pointer;
            transition: transform 0.5s, background-color 0.5s;
            overflow: hidden;
            animation: colorTransition 3.5s infinite;
            border: 2px solid #800000;
            border-radius: 50px;
            box-sizing: border-box;
        }
@keyframes colorTransition {
            0% { background-color: #800000; }
            6.25% { background-color: #751a1a; }
            12.5% { background-color: #6b3434; }
            18.75% { background-color: #605050; }
            25% { background-color: #546b6b; }
            31.25% { background-color: #488686; }
            37.5% { background-color: #3c9fa0; }
            43.75% { background-color: #00b3b3; }
            50% { background-color: #00b3b3; }
            56.25% { background-color: #3c9fa0; }
            62.5% { background-color: #488686; }
            68.75% { background-color: #546b6b; }
            75% { background-color: #605050; }
            81.25% { background-color: #6b3434; }
            87.5% { background-color: #751a1a; }
            93.75% { background-color: #800000; }
            100% { background-color: #800000; }
        }
.button:hover:before {
            border-right: 40px solid #00b3b3;
            opacity: 1;
            transform: translate(-50%, -50%) rotate(45deg) scale(1.2);
        }
.button.clicked {
            transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg);
        }
.button:after {
            content: "";
            position: absolute;
            top: 2px;
            left: 2px;
            width: calc(100% - 4px);
            height: calc(100% - 4px);
            opacity: 0;
            border: 2px solid #00b3b3;
            transition: opacity 1.5s;
            pointer-events: none;
            mix-blend-mode: overlay;
        }
.button span.number {
            z-index: 3;
            color: black;
        }
.button i {
            margin-right: 5px;
        }}
    </style>
</head>
<body>
    <div class="container">
        <button class="button" onclick="handleClick(event)">
            <i class="icon game-icon">&#x1F3AE;</i>
            <span class="text">LoftiesGames</span>
        </button>
        <button class="button replica-button" onclick="handleClick(event)">
            <i class="icon video-icon">&#x1F3A5;</i>
            <span class="text">LoftiesVideos</span>
        </button>
    </div>
<script>
        var clickCount = 0;
function handleClick(event) {
            event.stopPropagation();
            clickCount++;
            var button = event.target.closest('.button');
            var number = document.createElement('span');
            switch (clickCount) {
                case 1: number.textContent = 'Games'; break;
                case 2: number.textContent = 'Are'; break;
                case 3: number.textContent = 'Coming'; break;
                case 4: number.textContent = 'Soon'; break;
                case 5: number.textContent = 'I Hope'; break;
                default: number.textContent = clickCount; break;
            }
            number.className = 'number';
            button.innerHTML = '';
            button.appendChild(document.createElement('i')).className = 'icon';
            button.appendChild(number);
            animateButton(button);
            if (clickCount >= 5) window.location.href = "https://example.com";
        }function animateButton(button) {
            button.classList.add('clicked');
            setTimeout(function() {
                button.classList.remove('clicked');
            }, 500);
        }
    </script>
</body>
</html>






