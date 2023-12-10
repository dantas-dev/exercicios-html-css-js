# Respostas Node.js

### 1
    
  ```jsx
    // Importe o módulo fs.
    const fs = require('fs');
    
    const conteudo = fs.readFileSync('exemplo.json', 'utf-8');
    const conteudoParse = JSON.parse(conteudo);
    
    // Exiba o conteúdo do arquivo no console.
    console.log('Conteúdo do arquivo convertido:');
    console.log(conteudoParse);
  ```
    
### 2
    
  ```jsx
    // Importe o módulo fs.
    const fs = require('fs');
    
    // Conteúdo a ser gravado no arquivo.
    const exemplo = {
      marca: 'Toyota',
      modelo: 'Corolla',
      ano: 2020,
      cor: 'prata',
      motor: '1.8L'
    }
    
    const exemploStr = JSON.stringify(exemplo);
    
    fs.writeFileSync('exemplo.json', exemploStr);
    
    console.log('Arquivo exemplo.json salvo com sucesso!');
  ```
    
### 3
    
  ```jsx
    // Importe o módulo http.
    const http = require('http');
    
    // Crie um servidor HTTP que responda com uma mensagem quando acessado.
    const servidor = http.createServer((req, res) => {
      // Defina o cabeçalho de resposta com um código 200 (OK) e o tipo de conteúdo.
      res.writeHead(200, { 'Content-Type': 'text/plain' });
    
      // Escreva a mensagem de resposta.
      res.end('Bem-vindo ao Meu Servidor HTTP!\n');
    });
    
    // Configure o servidor para ouvir na porta 3000.
    servidor.listen(3000, () => {
      console.log('O servidor está ouvindo em http://127.0.0.0:3000/');
    });
  ```
    
### 4
    
  ```jsx
    function exibirMsg() {
      console.log("Após 2 segundos, esta mensagem é exibida.");
    }
    
    setTimeout(exibirMsg, 2000);
  ```
    
### 5
    
  ```jsx
    console.log("Iniciando programa...");
    
    function exibirMsg(segundos) {
      const palavra = segundos > 1 ? "segundos" : "segundo";
      console.log(`${segundos} ${palavra}`);
    }
    
    let contador = 0;
    
    const intervalo = setInterval(function() {
      contador++;
      exibirMsg(contador);
    
      if (contador >= 5) {
        clearInterval(intervalo);
        console.log("A execução foi interrompida após 5 segundos.");
      }
    }, 1000);
  ```