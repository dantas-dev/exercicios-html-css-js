# Respostas Javascript (Manipulacao de DOM)

### 1
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de getElementById</title>
    </head>
    <body>
      <h1 id="meuTitulo">Meu Título</h1>
      <p id="meuParagrafo">Este é um parágrafo de exemplo.</p>
      
      <script>
        const titulo = document.getElementById("meuTitulo");
        const paragrafo = document.getElementById("meuParagrafo");
    
        console.log(titulo.textContent);
        console.log(paragrafo.textContent);
      </script>
    </body>
    </html>
  ```
    
### 2
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de getElementsByClassName</title>
    </head>
    <body>
      <h1 class="meuTitulo">Meu Título</h1>
      <p class="meuParagrafo">Este é um parágrafo de exemplo 1.</p>
      <p class="meuParagrafo">Este é um parágrafo de exemplo 2.</p>
      
      <script>
        // Acesse elementos HTML pela classe usando document.getElementsByClassName.
        const titulos = document.getElementsByClassName("meuTitulo");
        const paragrafos = document.getElementsByClassName("meuParagrafo");
    
        // Exiba o conteúdo dos elementos no console.
        for (const titulo of titulos) {
          console.log(titulo.textContent);
        }
    
        for (const paragrafo of paragrafos) {
          console.log(paragrafo.textContent);
        }
      </script>
    </body>
    </html>
  ```
    
### 3
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de querySelector</title>
    </head>
    <body>
      <h1 id="meuTitulo">Meu Título</h1>
      <p class="meuParagrafo">Este é um parágrafo de exemplo.</p>
      
      <script>
        // Acesse elementos HTML pelo seletor usando document.querySelector.
        const titulo = document.querySelector("#meuTitulo");
        const paragrafo = document.querySelector(".meuParagrafo");
    
        // Exiba o conteúdo dos elementos no console.
        console.log(titulo.textContent);
        console.log(paragrafo.textContent);
      </script>
    </body>
    </html>
  ```
    
### 4
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de querySelector</title>
    </head>
    <body>
      <h1 id="meuTitulo">Meu Título</h1>
      <p class="meuParagrafo">Este é um parágrafo de exemplo 1.</p>
        <p class="meuParagrafo">Este é um parágrafo de exemplo 2.</p>
      
      <script>
        // Acesse elementos HTML pelo seletor usando document.querySelector.
        const titulos = document.querySelectorAll("#meuTitulo");
        const paragrafos = document.querySelectorAll(".meuParagrafo");
    
        titulos.forEach((titulo) => {
          console.log(titulo.textContent);
        });
    
        paragrafos.forEach((paragrafo) => {
          console.log(paragrafo.textContent);
        });
      </script>
    </body>
    </html>
  ```
    
### 5
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de element.innerHTML</title>
    </head>
    <body>
      <p id="meuParagrafo">Este é um parágrafo de exemplo.</p>
      
      <script>
        // Acesse o elemento HTML pelo ID usando document.getElementById.
        const paragrafo = document.getElementById("meuParagrafo");
    
        // Acesse e exiba o conteúdo do elemento no console.
        console.log("Conteúdo original: " + paragrafo.innerHTML);
    
        // Atualize o conteúdo do elemento usando element.innerHTML.
        paragrafo.innerHTML = "Este é o novo conteúdo do parágrafo.";
    
        // Exiba o conteúdo atualizado no console.
        console.log("Conteúdo atualizado: " + paragrafo.innerHTML);
      </script>
    </body>
    </html>
  ```
    
### 6
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de element.setAttribute e element.getAttribute</title>
    
      <style>
        .paragrafo-original {
          color: red;
        }
    
        .paragrafo-modificado {
          color: green;
          font-size: 20px;
        }
      </style>
    </head>
    <body>
      <p id="meuParagrafo" class="paragrafo-original">Este é um parágrafo de exemplo.</p>
      
      <script>
        // Acesse o elemento HTML pelo ID usando document.getElementById.
        const paragrafo = document.getElementById("meuParagrafo");
    
        // Adicione uma nova classe ao elemento usando element.setAttribute.
        setTimeout(() => {
          paragrafo.setAttribute("class", "paragrafo-modificado");
    
          const classeAtual = paragrafo.getAttribute("class");
          console.log("Classe do elemento: " + classeAtual);
        }, 1000)
      </script>
    </body>
    </html>
  ```
    
### 7
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exemplo de document.createElement, element.appendChild e element.removeChild</title>
    </head>
    <body>
      <div id="container">
        <!-### O novo elemento será adicionado aqui. -->
      </div>
      
      <script>
        // Crie um novo elemento <p> usando document.createElement.
        const novoParagrafo = document.createElement("p");
        novoParagrafo.textContent = "Este é um novo parágrafo criado dinamicamente.";
    
        // Acesse o elemento pai onde desejamos adicionar o novo elemento.
        const container = document.getElementById("container");
    
        // Adicione o novo elemento como filho do elemento pai usando element.appendChild.
        container.appendChild(novoParagrafo);
    
        // Aguarde alguns segundos e depois remova o novo elemento usando element.removeChild.
        setTimeout(function() {
          container.removeChild(novoParagrafo);
          console.log('O elemento <p> foi excluido com sucesso!');
        }, 5000);
      </script>
    </body>
    </html>
  ```