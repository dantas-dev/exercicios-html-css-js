# Exércicios Javascript (Manipulacao de DOM)

### 1. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  
  ```
  
  Acesse elementos HTML pelo ID usando `document.getElementById`.
  
  Exiba o conteudo do título e do parágrafo no console. Exemplo de saida no console:
  
  ```bash
  Meu Título
  Este é um parágrafo de exemplo.
  ```
  
### 2. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  
  ```
  
  Acesse elementos HTML pela classe usando `document.getElementsByClassName`.
  
  Note que esse método retorna uma lista de elementos, você pode usar o `for…of` loop para exibi-los no console, um a um.
  
  Exiba o conteudo do título e dos parágrafo no console. Exemplo de saida no console:
  
  ```bash
  Meu Título
  Este é um parágrafo de exemplo 1.
  Este é um parágrafo de exemplo 2.
  ```
  
### 3. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse elementos HTML pelo seletor CSS usando `document.querySelector`.
  
  Exiba o conteudo do título e do parágrafo no console. Exemplo de saida no console:
  
  ```bash
  Meu Título
  Este é um parágrafo de exemplo.
  ```
  
### 4. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse elementos HTML pelo seletor CSS usando `document.querySelectorAll`.
  
  Note que esse método retorna uma lista de elementos, você pode usar o `forEach` para exibi-los no console, um a um.
  
  Exiba o conteudo do título e do parágrafo no console. Exemplo de saida no console:
  
  ```bash
    Meu Título
    Este é um parágrafo de exemplo 1.
    Este é um parágrafo de exemplo 2.
  ```
  
### 5. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
  ```html
  <!DOCTYPE html>
  <html>
  <head>
    <title>Exemplo de element.innerHTML</title>
  </head>
  <body>
    <p id="meuParagrafo">Este é um parágrafo de exemplo.</p>
    <script>
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse o elemento HTML usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  Exiba o conteúdo original do elemento no console.

  Agora atualize o conteúdo do elemento usando `element.innerHTML` para "Este é o novo conteúdo do parágrafo.”

  Exiba o conteúdo atualizado no console. Exemplo de saida no console:
  
  ```bash
  Conteúdo original: Este é um parágrafo de exemplo.
  Conteúdo atualizado: Este é o novo conteúdo do parágrafo.
  ```
  
### 6. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
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
    <p id="meuParagrafo" class="paragrafo-original">
      Este é um parágrafo de exemplo.
    </p>
    <script>
        // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Acesse o elemento HTML usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  Após 1 segundo (use o `setTimeout` para isso). Substitua a classe do elemento usando `element.setAttribute`.
  
  Exiba a classe atualizada do elemento no console `element.getAttribute`.

  Exemplo de saida no console:
  
  ```bash
  Classe do elemento: paragrafo-modificado
  ```
  
### 7. Crie um arquivo `index.html`. Com o conteúdo abaixo:
  
  ```html
  <!DOCTYPE html>
  <html>
  <head>
    <title>Exemplo de document.createElement, element.appendChild e element.removeChild</title>
  </head>
  <body>
    <div id="container">
      <!-- O novo elemento será adicionado aqui. -->
    </div>
    
    <script>
      // seu codigo resposta aqui
    </script>
  </body>
  </html>
  ```
  
  Crie um novo elemento `<p>` usando `document.createElement` com o conteúdo "Este é um novo parágrafo criado dinamicamente.”
  
  Acesse o elemento `<div id="container">` usando qualquer um dos métodos ja aprendidos nos exercicios anteriores.
  
  Adicione o novo elemento como filho do elemento `<div id="container">` usando `element.appendChild`.
  
  Após 5 segundos (use o `setTimeout` para isso). Remova o novo elemento usando `element.removeChild`.
  
  Exiba uma mensagem de sucesso no console.
  Exemplo de saida no console:
  
  ```bash
  O elemento <p> foi excluido com sucesso!
  ```