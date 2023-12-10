# Exércicios Node.js

### 1. Crie um arquivo com o nome `exemplo.json` . Com o conteúdo abaixo:
    
  ```json
  {
      "marca": "Toyota",
      "modelo": "Corolla",
      "ano": 2020,
      "cor": "prata",
      "motor": "1.8L"
  }
  
  ```
  
  Use o método `readFileSync` para ler o conteúdo do arquivo. Converta o conteúdo do arquivo para um objeto usando  `JSON.parse`. Exiba o conteúdo convertido no console. Exemplo de saida no console:
  
  ```bash
  Conteúdo do arquivo convertido:
  {
    marca: 'Toyota',
    modelo: 'Corolla',
    ano: 2020,
    cor: 'prata',
    motor: '1.8L'
  }
  ```
    
### 2. Crie um objeto exemplo com as seguintes propriedades:
    
  ```jsx
  const exemplo = {
    marca: 'Toyota',
    modelo: 'Corolla',
    ano: 2020,
    cor: 'prata',
    motor: '1.8L'
  }
  ```
  
  Converta o objeto acima para string utilizando  `JSON.stringify`. Use o método `writeFileSync` para criar um arquivo chamado `exemplo.json` com os dados do objeto convertido para string. Exiba ao final, uma mensagem de sucesso. Exemplo de saida no console:
  
  obs: vale notar que precisa ter sido criado o arquivo exemplo.json na sua pasta
  
  ```bash
  Arquivo exemplo.json salvo com sucesso!
  ```
    
### 3. Crie um servidor HTTP que responda com uma mensagem quando acessado. Utilize o `http.createServer` para criar o servidor.

  Defina na `response` o `head` com o código `200`, e o tipo de conteúdo como `text/plain`.
  Por fim, no `response` escreva a mensagem "Bem-vindo ao Meu Servidor HTTP”.
  Agora utilize o servidor criado para ouvir na porta 3000. Usando o método `listen`. 
  Utilize o código base abaixo para completar o exércicio:
    
  ```jsx
  // Importe o módulo http.
  const http = require('http');
  
  // Crie um servidor HTTP que responda com uma mensagem quando acessado.
  const servidor = http.createServer((req, res) => {
    // AQUI: Defina o cabeçalho de resposta com um código 200 (OK) e o tipo de conteúdo.
    
  
    // AQUI: Escreva a mensagem de resposta.
    
  });
  
  // AQUI: Configure o servidor para ouvir na porta 3000. Usando o método listen
  ```
  
  obs: precisa acessar a URL http://127.0.0.0:3000/ e aparecer na tela a seguinte mensagem: “Bem-vindo ao Meu Servidor HTTP!”
  
  Exemplo de saida no console: 
  
  ```bash
  O servidor está ouvindo em http://127.0.0.0:3000/
  ```
    
### 4. Utilize a função `setTimeout` para executar a função abaixo após 2 segundos:
    
  ```jsx
  function exibirMsg() {
    console.log("Após 2 segundos, esta mensagem é exibida.");
  }
  ```
  
  Exemplo de saida no console: 
  
  ```bash
  Após 2 segundos, esta mensagem é exibida.
    ```
    
### 5. Utilize a função `setInterval` para executar a função abaixo a cada segundo, Após 5 segundos pare de exibir a mensagem usando a função `clearInterval`.
    
  ```jsx
  function exibirMsg(segundos) {
    const palavra = segundos > 1 ? "segundos" : "segundo";
    console.log(`${segundos} ${palavra}`);
  }
  ```
  
  Exemplo de saida no console: 
  
  ```bash
  Iniciando programa...
  1 segundo
  2 segundos
  3 segundos
  4 segundos
  5 segundos
  A execução foi interrompida após 5 segundos.
  ```