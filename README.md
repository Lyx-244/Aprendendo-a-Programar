# Aprendendo HTML5

---

Neste repositório se encontra uma jornada de aprendizado sobre HTML5, CSS3 e JavaScript. Nele uma documentação se encontrará presente, com informações para quem desejar explorar ou ter alguma referência sobre o assunto.

#### Listagem de conteúdo
1. [Estrutura de um arquivo HTML](#estrutura-de-um-arquivo-html)


## O que é HTML?

A internet é repleta de tecnologias impressionantes, como Python, JavaScript e HTML.

Inicialmente, grandes empresas como YouTube, X (antigo Twitter) e Instagram adotaram o HTML (HyperText Markup Language) na era moderna. Essa linguagem de marcação hipertextual é frequentemente chamada de "site" entre os leigos e é similar ao Markdown. O termo "HyperText" refere-se à capacidade de criar links, conhecidos como HyperLinks, que conectam diferentes referências.

O Markdown, por sua vez, é mais simples e intuitivo, com um processamento menos rigoroso. Isso o torna ideal para documentação  de projetos, especialmente em arquivos README, comuns em sites como GitHub. Em contrapartida, o HTML é mais robusto, permitindo a marcação de diversos elementos, como imagens, links, vídeos, PDFs, parágrafos e títulos.

## Estrutura de um arquivo HTML

Ao criar um novo projeto/arquivo, uma mesma estrutura irá se repetir para todos. Na primeira linha do documento, ``<!DOCTYPE html>`` dirá ao navegador como ele deve representar/lidar como o arquivo, instruindo de forma eficaz que trata-se de um conteúdo html.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Nome da Página</title>
        <!-- Seção de metadados sobre o documento: títulos, links para estilos, scripts... -->

    </head>
    <body>
        <!-- Nesta seção encontra-se toda a parte visual do arquivo: textos, links, imagens, vídeos... -->

    </body>
</html>
```

Após ``<!DOCTYPE html>`` prossegue-se com a(o) tag/elemento ``<html></html>``, sendo considerado como um elemento ancestral (ou uma tag ancestral) que contém ``<head>`` e ``<body>`` como tags/elementos filhos(a). Sempre que uma tag for aberta, deve-se fechá-la escrevendo a mesma tag com uma ``/`` antes do nome.

### Considerações
O conteúdo bruto de todo HTML deve sempre seguir a indentação, facilitando a legibilidade e tornando o seu entendimeto mais intuitivo e eficaz. A indentação funciona como como um quebra-cabeça, se as peças permanecerem espalhadas a imagem não fará sentido, pois encontra-se desconstruida.

##### Indentação Ausente:
```html
<!DOCTYPE html>
<html>
<head>
<title>Página Confusa</title>
<style>
body { background-color: #f0f0f0; }
h1 { color: blue; }
</style>
</head>
<body>
<h1>Bem-vindo</h1><p>Este é um parágrafo.</p>
<p>Outro parágrafo.</p>
<ul><li>Item 1</li><li>Item 2</li>
<li>Item 3</li></ul></body>
</html>
```

##### Indentação Presente:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Página Bem Indentada</title>
    </head>
    <body>
        <h1>Bem-vindo</h1>
        <p>Este é um parágrafo bem indentado.</p>
        <p>Outro parágrafo aqui.</p>
    </body>
</html>
```
