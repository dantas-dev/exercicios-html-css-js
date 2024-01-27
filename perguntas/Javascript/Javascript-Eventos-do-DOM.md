# Exércicios Javascript (Eventos do DOM)

### 1. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse o elemento de botão `<button>` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  Acesse o elemento de parágrafo `<p>` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  “Escute” ao evento de `click` do botão usando `addEventListener`
  
  Ao botão ser clicado substitua o conteúdo do parágrafo para “O botão já foi clicado? Sim.”
  
  e exiba uma mensagem de sucesso no console. Exemplo de saida no console:
  
  ```bash
  Botão foi clicado com sucesso!
  ```
  
### 2. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse o elemento de`<input>` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  Acesse o elemento de parágrafo `<p>` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  “Escute” ao evento de `change` do `input` usando `addEventListener`
  
  Ao `input` ser modificado(ou seja, escrever algo nele) substitua o conteúdo do parágrafo para o conteúdo digitado dentro do input
  
  e exiba o conteúdo digitado também no console. Exemplo de saida no console (caso o usuário tenha digitado no input “Olá, esse e um teste.”:
  
  ```bash
  Valor digitado: Olá, esse e um teste.
  ```
  
### 3. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse o elemento de link `<a>` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  “Escute” ao evento de `click` do `<a>` usando `addEventListener`
  
  Ao `<a>` ser clicado, use `event.preventDefault()` para cancelar o comportamento padrão do link
  
  e em seguida exiba a mensagem no console "O comportamento padrão do link foi cancelado. Você permanece na mesma página.”:
  
  ```bash
  O comportamento padrão do link foi cancelado. Você permanece na mesma página.
  ```

  ### 4. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  ```html
 <!DOCTYPE html>
<html>
<head>
  <title>Exemplo de Evento de Hover</title>
  <style>
    #meuDiv {
      width: 200px;
      height: 200px;
      background-color: #3498db;
      margin: 20px;
    }
  </style>
</head>
<body>
  <div id="meuDiv"></div>

  <script>
    // Acesse o link pelo ID usando document.getElementById.
    const meuDiv = document.getElementById('meuDiv');

    // Adicione um ouvinte de evento de mouseover à div.
    meuDiv.addEventListener('mouseover', function() {
      meuDiv.style.backgroundColor = '#e74c3c';
    });
    
    // Adicione um ouvinte de evento de mouseout à div.
    meuDiv.addEventListener('mouseout', function() {
      meuDiv.style.backgroundColor = '#3498db';
    });
  </script>
</body>
</html>

  ```
   Acesse o elemento  `<div>` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  “Escute” ao evento de `mouseover` da `<div>` usando `addEventListener` e defina a cor de background como `#e74c3c`.

  “Escute” ao evento de `mouseout` da `<div>` usando `addEventListener` e defina a cor de background como `#3498db`.

  Ao passar o mouse pela div a cor da `<div>` deve mudar a cor para vermelho, ao retirar o mouse da `<div>` a mesma deve ficar com cor azul.

  ```