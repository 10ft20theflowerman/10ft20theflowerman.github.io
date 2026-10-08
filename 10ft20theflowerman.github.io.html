<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Bubble Sort</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        background: #f4f4f2;
        text-align: center;
        padding: 20px;
      }

      #bars {
        height: 320px;
        display: flex;
        align-items: flex-end;   /* as barras crescem para cima, a partir do chão */
        justify-content: center;
        gap: 6px;
        margin: 20px 0;
      }

      .bar {
        width: 30px;
        background: lightblue;
      }

      button {
        padding: 10px 16px;
        font-size: 16px;
        margin: 0 5px;
      }
    </style>
  </head>
  <body>
    <h1>Bubble Sort</h1>
    <p>Compare dois vizinhos. Se o da esquerda for maior, troque os dois de lugar. Repita!</p>

    <button id="startBtn">Iniciar</button>
    <button id="randomBtn">Embaralhar</button>

    <div id="bars"></div>
    <p id="message">Pronto.</p>

    <script>
      // A lista de números que vamos ordenar
      let numbers = [];

      // Pegamos os elementos da página que vamos usar
      const barsDiv = document.getElementById("bars");
      const message = document.getElementById("message");
      const startBtn = document.getElementById("startBtn");
      const randomBtn = document.getElementById("randomBtn");

      // Faz uma pausa para conseguirmos ver o que está acontecendo
      function wait(ms) {
        return new Promise(function (resolve) {
          setTimeout(resolve, ms);
        });
      }

      // Cria uma nova lista com 12 números aleatórios entre 10 e 99
      function makeNumbers() {
        numbers = [];
        for (let i = 0; i < 12; i++) {
          numbers.push(Math.floor(Math.random() * 90) + 10);
        }
        drawBars(-1, -1, numbers.length, "lightblue");
      }

      // Desenha uma barra para cada número.
      // first e second = as duas barras que estão sendo comparadas
      // sortedFrom = toda barra nesta posição ou depois já está pronta (verde)
      // color = a cor das duas barras que estão sendo comparadas
      function drawBars(first, second, sortedFrom, color) {
        barsDiv.innerHTML = "";

        for (let i = 0; i < numbers.length; i++) {
          const bar = document.createElement("div");
          bar.className = "bar";
          bar.style.height = numbers[i] * 3 + "px";

          if (i >= sortedFrom) {
            bar.style.background = "lightgreen";
          } else if (i === first || i === second) {
            bar.style.background = color;
          }

          barsDiv.appendChild(bar);
        }
      }

      // O Bubble Sort em si
      async function bubbleSort() {
        // Desliga os botões enquanto ordena
        startBtn.disabled = true;
        randomBtn.disabled = true;

        const n = numbers.length;

        for (let i = 0; i < n - 1; i++) {
          // Depois de i rodadas, as últimas i barras já estão no lugar certo
          const sortedFrom = n - i;

          for (let j = 0; j < n - 1 - i; j++) {
            // Mostra os dois números que estamos comparando (laranja)
            message.textContent = "Comparando " + numbers[j] + " e " + numbers[j + 1];
            drawBars(j, j + 1, sortedFrom, "orange");
            await wait(300);

            // Se o da esquerda for maior, troca os dois de lugar
            if (numbers[j] > numbers[j + 1]) {
              let temp = numbers[j];
              numbers[j] = numbers[j + 1];
              numbers[j + 1] = temp;

              message.textContent = "Trocou!";
              drawBars(j, j + 1, sortedFrom, "salmon");
              await wait(300);
            }
          }
        }

        // Tudo ordenado, então deixa todas as barras verdes
        message.textContent = "Pronto! A lista está ordenada.";
        drawBars(-1, -1, 0, "lightblue");

        // Liga os botões de novo
        startBtn.disabled = false;
        randomBtn.disabled = false;
      }

      // Liga os botões às nossas funções
      startBtn.addEventListener("click", bubbleSort);
      randomBtn.addEventListener("click", function () {
        makeNumbers();
        message.textContent = "Novos números prontos.";
      });

      // Cria a primeira lista quando a página carrega
      makeNumbers();
    </script>
  </body>
</html>
