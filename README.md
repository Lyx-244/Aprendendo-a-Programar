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
#### Addres
O elemento HTML `<address>` fornece informações de contato para seu ancestral `<article>` ou `<body>` mais próximo; no segundo caso, ele se aplica ao documento inteiro.

#### Article
O Elemento HTML Article (`<article>`) representa uma composição independente em um documento, página, aplicação, ou site, ou que é destinado a ser distribuido de forma independente ou reutilizável, por exemplo, em sindicação. Este poderia ser o post de um fórum, um artigo de revista ou jornal, um post de um blog, um comentário enviado por um usuário, um gadget ou widget interativos, ou qualquer outra forma de conteúdo independente.

#### Aside
O elemento HTML `<aside>` representa uma seção de uma página que consiste de conteúdo que é tangencialmente relacionado ao conteúdo do seu entorno, que poderia ser considerado separado do conteúdo. Essas seções são, muitas vezes, representadas como barras laterais. Elas muitas vezes contem explicações laterais, como a definição de um glossário; conteúdo vagamente relacionado, como avisos; a biografia do autor; ou, em aplicações web, informações de perfil ou links de blogs relacionados.

#### Footer
O elemento HTML de Rodapé (`<footer>`) representa um rodapé para o seu sectioning content (conteúdo de seção) mais próximo ou sectioning root elemento (ou seja, seu parente mais próximo `<article>`, `<aside>`, `<nav>`, `<section>`, `<blockquote>`, `<body>`, `<details>`, `<fieldset>`, `<figure>`, `<td>`). Normalmente um rodapé contém informações sobre o autor da seção de dados, direitos autorais ou links para documentos relacionados.

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
