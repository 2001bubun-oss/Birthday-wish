# Birthday-wish<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🎉 Happy Birthday Ivana! 🌹✨</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body {
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
            background-size: 400% 400%;
            font-family: 'Playfair Display', serif;
            overflow: hidden;
            position: relative;
            animation: gradientShift 8s ease infinite;
        }

        .container {
            text-align: center;
            position: relative;
            z-index: 20;
            perspective: 1000px;
        }

        .birthday-card {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(20px);
            padding: 40px 60px;
            border-radius: 30px;
            border: 2px solid rgba(255,255,255,0.3);
            box-shadow: 0 25px 50px rgba(0,0,0,0.3);
            transform-style: preserve-3d;
            animation: float 6s ease-in-out infinite, heartbeat 2s ease-in-out infinite;
        }

        h1 {
            font-size: 4.2em;
            background: linear-gradient(45deg, #ff6b9d, #ffd93d, #6bcf7f, #4ecdc4);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin: 0 0 15px 0;
            text-shadow: 0 0 30px rgba(255,255,255,0.8);
            animation: rainbowText 3s ease infinite, glowPulse 1.5s ease-in-out infinite alternate;
            font-weight: 700;
        }

        .name-glow {
            font-size: 5em;
            background: linear-gradient(45deg, #ff1744, #ff9100, #00e676);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: nameGlow 2s ease-in-out infinite alternate;
            display: block;
            margin-bottom: 10px;
        }

        p {
            font-size: 1.6em;
            color: white;
            margin: 20px 0;
            line-height: 1.5;
            text-shadow: 2px 2px 10px rgba(0,0,0,0.5);
            font-style: italic;
        }

        /* 3D Rose Petals */
        .rose-petal {
            position: absolute;
            width: 25px;
            height: 25px;
            background: radial-gradient(ellipse at center, #ff69b4 0%, #c71585 70%, transparent 100%);
            border-radius: 50% 0 60% 0;
            transform: rotateY(0deg) rotateZ(0deg);
            animation: petalFloat 8s infinite linear;
            box-shadow: 0 5px 15px rgba(255,105,180,0.6);
        }

        .rose-petal:nth-child(odd) { background: radial-gradient(ellipse at center, #ff1493 0%, #8b008b 70%); }
        .rose-petal:nth-child(3n) { background: radial-gradient(ellipse at center, #ff69b4 0%, #db7093 70%); }

        /* Magic Sparkles */
        .sparkle {
            position: absolute;
            width: 6px;
            height: 6px;
            background: radial-gradient(circle, #fff 0%, transparent 70%);
            border-radius: 50%;
            pointer-events: none;
            animation: sparkleBurst 2s infinite;
            box-shadow: 0 0 10px #fff;
        }

        /* Confetti */
        .confetti {
            position: absolute;
            width: 12px;
            height: 12px;
            background: #ff6b9d;
            animation: confettiFall 3s linear infinite;
        }

        /* Animations */
        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotateX(0deg); }
            50% { transform: translateY(-20px) rotateX(5deg); }
        }

        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        @keyframes rainbowText {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        @keyframes glowPulse {
            0% { filter: drop-shadow(0 0 20px rgba(255,255,255,0.8)); }
            100% { filter: drop-shadow(0 0 40px rgba(255,255,255,1)); }
        }

        @keyframes nameGlow {
            0% { text-shadow: 0 0 20px #ff1744, 0 0 40px #ff1744; }
            100% { text-shadow: 0 0 30px #00e676, 0 0 60px #00e676; }
        }

        @keyframes petalFloat {
            0% {
                transform: translateY(100vh) rotateY(0deg) rotateZ(0deg) scale(0);
                opacity: 0;
            }
            10% {
                opacity: 1;
                scale(1);
            }
            90% { opacity: 1; }
            100% {
                transform: translateY(-100px) rotateY(720deg) rotateZ(360deg) scale(0.8);
                opacity: 0;
            }
        }

        @keyframes sparkleBurst {
            0%, 100% { transform: scale(0) rotate(0deg); opacity: 0; }
            50% { transform: scale(1.2) rotate(180deg); opacity: 1; }
        }

        @keyframes confettiFall {
            0% {
                transform: translateY(-100vh) rotateZ(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(100vh) rotateZ(720deg);
                opacity: 0;
            }
        }

        @media (max-width: 768px) {
            h1 { font-size: 2.8em !important; }
            .name-glow { font-size: 3.5em !important; }
            .birthday-card { padding: 30px 40px; margin: 20px; }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="container">
        <div class="birthday-card">
            <h1>✨ Happy Birthday ✨</h1>
            <span class="name-glow">Ivana</span>
            <p>🌹 My heart blooms for you every day. May your special day be filled with infinite love, magic, and dreams coming true! 💖</p>
        </div>
    </div>

    <script>
        // 3D Rose Petals Rain
        function createPetal() {
            const petal = document.createElement('div');
            petal.className = 'rose-petal';
            petal.style.left = Math.random() * 100 + 'vw';
            petal.style.animationDuration = (Math.random() * 3 + 5) + 's';
            petal.style.animationDelay = Math.random() * 2 + 's';
            document.body.appendChild(petal);

            setTimeout(() => petal.remove(), 10000);
        }

        // Sparkle Explosion
        function createSparkle(x, y) {
            for(let i = 0; i < 8; i++) {
                const sparkle = document.createElement('div');
                sparkle.className = 'sparkle';
                sparkle.style.left = x + 'px';
                sparkle.style.top = y + 'px';
                sparkle.style.animationDelay = (i * 0.1) + 's';
                document.body.appendChild(sparkle);
                setTimeout(() => sparkle.remove(), 2000);
            }
        }

        // Confetti Burst
        function createConfetti() {
            for(let i = 0; i < 15; i++) {
                const confetti = document.createElement('div');
                confetti.className = 'confetti';
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.background = `hsl(${Math.random() * 360}, 80%, 60%)`;
                confetti.style.animationDelay = Math.random() * 2 + 's';
                confetti.style.animationDuration = (Math.random() * 2 + 2) + 's';
                document.body.appendChild(confetti);
                setTimeout(() => confetti.remove(), 4000);
            }
        }

        // Continuous Effects
        setInterval(createPetal, 200);
        setInterval(() => {
            const rect = document.querySelector('.birthday-card').getBoundingClientRect();
            createSparkle(rect.left + rect.width/2, rect.top + rect.height/2);
        }, 1500);
        setInterval(createConfetti, 4000);

        // Click for Sparkle Explosion
        document.addEventListener('click', (e) => createSparkle(e.clientX, e.clientY));
    </script>
</body>
</html>
