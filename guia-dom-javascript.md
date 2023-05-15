# Guia de Manipulação do DOM com JavaScript

Este guia detalhado aborda todas as funcionalidades essenciais para a manipulação do DOM (Document Object Model) utilizando JavaScript. O DOM é uma interface de programação que permite interagir com os elementos HTML de uma página web. Vamos explorar diversas técnicas para manipular e atualizar elementos do DOM.

## Índice

1. Seleção de Elementos
   - Selecionando pelo ID do Elemento
   - Selecionando por Tag ou Classe
   - Selecionando Elementos Aninhados
   - Selecionando Elementos por Seletor CSS

2. Modificação de Elementos
   - Alterando o Conteúdo de um Elemento
   - Alterando os Atributos de um Elemento
   - Adicionando ou Removendo Classes
   - Alterando Estilos CSS

3. Manipulação de Eventos
   - Adicionando Event Listeners
   - Removendo Event Listeners
   - Eventos de Mouse
   - Eventos de Teclado

4. Trabalhando com Elementos Pai/Filho
   - Acessando Elementos Pai
   - Acessando Elementos Filho
   - Navegando entre Elementos Irmãos

5. Manipulação de Elementos
   - Criando Novos Elementos
   - Inserindo Elementos no DOM
   - Removendo Elementos do DOM
   - Clonando Elementos

6. Trabalhando com Formulários
   - Obtendo Valores dos Campos
   - Alterando Valores dos Campos
   - Validando Campos

7. Manipulação de Estilos
   - Obtendo Estilos Computados
   - Alterando Estilos em Tempo Real
   - Animando Elementos

## 1. Seleção de Elementos

### Selecionando pelo ID do Elemento

Para selecionar um elemento pelo ID, utilize o método `getElementById`:

```javascript
const element = document.getElementById('nome-do-elemento');
```

### Selecionando por Tag ou Classe

Para selecionar elementos por tag ou classe, utilize os métodos `getElementsByTagName` e `getElementsByClassName`, respectivamente:

```javascript
const elementsByTag = document.getElementsByTagName('tag');
const elementsByClass = document.getElementsByClassName('nome-da-classe');
```

### Selecionando Elementos Aninhados

Para selecionar elementos aninhados, utilize o método `querySelector` ou `querySelectorAll`, passando um seletor CSS:

```javascript
const element = document.querySelector('#id .classe');
const elements = document.querySelectorAll('.classe');
```

### Selecionando Elementos por Seletor CSS

Para selecionar elementos com base em um seletor CSS, utilize o método `querySelector` ou `querySelectorAll`:

```javascript
const element = document.querySelector('seletor-css');
const elements = document.querySelectorAll('seletor-css');
```

## 2. Modificação de Elementos

### Alterando o Conteúdo de um Elemento

Para alterar o conteúdo de um elemento, você pode modificar a propriedade `innerHTML` ou `textContent`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.innerHTML = 'Novo conteúdo';
element.textContent = 'Novo conteúdo';
```

### Alterando os Atributos de um Elemento

Para alterar os atributos de um elemento, utilize o método `setAttribute`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.setAttribute('atributo', 'valor');
```

### Adicionando ou Removendo Classes

Para adicionar uma classe a um elemento, utilize o método `classList.add`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.classList.add('nome-da-classe');
```

Para remover uma classe de um elemento, utilize o método `classList.remove`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.classList.remove('nome-da-classe');
```

### Alterando Estilos CSS

Para alterar estilos CSS de um elemento, você pode modificar as propriedades diretamente ou utilizar o método `style`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.style.color = 'red';
element.style.fontSize = '16px';
```

## 3. Manipulação de Eventos

### Adicionando Event Listeners

Para adicionar um event listener a um elemento, utilize o método `addEventListener`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.addEventListener('evento', funçãoCallback);
```

### Removendo Event Listeners

Para remover um event listener de um elemento, utilize o método `removeEventListener`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.removeEventListener('evento', funçãoCallback);
```

### Eventos de Mouse

Existem diversos eventos de mouse que você pode utilizar, como:

- `click`: acionado quando o elemento é clicado.
- `mouseover`: acionado quando o mouse é movido sobre o elemento.
- `mouseout`: acionado quando o mouse deixa o elemento.
- `mousedown`: acionado quando o botão do mouse é pressionado sobre o elemento.
- `mouseup`: acionado quando o botão do mouse é liberado após ter sido pressionado sobre o elemento.

```javascript
const element = document.getElementById('nome-do-elemento');

