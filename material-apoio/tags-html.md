# Guia Completo de TAGs HTML

Neste guia, você encontrará uma explicação detalhada de todas as TAGs HTML, bem como suas propriedades e uso adequado.

## Índice

1. [Introdução](#introdução)
2. [TAGs HTML](#tags-html)
   1. [TAG `<html>`](#tag-html)
   2. [TAG `<head>`](#tag-head)
   3. [TAG `<body>`](#tag-body)
   4. [TAGs de Títulos](#tags-de-títulos)
   5. [TAGs de Parágrafos](#tags-de-parágrafos)
   6. [TAGs de Links](#tags-de-links)
   7. [TAG `<img>`](#tag-img)
   8. [TAG `<div>`](#tag-div)
   9. [TAG `<span>`](#tag-span)
   10. [TAG `<ul>`](#tag-ul)
   11. [TAG `<ol>`](#tag-ol)
   12. [TAG `<li>`](#tag-li)
   13. [TAG `<table>`](#tag-table)
   14. [TAG `<tr>`](#tag-tr)
   15. [TAG `<td>`](#tag-td)
   16. [TAG `<form>`](#tag-form)
   17. [TAG `<input>`](#tag-input)
   18. [TAG `<button>`](#tag-button)
   19. [TAG `<textarea>`](#tag-textarea)
   20. [TAG `<select>`](#tag-select)
   21. [TAG `<option>`](#tag-option)
   


## Introdução

HTML (HyperText Markup Language) é a linguagem padrão para criação e estruturação de páginas web. As TAGs HTML são elementos usados para definir a estrutura e o conteúdo de uma página. Cada TAG HTML possui uma função específica e pode ter várias propriedades.

Neste guia, forneceremos informações detalhadas sobre as TAGs HTML mais comumente utilizadas, bem como suas propriedades e exemplos de uso.

## TAGs HTML

### TAG `<html>`

A TAG `<html>` é o elemento raiz de um documento HTML e engloba todo o conteúdo da página. Todas as outras TAGs HTML devem estar contidas dentro da TAG `<html>`. Exemplo de uso:

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- metadados e informações do documento -->
  </head>
  <body>
    <!-- conteúdo visível da página -->
  </body>
</html>
```

### TAG `<head>`

A TAG `<head>` é usada para incluir metadados e informações sobre o documento HTML. Esses metadados não são exibidos diretamente na página, mas fornecem informações importantes para o navegador e mecanismos de busca. Exemplo de uso:

```html
<head>
  <title>Título da Página</title>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="styles.css">
  <script src="script.js"></script>
</head>
```

### TAG `<body>`

A TAG `<body>` é usada para definir o conteúdo visível de uma página HTML. Todo o conteúdo, como texto, imagens, links e outros elementos, deve ser colocado dentro dessa TAG. Ex:
```html
<body>
  <h1>Título da Página</h1>
  <p>Este é um parágrafo de exemplo.</p>
  <a href="https://www.exemplo.com">Link</a>
  <img src="imagem.jpg" alt="Imagem de exemplo">
</body>
```

### TAGs de Títulos

As TAGs de títulos são usadas para definir os diferentes níveis de títulos em uma página. Os títulos são importantes para a estruturação e organização do conteúdo. Existem seis níveis de títulos, de `<h1>` a `<h6>`, sendo `<h1>` o mais importante e `<h6>` o menos importante. Exemplo de uso:

```html
<h1>Título Nível 1</h1>
<h2>Título Nível 2</h2>
<h3>Título Nível 3</h3>
<h4>Título Nível 4</h4>
<h5>Título Nível 5</h5>
<h6>Título Nível 6</h6>
```

### TAGs de Parágrafos

As TAGs de parágrafos são usadas para exibir texto em parágrafos. O conteúdo dentro dessas TAGs será renderizado como um bloco de texto. Exemplo de uso:

```html
<p>Este é um parágrafo de exemplo.</p>
```

### TAGs de Links

As TAGs de links são usadas para criar links para outras páginas ou recursos da web. O atributo `href` é usado para especificar o URL de destino do link. Exemplo de uso:

```html
<a href="https://www.exemplo.com">Link</a>
```

### TAG `<img>`

A TAG `<img>` é usada para inserir imagens em uma página HTML. O atributo `src` é usado para especificar o caminho da imagem, enquanto o atributo `alt` fornece uma descrição alternativa da imagem. Exemplo de uso:

```html
<img src="imagem.jpg" alt="Imagem de exemplo">
```

### TAG `<div>`

A TAG `<div>` é usada para criar um contêiner genérico que agrupa elementos relacionados. É amplamente utilizada para fins de estilização e estruturação do layout. Exemplo de uso:

```html
<div>
  <p>Conteúdo do div</p>
</div>
```

### TAG `<span>`

A TAG `<span>` é usada para aplicar estilo ou manipular partes específicas de um texto. Ela geralmente é usada dentro de outras TAGs para selecionar uma parte do conteúdo. Exemplo de uso:

```html
<p>Este é um <span style="color: red;">texto destacado</span>.</p>
```

### TAG `<ul>`

A TAG `<ul>` é usada para criar uma lista não ordenada, onde os itens são marcados com pontos ou outros símbolos. Os itens da lista devem ser definidos usando a TAG `<li>`. Exemplo de uso:

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

### TAG `<ol>`

A TAG `<ol>` é usada para criar uma lista ordenada, onde os itens são numerados sequencialmente. Os itens da lista devem ser definidos usando a TAG `<li>`. Exemplo de uso:

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

### TAG `<li>`

A TAG `<li>` é usada para definir um item de lista em uma lista ordenada (`<ol>`) ou uma lista não ordenada (`<ul>`). Cada item de lista deve estar contido dentro da TAG `<li>`. Exemplo de uso:

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

### TAG `<table>`

A TAG `<table>` é usada para criar uma tabela na página HTML. As células da tabela são definidas usando as TAGs `<tr>` (linha da tabela) e `<td>` (célula da tabela). Exemplo de uso:

```html
<table>
  <tr>
    <td>Célula 1</td>
    <td>Célula 2</td>
  </tr>
  <tr>
    <td>Célula 3</td>
    <td>Célula 4</td>
  </tr>
</table>
```

### TAG `<tr>`

A TAG `<tr>` é usada para definir uma linha em uma tabela (`<table>`). As células da linha são definidas usando a TAG `<td>`. Exemplo de uso:

```html
<table>
  <tr>
    <td>Célula 1</td>
    <td>Célula 2</td>
  </tr>
</table>
```

### TAG `<td>`

A TAG `<td>` é usada para definir uma célula em uma tabela (`<table>`). As células contêm o conteúdo da tabela. Exemplo de uso:

```html
<table>
  <tr>
    <td>Célula 1</td>
    <td>Célula 2</td>
  </tr>
</table>
```

### TAG `<form>`

A TAG `<form>` é usada para criar um formulário na página HTML. Os elementos do formulário, como campos de entrada e botões, são definidos dentro da TAG `<form>`. Exemplo de uso:

```html
<form>
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome">
  <input type="submit" value="Enviar">
</form>
```

### TAG `<input>`

A TAG `<input>` é usada para criar um campo de entrada em um formulário. O atributo `type` define o tipo de campo de entrada, como texto, senha, checkbox, entre outros. Exemplo de uso:

```html
<input type="text" id="nome" name="nome">
<input type="password" id="senha" name="senha">
<input type="checkbox" id="aceito" name="aceito">
```

### TAG `<button>`

A TAG `<button>` é usada para criar um botão na página HTML. O conteúdo dentro da TAG `<button>` define o texto exibido no botão. Exemplo de uso:

```html
<button type="button">Clique aqui</button>
```

### TAG `<textarea>`

A TAG `<textarea>` é usada para criar uma área de texto de várias linhas em um formulário. É útil quando se deseja permitir que os usuários insiram um texto mais longo. Exemplo de uso:

```html
<textarea rows="4" cols="50">
Digite seu texto aqui.
</textarea>
```

### TAG `<select>`

A TAG `<select>` é usada para criar uma lista suspensa de opções em um formulário. As opções são definidas usando a TAG `<option>`. Exemplo de uso:

```html
<select>
  <option value="opcao1">Opção 1</option>
  <option value="opcao2">Opção 2</option>
  <option value="opcao3">Opção 3</option>
</select>
```

### TAG `<option>`

A TAG `<option>` é usada para definir uma opção em uma lista suspensa (`<select>`). O atributo `value` define o valor da opção que será enviado ao servidor quando o formulário for enviado. Exemplo de uso:

```html
<select>
  <option value="opcao1">Opção 1</option>
  <option value="opcao2">Opção 2</option>
  <option value="opcao3">Opção 3</option>
</select>
```

## Conclusão

Este guia forneceu uma explicação detalhada das TAGs HTML mais comumente utilizadas, juntamente com suas propriedades e exemplos de uso. Com este conhecimento, você está pronto para começar a criar páginas HTML e estruturar o conteúdo da web de forma eficiente.

Lembre-se de consultar a documentação oficial do HTML para obter informações mais detalhadas e explorar outras TAGs e recursos disponíveis. Divirta-se criando suas páginas web!