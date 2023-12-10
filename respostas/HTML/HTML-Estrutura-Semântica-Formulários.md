# Respostas HTML (Estrutura, Semântica e Formulários)

### 1
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <meta charset="UTF-8">
      <title>Exercício de Estrutura HTML</title>
    </head>
    <body>
      <header>
        Eu sou um header
      </header>
      <main>
          Eu sou um main
      </main>
      <footer>
        Eu sou um footer
      </footer>
    </body>
    </html>
  ```
    
### 2
    
  ```html
    <!DOCTYPE html>
    <html lang="pt-BR">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Exercício de Semântica HTML</title>
    </head>
    <body>
      <header>
        <h1>Meu Site</h1>
        <nav>
          <ul>
            <li><a href="#">Página Inicial</a></li>
            <li><a href="#">Sobre</a></li>
            <li><a href="#">Contato</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>Sobre Nós</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </section>
        <section>
          <h2>Contato</h2>
          <p>Você pode nos contatar pelo e-mail: exemplo@meusite.com</p>
        </section>
      </main>
      <footer>
        <p>&copy; 2023 Meu Site</p>
      </footer>
    </body>
    </html>
  ```
    
### 3
    
  ```html
    <!DOCTYPE html>
    <html>
    <head>
      <title>Exercício de Formulários HTML</title>
    </head>
    <body>
      <h1>Formulário de Contato</h1>
      <form action="processar-formulario.php" method="post">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required>
        
        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="mensagem">Mensagem:</label>
        <textarea id="mensagem" name="mensagem" rows="4" required></textarea>
        
        <input type="submit" value="Enviar">
      </form>
    </body>
    </html>
  ```