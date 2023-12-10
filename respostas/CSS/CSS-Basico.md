# Respostas CSS (Básico)

### 1
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <style>
        /* Use um seletor de tipo para estilizar todos os parágrafos */
        p {
          color: red;
        }
    
        /* Use um seletor de tipo para estilizar todos os cabeçalhos de nível 1 */
        h1 {
          color: blue;
        }
      </style>
    </head>
    <body>
      <h1>Título Principal</h1>
      <p>Este é um parágrafo de exemplo.</p>
      <h1>Outro Título</h1>
      <p>Este é outro parágrafo.</p>
      <h2>Subtítulo</h2>
    </body>
    </html>
  ```
    
### 2
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <style>
        /* Use um seletor de tipo para estilizar todos os parágrafos */
        .paragrafo {
          color: red;
        }
    
        /* Use um seletor de tipo para estilizar todos os cabeçalhos de nível 1 */
        #meuTitulo {
          color: blue;
        }
      </style>
    </head>
    <body>
      <h1 id="meuTitulo">Título Principal</h1>
      <p class="paragrafo">Este é um parágrafo de exemplo.</p>
      <h1>Outro Título</h1>
      <p>Este é outro parágrafo.</p>
      <h2>Subtítulo</h2>
      <p class="paragrafo">Este é mais um parágrafo.</p>
    </body>
    </html>
  ```
    
### 3
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <style>
        p {
          background-color: red;
          color: white;
          margin: 20px;
          padding: 10px;
        }
      </style>
    </head>
    <body>
      <p>Este é um parágrafo comum.</p>
    </body>
    </html>
  ```
    
### 4
  
  ```html
    <!DOCTYPE html>
    <html>
    
    <head>
      <style>
        a {
          color: green;
        }
    
        a:hover {
          color: red;
        }
    
        p::before {
          content: "Ínicio do parágrafo ### ";
        }
    
        p::after {
          content: " ### Fim do parágrafo.";
        }
      </style>
    </head>
    
    <body>
      <a href="https://www.example.com">Meu Link</a>
      <p>Este é um parágrafo comum.</p>
    </body>
    
    </html>
  ```
    
### 5
    
  ```md
    A ordem de precedência é determinada pela especificidade e pela ordem de declaração.
    No exemplo, o "paragrafo-especifico" tem a maior precedência devido ao seletor de ID
    seguido pelo elemento com a classe "texto-azul".
    
    O primeiro parágrafo não tem nenhuma classe ou ID específico, portanto, recebe a cor vermelha da Regra 1.
  ```
    
### 6
    
  ```md
    Neste exercício, criamos três regras CSS com diferentes níveis de especificidade:
    
    A Regra 1 é a mais específica, pois se aplica apenas aos parágrafos com o ID "paragrafo-especifico". Ela define a cor do texto como verde.
    
    A Regra 2 é específica para parágrafos com a classe "texto-azul". Ela define a cor do texto como azul.
    
    A Regra 3 é a menos específica e se aplica a todos os parágrafos. Ela define a cor do texto como vermelho.
    
    Ao abrir este código em um navegador, você verá como a especificidade das regras CSS afeta a cor do texto dos parágrafos. O parágrafo com o ID "paragrafo-especifico" tem a maior especificidade e será exibido em verde, o parágrafo com a classe "texto-azul" terá a cor azul, e o parágrafo comum será vermelho de acordo com a Regra 3. Isso demonstra como a especificidade influencia a aplicação das regras CSS.
  ```
    
### 7
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <style>
        /* Regra 1 ### Usa pixels (px) para definir o tamanho da fonte */
        .paragrafo-pixels {
          font-size: 16px;
        }
    
        /* Regra 2 ### Usa ems (em) para definir o tamanho da fonte */
        .paragrafo-ems {
          font-size: 2em;
        }
    
        /* Regra 3 ### Usa porcentagem (%) para definir o tamanho da fonte */
        .paragrafo-porcentagem {
          font-size: 120%;
        }
    
        /* Regra 4 ### Usa viewport width (vw) para definir o tamanho da fonte */
        .paragrafo-viewport {
          font-size: 5vw;
        }
      </style>
    </head>
    <body>
      <p class="paragrafo-pixels">Este parágrafo usa pixels (px) para o tamanho da fonte.</p>
      <p class="paragrafo-ems">Este parágrafo usa ems (em) para o tamanho da fonte.</p>
      <p class="paragrafo-porcentagem">Este parágrafo usa porcentagem (%) para o tamanho da fonte.</p>
      <p class="paragrafo-viewport">Este parágrafo usa viewport width (vw) para o tamanho da fonte.</p>
    </body>
    </html>
  ```