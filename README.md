# Curso de HTML e CSS : Front-End Web Development Quick Start With HTML5, CSS, and JavaScript , da Pluralsight.

## HTML
### O que é o HTML?
HyperText Markup Language, como o próprio nome diz, o HTML é uma linguagem de marcação, usada para estrutar o texto e criar conexões com outros elementos do website. De maneira simplória: "O esqueleto" da página web. Esta marcação é dada em tags.

### Tags
Tags são instruções na linguagem de marcação, tendo uma marca de início e outra de fim para que o navegador possa renderizar uma página. ( < > , </ > ).

### Estrutura padrão 
``` HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title> Titulo da página </title>
</head>
<body>
    
</body>
</html>
``` 
- **Nota**: Os elementos dados entre < > e </ > são as chamadas tags. 
- Para gerar essa estrutura inicial basta digitar ! no seu editor de texto.
------------------------------------------
### Inline vs Block Elements
Os elementos 


### Criando Listas
- Lista Não Ordenada 
Lista sem numeração, a qual a ordem não importa. Usa-se a tag < ul > e para criar elementos de lista usa-e < li >
``` CSS
<ul>
    <li> Item 1  </li>
    <li> Item 2  </li>
    <li> Item 3  </li>
</ul>
```
- Lista Ordenada
Lista numerada (1,2, 3...), a qual se importa em ordenar. Usa-se a tag < ol > e para criar elementos de lista usa-e < li >

``` CSS
<ol>
    <li> Item 1  </li>
    <li> Item 2  </li>
    <li> Item 3  </li>
</ol>
```
------------------------------------------
### Criando Formulários
``` HTML

<body>
    <form> 
        <!-- circuncidar os elementos de form com divs, para colocar em bloco e gerar espaço. -->
        <div>
        <label for="fullName"> FullName</label> <!-- Label é o cabeçalho dentro do input que colocarmos, precisa da propriedade for= para apontar o input. -->
        </div>

        <div>
            <input id="fullName" type="text" /> <!-- Type define o tipo de input desejado -->
        </div>

        <div>
        <label for="email"> Email</label> 
        </div>

         <div>
        <input id="email" type="text" />
        </div>

        <div>
            <label for="subject"> Subject</label> 
        </div>

        <div> <!-- Cria um bota de seleçao de opçoes -->
            <select id="subject">
                <option>Job Offer</option>
                <option>Personal Message </option>
                <option>Complaint</option>
        </div>

        <div>
            <label for="msg"> Message</label> 
        </div>
        
        <div> 
            <textarea id="msg" rows="4"> </textarea> <!-- Cria uma area de texto para digitacao-->
        </div>

        <div>
            <input type="submit" value="Send Mail"> <!-- Botao de envio, nao precisa de label, se poe o texto em value-->
        </div>
    </form>
</body>
</html>
```
------------------------------------------
### Criando Tabelas
 Inicializada com a tag `<table> `e e struturada em Caption (cabeçalho), thead, tbody e tfood. No "thead" são adicionadas linhas `<tr>` e dentro das linhas são adicionadas colunas `<th> `, para a criação de colunas na tabela. Para adicionar dados na tabela usamos o `<td>`.
  **Legenda:** <br>
    tr:  (table rows) <br>
    th:  (table height) <br>
    td : (table data) <br>
    
 ### Estrutura básica no HTML:
    ``` HTML
          <table>
        <thead>
            <tr>
                <th> </th>
                <th></th>
                <th></th>
            </tr>
        </thead>
        <tbody></tbody>
        <tfoot></tfoot>
    </table>
     ```
Colspan —> Mescla colunas
Rowspan —> Mescla linhas
------------------------------------------
## CSS

### Display Content
O `display` define um layout para o seu CSS.

- **Opçoes de Display:**
- `display : block;`
Define o alinhamento dos itens do container em bloco, um sobre o outro verticalmente.
- `display : inline;`
Define o alinhamento dos itens do conteiner de forma que possam ficar lado a lado.
- `display : hidden;`
Altera a visibilidade do container, mas ainda deixa o espaço alocado por ele, ocultando apenas os itens do container. Usado juntamente do JS para menu de seleção, caso um item seja selecionado exibe-se o conteúdo de hidden.
- `display : none;`
Diferente do `display: hidden`, este tipo de display oculta também o espaço alocado pelo container.
------------------------------------------
- **`display : flex;`**
Torna o elemento um flex container automaticamente transformando todos os seus filhos diretos em flex itens.

