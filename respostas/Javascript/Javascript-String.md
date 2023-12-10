# Respostas Javascript (String)

### 1
    
  ```jsx
    // Crie uma string com uma frase.
    const frase = "Estou aprendendo Javascript.";
    
    // Use a propriedade "length" para contar o número de caracteres na frase.
    const numeroCaracteres = frase.length;
    
    // Exiba o número de caracteres no console.
    console.log("O número de caracteres na frase é: " + numeroCaracteres);
  ```
    
### 2
    
  ```jsx
    // Crie uma string com uma palavra.
    const palavra = "JavaScript";
    
    // Use o método "charAt" para acessar o caractere na posição 3.
    const terceiroCaractere = palavra.charAt(3);
    
    // Exiba o terceiro caractere no console.
    console.log("O terceiro caractere na palavra é: " + terceiroCaractere);
  ```
    
### 3
    
  ```jsx
    // Crie duas strings.
    const string1 = "Olá, ";
    const string2 = "mundo!";
    
    // Use o método "concat" para combinar as duas strings.
    const mensagem = string1.concat(string2);
    
    // Exiba a mensagem combinada no console.
    console.log(mensagem);
  ```
    
### 4
    
  ```jsx
    // Crie uma string.
    const frase = "Javascript é muito top.";
    
    // Use o método "substring" para extrair uma parte da frase.
    const subfrase = frase.substring(13, 18);
    
    // Exiba a subfrase no console.
    console.log("Parte extraida: " + subfrase);
  ```
    
### 5
    
  ```jsx
    // Crie uma string com uma frase que contenha a palavra "exemplo".
    const frase = "Esta é uma frase de exemplo, e o exemplo é simples.";
    
    // Use o método "replace" para substituir a primeira ocorrência da palavra "exemplo" por "amostra".
    const novaFrase = frase.replace("exemplo", "amostra");
    
    // Exiba a nova frase no console.
    console.log("Nova frase: " + novaFrase);
  ```
    
### 6
    
  ```jsx
    // Crie uma string com espaços em branco no início e no final.
    const texto = "   Este é um texto com espaços em branco.   ";
    
    // Use o método "trim" para remover os espaços em branco no início e no final do texto.
    const textoSemEspacos = texto.trim();
    
    // Exiba o texto sem espaços no console.
    console.log("Texto sem espaços em branco: " + textoSemEspacos);
  ```
    
### 7
    
  ```jsx
    // Crie uma string com palavras separadas por vírgulas.
    const listaPalavras = "maçã,banana,morango,uva,laranja";
    
    // Use o método "split" para dividir a string em um array de palavras.
    const arrayPalavras = listaPalavras.split(',');
    
    // Exiba o array resultante no console.
    console.log("Array de palavras: " + arrayPalavras);
  ```
    
### 8
    
  ```jsx
    // Crie uma string que contém uma frase.
    const frase = "O JavaScript é uma linguagem de programação popular.";
    
    // Use o método "includes" para verificar se a string contém a palavra "JavaScript".
    const contemJavaScript = frase.includes("JavaScript");
    
    // Exiba o resultado no console.
    if (contemJavaScript) {
      console.log("A frase contém a palavra 'JavaScript'.");
    } else {
      console.log("A frase não contém a palavra 'JavaScript'.");
    }
  ```