<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cronómetro Futurista</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="styles/main.css">
</head>
<body class="futuristic">
    <canvas id="particle-canvas"></canvas>
    <div class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-md-8 text-center">
                <h1 class="my-4 neon-text">Cronómetro Futurista</h1>
                <div class="mb-3">
                    <select id="game-mode-selector" class="form-select neon-select">
                        <option value="classic">Clásico</option>
                        <option value="quickclick">Quick Click</option>
                        <option value="targettime">Target Time</option>
                    </select>
                </div>
            </div>
        </div>
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div id="game-circle-container">
                    <canvas id="game-circle"></canvas>
                    <div id="timer" class="neon-text">0.00</div>
                </div>
                <div id="quick-click-area"></div>
                <div id="score" class="text-center mt-3 neon-text">Puntuación: 0</div>
                <div id="message" class="text-center mt-2 neon-text"></div>
            </div>
        </div>
        <div class="row justify-content-center mt-4">
            <div class="col-md-8">
                <h2 class="text-center neon-text">Ranking</h2>
                <table class="table table-dark table-striped neon-table">
                    <thead>
                        <tr>
                            <th>Posición</th>
                            <th>Nombre</th>
                            <th>Puntuación</th>
                        </tr>
                    </thead>
                    <tbody id="ranking-body"></tbody>
                </table>
            </div>
        </div>
    </div>
    <div id="name-popup" class="popup">
        <div class="popup-content">
            <h2>Enter Your Name</h2>
            <input type="text" id="player-name" placeholder="Your Name">
            <button id="submit-name">Start Game</button>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <script src="scripts/script.js"></script>
</body>
</html>

