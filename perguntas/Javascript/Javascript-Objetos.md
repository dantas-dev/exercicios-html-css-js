# Exércicios Javascript (Objetos)

### 1. Crie um objeto "pessoa" com algumas propriedades: 
  ```jsx
    const pessoa = {
      nome: "João",
      idade: 30,
      cidade: "São Paulo"
    };
  ```
    
  Use `Object.keys` para listar as propriedades do objeto. Exemplo de saida no console:
    
  ```bash
    Propriedades do objeto pessoa: nome,idade,cidade
  ```

### 2. Crie um objeto `frutas` com várias frutas e seus preços:
    
  ```jsx
    const frutas = {
      maca: 1.99,
      banana: 0.79,
      pera: 2.49,
      uva: 3.99
    };
  ```
    
  Use `Object.values` para obter um array com os preços das frutas. Exemplo de saida no console:
    
  ```bash
    Preços das frutas: 1.99,0.79,2.49,3.99
  ```

### 3. Crie um objeto `alunos` com nomes e idades dos alunos.

  ```jsx
    const alunos = {
      Alice: 20,
      Bob: 22,
      Carol: 21,
      Dave: 23
    };
  ```
    
  Use `Object.entries` para obter um array de pares nome-idade. Exemplo de saida no console:
    
  ```bash
    Lista de alunos e idades: 
    Alice tem 20 anos.
    Bob tem 22 anos.
    Carol tem 21 anos.
    Dave tem 23 anos.
  ```

### 4. Crie um objeto `destino` e um objeto `origem` com propriedades:

  ```jsx
    const destino = { a: 1, b: 2 };
    const origem = { b: 3, c: 4 };
  ```
    
  Use `Object.assign` para copiar propriedades da `origem` para o `destino`. Exemplo de saida no console:
    
  ```bash
    Objeto destino após Object.assign:  { a: 1, b: 3, c: 4 }
  ```

### 5. Crie um objeto `animal` com propriedades comuns a todos os animais:

  ```jsx
    const animal = {
      tipo: "Desconhecido",
      som: "Desconhecido",
      fazerBarulho: function() {
        console.log("O " + this.tipo + " faz um som " + this.som);
      }
    };
  ```
    
  Crie um novo objeto `gato` com base no objeto `animal` usando `Object.create`. Altere para que o a propriedade `tipo` seja `Gato` e a propriedade `som` seja `Miado`. Chame o método "fazerBarulho" para o gato. Exemplo de saida no console:
    
  ```bash
    O Gato faz um som Miado
  ```
