# Curso de HTML e CSS : Front-End Web Development Quick Start With HTML5, CSS, and JavaScript , da Pluralsight.

## HTML
### O que é o HTML?
HyperText Markup Language, como o próprio nome diz, o HTML é uma linguagem de marcação, usada para estrutar o texto e criar conexões com outros elementos do website. De maneira simplória: "O esqueleto" da página web. Esta marcação é dada em tags.

### Tags
Tags são instruções na linguagem de marcação, tendo uma marca de início e outra de fim para que o navegador possa renderizar uma página. ( < > , </ > ).

### Estrutura padrão 
```HTML
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
------------------------------------------
- flex-direction:
    - flex-direction: row;
    // Os itens ficam em linha
    - flex-direction: row-reverse;
    // Os itens ficam em linha reversa, ou      seja 3, 2, 1.
    -  flex-direction: column;
    // Os itens ficam em uma única coluna,      um embaixo do outro.
    - flex-direction: column-reverse;
    // Os itens ficam em uma única coluna,      um embaixo do outro, porém em ordem         reversa: 3, 2 e 1.
------------------------------------------
- **`display : grid;`**
