# Alex Barroso Paz 
<h1 align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Verdana&pause=1000&color=60FFCA&center=true&vCenter=true&width=435&lines=Olá!+Meu+nome+é+Alex+Barroso+Paz.;Sou+um+Desenvolvedor+Full+Stack.">
  </a>
</h1>

<div align="center">
  <a href="https://github.com/finntroll89">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=finntroll89&show_icons=true&theme=aura&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=finntroll89&layout=compact&langs_count=7&theme=aura"/>
  </a>
</div>

##

### 🚀 Tecnologias & Ferramentas:

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,javascript,typescript,react,next,nodejs,express,python,django,java,spring,mysql,postgresql,firebase,mongodb,docker,git,linux,vscode" />
  </a>
</p>

##

### 📬 Contato:

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alex Barroso Paz</title>
    <style>
        body {
            margin: 0;
            padding: 20px;
            background: #0d1117;
            color: #c9d1d9;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', Helvetica, Arial, sans-serif;
            line-height: 1.5;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        h1 {
            text-align: center;
            margin: 30px 0;
        }
        
        .stats-container {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin: 30px 0;
            flex-wrap: wrap;
        }
        
        .stats-container img {
            border-radius: 8px;
        }
        
        h3 {
            color: #58a6ff;
            margin: 30px 0 20px 0;
        }
        
        .tech-section {
            text-align: center;
            margin: 40px 0;
        }
        
        .contact-section {
            text-align: center;
            margin: 40px 0;
        }
        
        .social-buttons {
            margin-bottom: 30px;
        }
        
        .social-buttons a {
            margin: 0 10px;
            text-decoration: none;
            display: inline-block;
            transition: transform 0.3s ease;
        }
        
        .social-buttons a:hover {
            transform: scale(1.1);
        }
        
        /* Game Styles */
        .game-container {
            width: 500px;
            height: 400px;
            background: linear-gradient(135deg, #000428 0%, #004e92 100%);
            border: 3px solid #60FFCA;
            border-radius: 15px;
            margin: 20px auto;
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 30px rgba(96, 255, 202, 0.3);
        }
        
        /* Invader ETs (top enemies moving like Space Invaders) */
        .invader-row {
            position: absolute;
            width: 100%;
            display: flex;
            justify-content: space-around;
            animation: invader-move 4s linear infinite;
        }
        
        .invader-row:nth-child(3) {
            top: 50px;
            animation-delay: 0s;
        }
        
        .invader-row:nth-child(4) {
            top: 90px;
            animation-delay: 0.5s;
        }
        
        .invader-row:nth-child(5) {
            top: 130px;
            animation-delay: 1s;
        }
        
        .invader {
            width: 30px;
            height: 25px;
            background: linear-gradient(45deg, #ff4081, #e91e63);
            border-radius: 40% 40% 60% 60%;
            position: relative;
            animation: invader-pulse 1s ease-in-out infinite;
        }
        
        .invader::before {
            content: '👾';
            position: absolute;
            top: -3px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 16px;
        }
        
        /* Player spaceship (bottom) */
        .player-ship {
            width: 50px;
            height: 30px;
            background: linear-gradient(45deg, #00ff41, #7cb342);
            position: absolute;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 0 0 50% 50%;
            box-shadow: 0 0 20px #00ff41;
            animation: player-move 6s ease-in-out infinite;
        }
        
        .player-ship::before {
            content: '🚀';
            position: absolute;
            top: -5px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 20px;
        }
        
        /* Lasers */
        .laser {
            width: 3px;
            height: 25px;
            position: absolute;
            border-radius: 50%;
        }
        
        .player-laser {
            background: linear-gradient(0deg, #00ff41, #ffffff);
            animation: player-laser-shoot 2s linear infinite;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .enemy-laser {
            background: linear-gradient(0deg, #ff4081, #ffffff);
            animation: enemy-laser-shoot 3s linear infinite;
        }
        
        .enemy-laser:nth-of-type(6) {
            left: 100px;
            animation-delay: 0s;
        }
        
        .enemy-laser:nth-of-type(7) {
            left: 200px;
            animation-delay: 1s;
        }
        
        .enemy-laser:nth-of-type(8) {
            left: 300px;
            animation-delay: 2s;
        }
        
        .stars {
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: 
                radial-gradient(1px 1px at 20px 30px, #fff, transparent),
                radial-gradient(1px 1px at 40px 70px, #fff, transparent),
                radial-gradient(1px 1px at 90px 40px, #fff, transparent),
                radial-gradient(1px 1px at 130px 80px, #fff, transparent),
                radial-gradient(1px 1px at 160px 30px, #fff, transparent),
                radial-gradient(1px 1px at 220px 50px, #fff, transparent),
                radial-gradient(1px 1px at 280px 90px, #fff, transparent),
                radial-gradient(1px 1px at 320px 20px, #fff, transparent),
                radial-gradient(1px 1px at 360px 110px, #fff, transparent),
                radial-gradient(1px 1px at 400px 60px, #fff, transparent);
            background-repeat: repeat;
            background-size: 450px 150px;
            animation: twinkle 3s ease-in-out infinite;
        }
        
        .game-title {
            position: absolute;
            top: 15px;
            left: 50%;
            transform: translateX(-50%);
            color: #60FFCA;
            font-family: 'Courier New', monospace;
            font-size: 16px;
            font-weight: bold;
            text-shadow: 0 0 15px #60FFCA;
            z-index: 10;
        }
        
        .score {
            position: absolute;
            top: 45px;
            left: 20px;
            color: #00ff41;
            font-family: 'Courier New', monospace;
            font-size: 12px;
            text-shadow: 0 0 10px #00ff41;
            z-index: 10;
        }
        
        /* Animations */
        @keyframes invader-move {
            0% { transform: translateX(0); }
            25% { transform: translateX(80px); }
            50% { transform: translateX(80px) translateY(20px); }
            75% { transform: translateX(-80px) translateY(20px); }
            100% { transform: translateX(-80px) translateY(40px); }
        }
        
        @keyframes invader-pulse {
            0%, 100% { 
                transform: scale(1);
                filter: brightness(1);
            }
            50% { 
                transform: scale(1.1);
                filter: brightness(1.3);
            }
        }
        
        @keyframes player-move {
            0%, 100% { left: 20%; }
            25% { left: 40%; }
            50% { left: 60%; }
            75% { left: 80%; }
        }
        
        @keyframes player-laser-shoot {
            0% { 
                bottom: 70px;
                opacity: 1;
            }
            100% { 
                bottom: 400px;
                opacity: 0;
            }
        }
        
        @keyframes enemy-laser-shoot {
            0% { 
                top: 180px;
                opacity: 1;
            }
            100% { 
                top: 400px;
                opacity: 0;
            }
        }
        
        @keyframes twinkle {
            0%, 100% { opacity: 0.7; }
            50% { opacity: 1; }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .stats-container {
                flex-direction: column;
            }
            
            .stats-container img {
                max-width: 100%;
                height: auto;
            }
            
            .game-container {
                width: 90%;
                max-width: 400px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header with typing animation -->
        <h1 align="center">
            <a href="https://git.io/typing-svg">
                <img src="https://readme-typing-svg.herokuapp.com?font=Verdana&pause=1000&color=60FFCA&center=true&vCenter=true&width=435&lines=Olá!+Meu+nome+é+Alex+Barroso+Paz.;Sou+um+Desenvolvedor+Full+Stack.">
            </a>
        </h1>

        <!-- GitHub Stats -->
        <div class="stats-container">
            <a href="https://github.com/finntroll89">
                <img height="180em" src="https://github-readme-stats.vercel.app/api?username=finntroll89&show_icons=true&theme=aura&include_all_commits=true&count_private=true"/>
                <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=finntroll89&layout=compact&langs_count=7&theme=aura"/>
            </a>
        </div>

        <!-- Tech Section -->
        <div class="tech-section">
            <h3>🚀 Tecnologias & Ferramentas:</h3>
            <p align="center">
                <a href="https://skillicons.dev">
                    <img src="https://skillicons.dev/icons?i=html,css,javascript,typescript,react,next,nodejs,express,python,django,java,spring,mysql,postgresql,firebase,mongodb,docker,git,linux,vscode" />
                </a>
            </p>
        </div>

        <!-- Contact Section -->
        <div class="contact-section">
            <h3>📬 Contato:</h3>
            
            <!-- Botões de contato -->
            <div class="social-buttons">
                <a href="mailto:wallezpaz@gmail.com" target="_blank">
                    <img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
                </a>
                <a href="https://www.linkedin.com/in/alex-barroso-paz" target="_blank">
                    <img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
                </a>
                <a href="https://wa.me/5592988356730?text=Ol%C3%A1%2C%20vim%20pelo%20GitHub" target="_blank">
                    <img src="https://img.shields.io/badge/-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
                </a>
            </div>
            
            <!-- Título Redes Sociais -->
            <h3>Redes Sociais</h3>
            
            <!-- ET Space Invaders Game -->
            <div class="game-container">
                <div class="stars"></div>
                <div class="game-title">ET SPACE INVADERS</div>
                <div class="score">SCORE: 9999</div>
                
                <!-- Enemy Invader Rows -->
                <div class="invader-row">
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                </div>
                
                <div class="invader-row">
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                </div>
                
                <div class="invader-row">
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                    <div class="invader"></div>
                </div>
                
                <!-- Player Ship -->
                <div class="player-ship"></div>
                
                <!-- Lasers -->
                <div class="laser player-laser"></div>
                <div class="laser enemy-laser"></div>
                <div class="laser enemy-laser"></div>
                <div class="laser enemy-laser"></div>
            </div>
        </div>
    </div>
</body>
</html>
