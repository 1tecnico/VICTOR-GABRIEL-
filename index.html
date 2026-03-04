<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mochila Victor - Problema da Mochila 0/1</title>

<style>
body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #141E30, #243B55);
    color: white;
    display: flex;
    justify-content: center;
    padding: 40px;
}

.container {
    background: rgba(255, 255, 255, 0.1);
    padding: 30px;
    border-radius: 15px;
    width: 600px;
    backdrop-filter: blur(15px);
    box-shadow: 0 0 20px rgba(0,0,0,0.4);
}

h1 {
    text-align: center;
    margin-bottom: 20px;
}

input {
    width: 100%;
    padding: 10px;
    margin: 6px 0;
    border-radius: 8px;
    border: none;
}

button {
    width: 100%;
    padding: 12px;
    margin-top: 10px;
    border: none;
    border-radius: 8px;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;
}

.btn-add {
    background-color: #00c6ff;
    color: white;
}

.btn-add:hover {
    background-color: #0072ff;
}

.btn-solve {
    background-color: #28a745;
    color: white;
}

.btn-solve:hover {
    background-color: #218838;
}

.lista {
    margin-top: 15px;
}

.lista ul {
    list-style: none;
    padding: 0;
}

.lista li {
    background: rgba(255,255,255,0.2);
    padding: 8px;
    margin: 5px 0;
    border-radius: 6px;
}

.resultado {
    margin-top: 20px;
    background: rgba(0,0,0,0.4);
    padding: 15px;
    border-radius: 10px;
}
</style>
</head>

<body>

<div class="container">
    <h1>🎒 Problema da Mochila 0/1</h1>

    <label>Capacidade da Mochila:</label>
    <input type="number" id="capacidade" placeholder="Ex: 50">

    <h3>Adicionar Item</h3>
    <input type="text" id="nome" placeholder="Nome do item">
    <input type="number" id="peso" placeholder="Peso">
    <input type="number" id="valor" placeholder="Valor">

    <button class="btn-add" onclick="adicionarItem()">Adicionar Item</button>

    <div class="lista">
        <h3>Itens Adicionados</h3>
        <ul id="listaItens"></ul>
    </div>

    <button class="btn-solve" onclick="resolverMochila()">Resolver Mochila</button>

    <div class="resultado" id="resultado"></div>
</div>

<script>
let itens = [];

function adicionarItem() {
    const nome = document.getElementById("nome").value;
    const peso = parseInt(document.getElementById("peso").value);
    const valor = parseInt(document.getElementById("valor").value);

    if (!nome || isNaN(peso) || isNaN(valor)) {
        alert("Preencha todos os campos corretamente!");
        return;
    }

    itens.push({ nome, peso, valor });
    atualizarLista();

    document.getElementById("nome").value = "";
    document.getElementById("peso").value = "";
    document.getElementById("valor").value = "";
}

function atualizarLista() {
    const lista = document.getElementById("listaItens");
    lista.innerHTML = "";

    itens.forEach((item) => {
        const li = document.createElement("li");
        li.textContent = `${item.nome} - Peso: ${item.peso} | Valor: ${item.valor}`;
        lista.appendChild(li);
    });
}

function resolverMochila() {
    const capacidade = parseInt(document.getElementById("capacidade").value);

    if (isNaN(capacidade)) {
        alert("Informe a capacidade da mochila!");
        return;
    }

    const n = itens.length;
    let dp = Array(n + 1).fill(null).map(() => Array(capacidade + 1).fill(0));

    for (let i = 1; i <= n; i++) {
        for (let w = 0; w <= capacidade; w++) {
            if (itens[i - 1].peso <= w) {
                dp[i][w] = Math.max(
                    itens[i - 1].valor + dp[i - 1][w - itens[i - 1].peso],
                    dp[i - 1][w]
                );
            } else {
                dp[i][w] = dp[i - 1][w];
            }
        }
    }

    let w = capacidade;
    let escolhidos = [];

    for (let i = n; i > 0; i--) {
        if (dp[i][w] !== dp[i - 1][w]) {
            escolhidos.push(itens[i - 1]);
            w -= itens[i - 1].peso;
        }
    }

    let resultadoDiv = document.getElementById("resultado");

    resultadoDiv.innerHTML = `
        <h3>Resultado</h3>
        <p><strong>Valor Máximo:</strong> ${dp[n][capacidade]}</p>
        <p><strong>Itens Escolhidos:</strong></p>
        <ul>
            ${escolhidos.map(item => 
                `<li>${item.nome} (Peso: ${item.peso}, Valor: ${item.valor})</li>`
            ).join("")}
        </ul>
    `;
}
</script>

</body>
</html>
