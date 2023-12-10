# Respostas Javascript (Objetos)

### 1
    
  ```jsx
    // Crie um objeto "pessoa" com algumas propriedades.
    const pessoa = {
      nome: "João",
      idade: 30,
      cidade: "São Paulo"
    };
    
    // Use Object.keys para listar as propriedades do objeto.
    const propriedades = Object.keys(pessoa);
    console.log("Propriedades do objeto pessoa: " + propriedades);
  ```
    
### 2
    
  ```jsx
    // Crie um objeto "frutas" com várias frutas e seus preços.
    const frutas = {
      maca: 1.99,
      banana: 0.79,
      pera: 2.49,
      uva: 3.99
    };
    
    // Use Object.values para obter um array com os preços das frutas.
    const precos = Object.values(frutas);
    
    console.log("Preços das frutas: " + precos);
  ```
    
### 3
    
  ```jsx
    // Crie um objeto "alunos" com nomes e idades dos alunos.
    const alunos = {
      Alice: 20,
      Bob: 22,
      Carol: 21,
      Dave: 23
    };
    
    // Use Object.entries para obter um array de arrays com pares nome-idade.
    const listaAlunos = Object.entries(alunos);
    
    console.log("Lista de alunos e idades: ");
    for (let i = 0; i < listaAlunos.length; i++) {
      const entrada = listaAlunos[i];
      const nome = entrada[0];
      const idade = entrada[1];
      console.log(nome + " tem " + idade + " anos.");
    }
  ```
    
### 4
    
  ```jsx
    // Crie um objeto "destino" e um objeto "origem" com propriedades.
    const destino = { a: 1, b: 2 };
    const origem = { b: 3, c: 4 };
    
    // Use Object.assign para copiar propriedades da origem para o destino.
    Object.assign(destino, origem);
    
    console.log("Objeto destino após Object.assign: ", destino);
  ```
    
### 5
    
  ```jsx
    // Crie um objeto protótipo "animal" com propriedades comuns a todos os animais.
    const animal = {
      tipo: "Desconhecido",
      som: "Desconhecido",
      fazerBarulho: function() {
        console.log("O " + this.tipo + " faz um som " + this.som);
      }
    };
    
    // Crie um novo objeto "gato" com base no protótipo "animal" usando Object.create.
    const gato = Object.create(animal);
    
    // Configure as propriedades específicas do objeto "gato".
    gato.tipo = "Gato";
    gato.som = "Miado";
    
    // Chame o método "fazerBarulho" para o gato.
    gato.fazerBarulho();
  ```