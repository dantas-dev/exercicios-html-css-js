# Respostas Javascript (Loops)

### 1
    
  ```jsx
    const numero = 7;
    
    console.log("Tabuada de multiplicação de " + numero + ":");
    
    for (let i = 1; i <= 10; i++) {
      const resultado = numero * i;
      console.log(numero + " x " + i + " = " + resultado);
    }
  ```
    
### 2
    
  ```jsx
    let numeroInicial = 5;
    
    console.log("Contagem regressiva:");
    
    while (numeroInicial >= 1) {
      console.log(numeroInicial);
      numeroInicial--;
    }
  ```
    
### 3
    
  ```jsx
    const numeroMaximo = 10; 
    
    console.log("Contagem crescente:");
    
    let numeroAtual = 1;
    
    do {
      console.log(numeroAtual);
      numeroAtual++;
    } while (numeroAtual <= numeroMaximo);
  ```
    
### 4
    
  ```jsx
    // Crie um objeto que represente um carro com várias propriedades, como marca, modelo, ano, cor, etc.
    const carro = {
      marca: "Toyota",
      modelo: "Corolla",
      ano: 2020,
      cor: "prata",
      motor: "1.8L",
    };
    
    // Use um loop "for...in" para iterar sobre as propriedades do objeto e exibir os pares chave-valor.
    console.log("Detalhes do Carro:");
    
    for (const chave in carro) {
      console.log(chave + ": " + carro[chave]);
    }
  ```
    
### 5
    
  ```jsx
    // Crie um array que contenha nomes de frutas.
    const frutas = ["Maçã", "Banana", "Laranja", "Morango", "Uva"];
    
    // Use um loop "for...of" para iterar sobre os elementos do array e exibir cada nome de fruta.
    console.log("Lista de Frutas:");
    
    for (const fruta of frutas) {
      console.log(fruta);
    }
  ```