# Passo a passo: Principais formas de utilizar o CSS

## Formas de Utilizar CSS:

### CSS Inline:

CSS inline envolve a aplicação de estilos diretamente nos elementos HTML usando o atributo style.

Exemplo: 
```<p style="color: red;">Texto vermelho</p>```

### CSS Interno:

-CSS interno- envolve a inserção de estilos diretamente na seção ```<style>``` dentro da tag ```<head>``` do documento HTML.
Exemplo, como:
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset='utf-8'>
        <title>CSS Interno</title>
        <style>
        p {
        color: blue;
        }
    </style>
    </head>
    <body>
        <p>Texto para ficar azul</p>
    </body>
</html>
```

### CSS Externo:

CSS externo envolve a criação de um arquivo CSS separado e a vinculação a ele no documento HTML usando a tag ```<link>```.
Exemplo

```
<html>
    <head>
        <meta charset='utf-8'>
        <title>CSS Externo</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <p>Conteúdo do Site deve estar aqui</p>
    </body>
</html>
```

## Seletores CSS:

Existe diferentes tipos de seletores CSS, ou seja, uma forma de manipular as TAGS ```HTML`` de meu site. São eles:

- Seletor de elemento: 

    ```
    p { 
        color: red; 
    }
    ```

- Seletor de classe: 

    ```
    .destaque { 
        font-weight: bold; 
    }
    ```

- Seletor de ID: 

    ```
    #titulo { 
        font-size: 24px; 
    }
    ```

- Seletor de atributo: 

    ```
    input[type="text"]{ 
        border: 1px solid gray; 
    }
    ```