- flex-direction:
    - flex-direction: row;
    // Os itens ficam em linha
    - flex-direction: row-reverse;
    // Os itens ficam em linha reversa, ou      seja 3, 2, 1.
    -  flex-direction: column;
    // Os itens ficam em uma única coluna,      um embaixo do outro.
    - flex-direction: column-reverse;
    // Os itens ficam em uma única coluna,      um embaixo do outro, porém em ordem         reversa: 3, 2 e 1.
 - flex-wrap:
    - flex-wrap: nowrap;
    // Valor padrão, não permite a quebra       de linha.
    -flex-wrap: wrap;
    // Quebra a linha assim que um dos          flex itens não puder mais ser              compactado.
    -flex-wrap: wrap-reverse;
    // Quebra a linha assim que um dos            flex itens não puder mais ser             compactado. A quebra é na direção         contrária, ou seja para a linha           acima.  
 - flex-flow
    - flex-flow: row nowrap;
    // Coloca o conteúdo em linha e não         permite a quebra de linha.
    - flex-flow: row wrap;
    // Coloca o conteúdo em linha e            permite a quebra de linha.
    - flex-flow: column nowrap;
    // Coloca o conteúdo em coluna e não        permite a quebra de linha.
------------------------------------------
- **`display : grid;`**
A ideia é que você tem itens individuais que serão exibidos naturalmente em uma grade, e você pode especificar quantos itens serão exibidos nessa grid.

Neste módulo usa-se um modelo de grid, onde se configura trechos de texto para especificar onde queremos o cabeçalho, rodapé, o conteúdo e a barra lateral se existir na página.

Modelo lógico citado:
```CSS
grid-template-areas:
 "header header"
  "main sidebar"
   "footer footer";
   ```
------------------------------------------
## JavaScript
    Iniciar com uma tag script no HTML, essa tag precisa de um início `<script>` e um fim `</script>`, ou criar uma pagina .js externa e apenas importá-la usando uma anchor na tag script criada.
------------------------------------------

### Objeto
Um objeto é qualquer coisa que represente algo mais complexo que os tipos primitivos, os objetos tem os seus próprios dados.
------------------------------------------

### Condicional IF
- Estrutura:
``` bash
    if(var === conditional &&  var=== conditional2 || var === conditional 3 ) 
    {
        //faça alguma coisa
    }
    else{
        //senão faça isso
    }
```
&& = "e"
|| = "ou"
------------------------------------------
### DOM
Document Object Model, o HTML funciona em uma estrutura de árvore e uma dessas estruturas mais básica é a classse Document que é derivada da `window.document` e da documente se deriva `document.head`, `document.body` entre outras...
### Events 
Capturar eventos que acontecem na página é um ponto crucial da programação web.
- Estrutura:
``` bash
//geralmente capturamos o elemento a ser trabalhado em forma de objeto ou seja retorna um objeto
const element = document.getElemetById ("id do elemento")
// ou 
const vetElement = document.getElemetByClassName ("nome da classe que deseja obter os elementos")
// retorna um vetor com todos elementos da classe (vetor de objetos)

//Evento
element.addEventListener ("qualEvento" , function (event){
event.target  = ação a ser realizada ;
//captura o elemento que disparou o evento 
```
------------------------------------------
### Webpack
"De maneira simples, Webpack é um empacotador de módulos para aplicações javascript." Pega todos os nosso arquivos .js ou .css e funde-os em um formato que o navegador possa compilar mais facilmente. Ele também transpila o seu código, que é pegar o código e garantir que ele seja válido no maior número de navegadores possível. É necessário baixá-lo via npm.

- Principais comandos:
    - ./"nomeDaClasse.js"
        Cria o arquivo formatado com todas suas classes         .js
    -   ./"nomeDaClasse.js" --mode development
        Altera o modo de formatação do arquivo para um           modo legível.
        
     -   ./"nomeDaClasse.js" --mode watch
        Altera o arquivo para o modo watch.
        
