# Respostas Javascript (Eventos do DOM )

### 1
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de addEventListener</title>
    </head>
    <body>
      <button id="meuBotao">Clique em Mim</button>
      <p id="mensagem">O botão já foi clicado? Não.</p>
      
      <script>
        // Acesse o botão pelo ID usando document.getElementById.
        const botao = document.getElementById("meuBotao");
    
        // Acesse o parágrafo pelo ID onde exibiremos a mensagem.
        const mensagemParagrafo = document.getElementById("mensagem");
    
        // Adicione um ouvinte de evento de clique ao botão usando addEventListener.
        botao.addEventListener("click", function() {
          mensagemParagrafo.textContent = "O botão já foi clicado? Sim.";
          console.log('Botão foi clicado com sucesso!');
        });
      </script>
    </body>
    </html>
  ```
    
### 2
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de addEventListener com o Evento "change"</title>
    </head>
    <body>
      <input type="text" id="meuInput" placeholder="Digite algo">
      <p id="mensagem"></p>
      
      <script>
        // Acesse o campo de entrada de texto e o parágrafo pelo ID.
        const input = document.getElementById("meuInput");
        const mensagemParagrafo = document.getElementById("mensagem");
    
        // Adicione um ouvinte de evento "change" ao campo de entrada de texto.
        input.addEventListener("change", function() {
          mensagemParagrafo.textContent = "Valor atualizado: " + input.value;
    
          console.log(`Valor digitado: ${input.value}`);
        });
      </script>
    </body>
    </html>
  ```
    
### 3
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de event.preventDefault()</title>
    </head>
    <body>
      <p>Clique no link a seguir para ver o comportamento padrão:</p>
      <a href="https://www.example.com" id="meuLink">Exemplo.com</a>
      
      <script>
        // Acesse o link pelo ID usando document.getElementById.
        const link = document.getElementById("meuLink");
    
        // Adicione um ouvinte de evento de clique ao link.
        link.addEventListener("click", function(event) {
          // Use event.preventDefault() para cancelar o comportamento padrão do link.
          event.preventDefault();
          console.log("O comportamento padrão do link foi cancelado. Você permanece na mesma página.");
        });
      </script>
    </body>
    </html>
  ```