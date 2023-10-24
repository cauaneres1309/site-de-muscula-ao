<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro de Musculação</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
        }

        .container {
            background-color: #fff;
            max-width: 400px;
            margin: 20px auto;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }

        label {
            display: block;
            margin: 10px 0;
        }

        input {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background-color: #0074d9;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Cadastro de Musculação</h1>
        <form id="cadastro-form">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" required>

            <label for="idade">Idade:</label>
            <input type="number" id="idade" required>

            <label for="peso">Peso (kg):</label>
            <input type="number" id="peso" required>

            <label for="musculo">Músculo a Aprimorar:</label>
            <input type="text" id="musculo" required>

            <button type="button" onclick="cadastrar();return false">Cadastrar</button>
        </form>
    </div>

    <script>
        function cadastrar() {
            const nome = document.getElementById("nome").value;
            const idade = document.getElementById("idade").value;
            const peso = document.getElementById("peso").value;
            const musculo = document.getElementById("musculo").value;

            
            alert(`Nome: ${nome}\nIdade: ${idade}\nPeso: ${peso} kg\nMúsculo a Aprimorar: ${musculo}`);
            location.href="site de musculaçao.html";
        }
    </script>
</body>
</html>
