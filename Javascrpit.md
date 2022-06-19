
### Variaveis
    string 
        var nome ="Felipe"
    number
        var idade = 24
    boolean
        var texte = true

### Escreve do html
    var texto = "<h1>Bem Vindo</h1>"
    document.write(texto)
---------------------------------------------------
    var nome = "Felipe"
    document.write("<h1>O meu no é" + nome + " e estou apreendendo a usar o javascript</h1>")

### Usar o console
        console.log()

### Usar o alert
        alert()

### Usar o sistema de id para passagem de informação
    document.getElementById('nome').value = 'Bem vindo'

### Escreveer no alert
    var nome = prompt("Escreva seu nome")
    console.log(nome)

### if/else
    var idade = 10 
    if (idade > 11)
    {
        console.log(idade)
    }
    else(idade > 11)
    {
        console.log(idade + idade)
    }
    
    toString, parseInt, parseFloat
    var v1 = "10"
    var v2 = "10.5"
    var v3 = 10
    
    v1 = parseInt(v1)
    v2 = parseFloat(v2)
    
    document.write(v1+v2)
    document.write("<p></p>")
    document.write(v3.toString())

### Uso do Swich
    var opcao = 2
    switch(opcao){
        case 1:
        console.log("Certo")
        break
    
        case 2:
        console.log("Certo")
        break
    
        default:
        console.log("Errado")
        break
    }

### Uso de Funções
    function area(largura,comprimento){
        var area = largura * comprimento
        return area
    }
    console.log(area(10,15))

### funções anonimas e tecnica de wrapper  
    var a = function(nome){
            document.write("Olá " + nome)
        }
    a('felipe')

### Funções nativas para mudança de Strings
 var nome = "Felipe Giglio"
       document.write("Felipe Giglio".charAt(4))
       document.write(nome.indexOf('8'))
       document.write(nome.replace("Giglio","Silva "))
       document.write("Felipe Giglio".toUpperCase())  

### Funções nativas para mudança de tarefas matematicas
 var x = Math.ceil(10.38)
      var y = Math.floor(10.38)
      var i = Math.random()
      document.write(y)
      document.write("<br>")
      document.write(x)
      document.write("<br>")
      document.write(i)

### Funções nativas para manipular datas
      var data = new Date()
       var n = data.getDate()
       var d = data.getDate()
       var m = data.getMonth()
       var a = data.getFullYear()
      document.write(n)
      document.write("<br>")
      document.write(d +"/"+ m + "/" + a)
      
### Praticando funções de Datas
       var data = new Date()
       document.write(data)
       document.write('<hr>')
       document.write(data.getFullYear())
    
### Eventos com mouse
        onclick
        ondblclick
        onmouseup
        onmouseover
        onmeuseout

        <script>
            function acao(){
                document.write("Evento")
            }
        </script>
    </head>
    <body>
    <button onmouseover="acao()">Botão</button>
    </body>

### Eventos com o teclado
   onkeydown = usar qualquer tecla
   onkeupress
   onkeyup   

### Eventos janela
        onscroll
        onresize

        <script>
            function acao(){
                console.log("Evento")
            }
        </script>
    </head>
    <body onresize="acao()">
        
    </body>

### Evento Formulario
        onfocus
        onblur
        onchange

        <script>
            function acao(){
                console.log("Evento")
                document.write("<hr>")
            }
        </script>
    </head>
    <body>
        <form action="">
        <input onfocus="acao()" type="text ">
        </form>

### Uso do Dom APi
        getElementById()
        getElementByTagName()
        getElementsByClassName()
        getElementsByName()

### Exemplo
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Javacript</title>
    </head>
    <body>
        <hr>
        <input type="text" onkeyup="distribuicao()" placeholder="Digite um Caracter aqui" id="entrada">
        <hr>
        <span>Letras:</span>
        <input type="text" placeholder="Digite Letras" id="letras" disabled>
        <span>Numeros:</span>
        <input type="text" placeholder="Digite Numeros"id="numeros" disabled>
        <hr>
    <script>
        function distribuicao(){
            var caracter = document.getElementById('entrada').value
        
        document.getElementById('entrada').value = ''

        caracter.trim()

        switch(caracter){
        case '0':
        case '1':
        case '2':
        case '3':
        case '4':
        case '5':
        case '6':
            document.getElementById('numeros').value = caracter
            break
            default:
            document.getElementById('letras').value = caracter
        }
        }
    </script>
    </body>
    </html>    

    ### fd



