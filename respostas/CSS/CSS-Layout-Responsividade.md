# Respostas CSS (Layout e Responsividade)

### 1
  
  ```html
    <!DOCTYPE html>
    <html>
    
    <head>
      <style>
        body {
          margin: 0;
          padding: 0;
          border: 0;
        }
    
        .item {
          width: 300px;
          height: 300px;
          background-color: tomato;
          margin: 10px;
          padding: 10px;
        }
        
        .container {
          display: flex;
        }
      </style>
    </head>
    
    <body>
      <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
      </div>
    </body>
    
    </html>
  ```
  
### 2
  
  ```html
    <!DOCTYPE html>
    <html>
    
    <head>
      <style>
        body {
          margin: 0;
          padding: 0;
          border: 0;
        }
    
        .item {
          color: white;
          height: 20px;
          width: 100%;
          background-color: purple;
          padding: 10px;
          margin: 4px;
          max-width: 25%;
        }
    
        .container {
          display: flex;
          flex-wrap: wrap;
        }
        
      </style>
    </head>
    
    <body>
      <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Item 5</div>
        <div class="item">Item 6</div>
        <div class="item">Item 7</div>
        <div class="item">Item 8</div>
        <div class="item">Item 9</div>
      </div>
    </body>
    
    </html>
  ```
  
### 3
  
  ```html
    <!DOCTYPE html>
    <html>
    
    <head>
      <style>
        body {
          margin: 0;
          padding: 0;
          border: 0;
        }
    
        .item {
          color: white;
          background-color: blue;
          height: 100px;
          width: 100px;
        }
    
        .container {
          background-color: tomato;
          height: 300px;
          width: 300px;
    
          display: flex;
          align-items: center;
          justify-content: center;
        }
        
      </style>
    </head>
    
    <body>
      <div class="container">
        <div class="item">Item 1</div>
      </div>
    </body>
    
    </html>
  ```