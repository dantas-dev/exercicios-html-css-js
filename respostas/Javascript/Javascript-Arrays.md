# Respostas Javascript (Arrays)

### 1
  
  ```jsx
    // Crie um array vazio chamado "frutas".
    const frutas = [];
    
    // Use o método "push" para adicionar algumas frutas ao array.
    frutas.push("Maçã");
    frutas.push("Banana");
    frutas.push("Morango");
    
    // Exiba o array atualizado no console.
    console.log("Array de frutas: " + frutas);
  ```
  
### 2
  
  ```jsx
  // Crie um array de cores.
    const cores = ["vermelho", "verde", "azul", "amarelo"];
    
    // Use o método "pop" para remover e retornar a última cor do array.
    const corRemovida = cores.pop();
    
    // Exiba a cor removida e o array atualizado no console.
    console.log("Cor removida: " + corRemovida);
    console.log("Array de cores atualizado: " + cores);
  ```
  
### 3
  
  ```jsx
    // Crie dois arrays de números.
    const array1 = [1, 2, 3];
    const array2 = [4, 5, 6];
    
    // Use o método "concat" para combinar os dois arrays em um novo array.
    const arrayCombinado = array1.concat(array2);
    
    // Exiba o novo array combinado no console.
    console.log("Array combinado: " + arrayCombinado);
  ```
  
### 4
  
  ```jsx
    // Crie um array com nomes de cores.
    const cores = ["vermelho", "verde", "azul", "amarelo"];
    
    // Use o método "join" para converter os elementos do array em uma string separada por vírgulas.
    const coresString = cores.join(", ");
    
    // Exiba a string resultante no console.
    console.log("Cores: " + coresString);
  ```
  
### 5
  
  ```jsx
    // Crie um array de números.
    const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    
    // Use o método "slice" para criar uma cópia dos elementos entre a posição 2 (inclusive) e 5 (exclusiva).
    const subArray = numeros.slice(2, 5);
    
    // Exiba o subarray no console.
    console.log("Subarray: " + subArray);
  ```
  
### 6
  
  ```jsx
    // Crie um array de frutas.
    const frutas = ["Maçã", "Banana", "Morango", "Laranja"];
    
    // Use o método "splice" para remover "Banana" do array.
    const frutaRemovida = frutas.splice(1, 1);
    
    // Use o método "splice" para adicionar "Pera" e "Uva" no lugar de "Morango".
    const a = frutas.splice(1, 1, "Pera", "Uva");
    
    // Exiba o array atualizado e a fruta removida no console.
    console.log("Array de frutas: " + frutas);
    console.log("Fruta removida: " + frutaRemovida);
  ```
  
### 7
  
  ```jsx
    // Crie um array de nomes de cores.
    const cores = ["vermelho", "verde", "azul", "amarelo"];
    
    // Use o método "indexOf" para encontrar a posição de "azul" no array.
    const posicaoAzul = cores.indexOf("azul");
    
    // Exiba a posição de "azul" no console.
    console.log("A cor 'azul' está na posição: " + posicaoAzul);
  ```
  
### 8
  
  ```jsx
    // Crie um array de números.
    const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    
    // Use o método "filter" para criar um novo array contendo apenas os números pares.
    const numerosPares = numeros.filter(function(numero) {
      return numero % 2 === 0;
    });
    
    // Exiba o novo array com os números pares no console.
    console.log("Números pares: " + numerosPares);
  ```
  
### 9
  
  ```jsx
    // Crie um array de números.
    const numeros = [1, 2, 3, 4, 5];
    
    // Use o método "map" para criar um novo array com o dobro de cada número.
    const numerosDobrados = numeros.map(function(numero) {
      return numero * 2;
    });
    
    // Exiba o novo array com os números dobrados no console.
    console.log("Números dobrados: " + numerosDobrados);
  ```
  
### 10
  
  ```jsx
    // Crie um array de números.
    const numeros = [1, 2, 3, 4, 5];
    
    // Use o método "reduce" para encontrar a soma de todos os números no array.
    const soma = numeros.reduce(function(acumulador, numero) {
      return acumulador + numero;
    }, 0); // O segundo argumento é o valor inicial do acumulador.
    
    // Exiba a soma no console.
    console.log("Soma dos números: " + soma);
  ```
  
### 11
  
  ```jsx
    // Crie um array de nomes de frutas.
    const frutas = ["Maçã", "Banana", "Morango", "Laranja"];
    
    // Use o método "forEach" para exibir cada nome de fruta no console.
    frutas.forEach(function(fruta) {
      console.log("Nome da fruta: " + fruta);
    });
  ```
  
### 12
  
  ```jsx
  // Crie um array de idades.
    const idades = [25, 32, 28, 21, 37];
    
    // Use o método "every" para verificar se todas as idades são maiores que 18.
    const todasMaioresQue18 = idades.every(function(idade) {
      return idade > 18;
    });
    
    // Exiba o resultado no console.
    if (todasMaioresQue18) {
      console.log("Todas as idades são maiores que 18.");
    } else {
      console.log("Pelo menos uma das idades não é maior que 18.");
    }
  ```
  
### 13
  
  ```jsx
    // Crie um array vazio chamado "frutas".
    const frutas = [];
    
    // Use o método "push" para adicionar algumas frutas ao array.
    frutas.push("Maçã");
    frutas.push("Banana");
    frutas.push("Morango");
    
    // Exiba o array atualizado no console.
    console.log("Array de frutas: " + frutas);
  ```