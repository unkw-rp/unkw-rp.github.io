<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Site</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        #menu {
            text-align: center;
            background-color: #333;
            padding: 10px;
        }
        #menu button {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 10px 20px;
            margin: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        #menu button:hover {
            background-color: #555;
        }
        #content {
            text-align: center;
            margin: 20px;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <div id="menu">
        <button onclick="showPage(1)">Top Rank</button>
        <button onclick="showPage(2)">Servidores</button>
        <button onclick="showPage(3)">Comprar VIP</button>
        <button onclick="showPage(4)">Regras</button>
    </div>
    <div id="content">
        <div id="page1" class="hidden">
            <h1>Página 1</h1>
            <!-- Conteúdo da Página 1 -->
        </div>
        <div id="page2" class="hidden">
            <h1>Página 2</h1>
            <!-- Conteúdo da Página 2 -->
        </div>
        <div id="page3" class="hidden">
            <h1>Página 3</h1>
            <!-- Conteúdo da Página 3 -->
        </div>
        <div id="page4" class="hidden">
            <h1>Regras</h1>
            <ol>
                <li>Não é permitido spam ou flood no chat.</li>
                <li>Seja respeitoso com outros jogadores e evite comportamentos tóxicos.</li>
                <li>Respeite as regras específicas do servidor e do jogo em que está jogando.</li>
                <li>Não compartilhe informações pessoais ou sensíveis no chat.</li>
                <li>Qualquer forma de trapaça ou uso de programas ilegais resultará em banimento permanente.</li>
            </ol>
        </div>
    </div>

    <script>
        function showPage(pageNumber) {
            for (let i = 1; i <= 4; i++) {
                document.getElementById(`page${i}`).classList.add('hidden');
            }
            document.getElementById(`page${pageNumber}`).classList.remove('hidden');
        }
    </script>
</body>
</html>