element.addEventListener('click', funçãoCallback);
element.addEventListener('mouseover', funçãoCallback);
element.addEventListener('mouseout', funçãoCallback);
element.addEventListener('mousedown', funçãoCallback);
element.addEventListener('mouseup', funçãoCallback);
```

### Eventos de Teclado

Existem diversos eventos de teclado que você pode utilizar, como:

- `keydown`: acionado quando uma tecla é pressionada.
- `keyup`: acionado quando uma tecla é liberada após ter sido pressionada.
- `keypress`: acionado quando uma tecla é pressionada e solta.

```javascript
const element = document.getElementById('nome-do-elemento');

element.addEventListener('keydown', funçãoCallback);
element.addEventListener('keyup', funçãoCallback);
element.addEventListener('keypress', funçãoCallback);
```

## 4. Trabalhando com Elementos Pai/Filho

### Acessando Elementos Pai

Para acessar o elemento pai de um elemento, utilize a propriedade `parentNode`:

```javascript
const element = document.getElementById('nome-do-elemento');
const parentElement = element.parentNode;
```

### Acessando Elementos Filho

Para acessar os elementos filhos de um elemento, utilize as propriedades `childNodes` ou `children`:

```javascript
const element = document.getElementById('nome-do-elemento');
const childNodes = element.childNodes;
const children = element.children;
```

### Navegando entre Elementos Irmãos

Para navegar entre elementos irmãos, utilize as propriedades `previousSibling`, `nextSibling`, `previousElementSibling` e `nextElementSibling`:

```javascript
const element = document.getElementById('nome-do-elemento');
const previousSibling = element.previousSibling;
const nextSibling = element.nextSibling;
const previousElementSibling = element.previousElementSibling;
const nextSibling = element.nextElementSibling;
```

## 5. Manipulação de Elementos

### Criando Novos Elementos

Para criar um novo elemento, utilize o método `createElement`:

```javascript
const newElement = document.createElement('tag');
```

### Inserindo Elementos no DOM

Para inserir um elemento no DOM, utilize os métodos `appendChild`, `insertBefore` ou `insertAdjacentElement`:

```javascript
const parentElement = document.getElementById('nome-do-elemento-pai');
const childElement = document.getElementById('nome-do-elemento-filho');

parentElement.appendChild(newElement); // Insere como último filho
parentElement.insertBefore(newElement, childElement); // Insere antes de um elemento específico
parentElement.insertAdjacentElement('position', newElement); // Insere em uma posição específica: 'beforebegin', 'afterbegin', 'beforeend', 'afterend'
```

### Removendo Elementos do DOM

Para remover um elemento do DOM, utilize o método `remove`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.remove();
```

### Clonando Elementos

Para clonar um elemento, utilize o método `cloneNode`:

```javascript
const element = document.getElementById('nome-do-elemento');
const clonedElement = element.cloneNode(true); // true para clonar também os filhos, false para clonar somente o elemento
```

## 6. Trabalhando com Formulários

### Obtendo Valores dos Campos

Para obter o valor de um campo de formulário, utilize a propriedade `value`:

```javascript
const inputElement = document.getElementById('nome-do-input');
const valor = inputElement.value;
```

### Alterando Valores dos Campos

Para alterar o valor de um campo de formulário, atribua um novo valor à propriedade `value`:

```javascript
const inputElement = document.getElementById('nome-do-input');
inputElement.value = 'novo valor';
```

### Validando Campos

Para validar um campo de formulário, utilize a propriedade `validity` para acessar os diferentes estados de validação:

```javascript
const inputElement = document.getElementById('nome-do-input');

if (inputElement.validity.valid) {
  // campo válido
} else {
  // campo inválido
}
```

## 7. Manipulação de Estilos

### Obtendo Estilos Computados

Para obter os estilos computados de um elemento, utilize o método `getComputedStyle`:

```javascript
const element = document.getElementById('nome-do-elemento');
const styles = getComputedStyle(element);
const color = styles.color;
const fontSize = styles.fontSize;
```

### Alterando Estilos em Tempo Real

Para alterar os estilos de um elemento em tempo real, utilize a propriedade `style`:

```javascript
const element = document.getElementById('nome-do-elemento');
element.style.color = 'red';
element.style.fontSize = '16px';
```

### Animando Elementos

Para animar elementos, você pode utilizar CSS ou bibliotecas/frameworks como CSS3 Transitions, CSS3 Animations, jQuery, entre outros.

Este guia abrange as principais funcionalidades para manipulação do DOM com JavaScript. Com essas técnicas, você pode interagir e atualizar elementos do DOM de forma dinâmica e personalizada. Experimente e explore esses recursos para criar interações ricas e intuitivas em suas páginas web.