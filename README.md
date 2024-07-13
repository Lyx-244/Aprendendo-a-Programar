# Guia de Referência de Tags HTML

Este arquivo contém uma lista de tags HTML e suas respectivas descrições para facilitar a consulta durante a programação.

#### Tabela de Conteúdo
1. [Tags de Estrutura](#tags-de-estrutura)

## Estrutura Básica do HTML
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="caminho/para/style.css"> <!-- Importa o CSS -->
    <title>Título da Página</title>
</head>
<body>
    <!-- Conteúdo da página -->
</body>
</html>
```

## Tags de Estrutura
#### Header
O elemento HTML `<header>` representa um grupo de suporte introdutório ou navegacional. Pode conter alguns elementos de cabeçalho mas também outros elementos como um logo, seções de cabeçalho, formulário de pesquisa, e outros.

#### H1, H2, H3, H4, H5, H6
Os **elementos HTML** `<h1>`—`<h6>` representam seis níveis de título de seção. `<h1>` é o nível de seção mais baixo e `<h6>` é o mais baixo.

#### Main
O elemento `<main>` define o conteúdo principal dentro do `<body>` em seu documento ou aplicação. Entende-se como conteúdo principal aquele relacionado diretamente com o tópico central da página ou com a funcionalidade central da aplicação. O mesmo deverá ser único na página, ou seja, dentro do elemento `<main>` não deverá ser incluidas seções da página que sejam comuns a todo site ou aplicação, tais como mecanismo de navegação, informações de copyright, logotipo e campos de busca (a não ser, é claro, caso a função principal do documento seja fazer algum tipo de busca).

#### Nav
O Elemento HTML de Navegação (`<nav>`) representa uma seção de uma página que aponta para outras páginas ou para outras áreas da página, ou seja, uma seção com links de navegação.

#### Section
O elemento HTML `<section>` representa uma seção genérica contida em um documento HTML, geralmente com um título, quando não existir um elemento semântico mais específico para representá-lo.
