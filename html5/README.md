# Aprendendo HTML5
**ATENÇÃO:** Não iremos focar em questões históricas. Embora possamos em algum momento mencionar algo relacionado, a inteção é construir uma base que sirva de referêcia. Não sou o melhor escrítor, então se indentificar erros ortográficos, peço desculpas.

Aqui encontra-se anotações pessoais sobre HTML5. Tentarei atualizar esse repositório com tudo de novo que eu conseguir aprender, e sempre reformulando os arquivos **README.md** para trazer a maior coesão possível.

**Documentação Oficial:** [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)

----

#### Listagem de conteúdo
Aqui você pode clicar rápidamente nos link abaixo e ir para alguma dessas seções.

1. [O que é HTML?](#o-que-é-html?)
2. [Navegadores: O que é um navegador?](#navegadores-o-que-é-um-navegador)
    - [Como um navegador lida com HTML?](#como-um-navegador-lida-com-html)
    - [Como tudo funciona?](#como-tudo-funciona)
3. [Estrutura de um arquivo HTML](#estrutura-de-um-arquivo-html)

## O que é HTML?

Em termos simples, HTML é uma Linguagem de Marcação Hipertextual (HyperText Markup Language). Diferentemente do JavaScript ou Python, o HTML **não é considerado** como uma linguagem de programação, pois não possui a mesma lógica (loops, condicionais, etc). 

> "HTML pode ser comparado à estrutura de uma casa, definindo onde estão as paredes, portas e janelas, enquanto JavaScript é como os móveis e a decoração que dão vida a esse espaço. Sem HTML, não teríamos uma base organizada, mas, sem JavaScript, essa estrutura ficaria vazia e sem interatividade. Juntos, eles criam uma experiência web completa, onde a estrutura é essencial, mas a funcionalidade é o que realmente torna tudo dinâmico e envolvente."
> *Fonte: [ChatGPT](chatgpt.com)*

## Navegadores: O que é um navegador?
Primeiro, imagine-se como um navio cargueiro: você possui vários containers a bordo (dúvidas, necessidades, interesses, etc), mas se você não possuir alguém para conduzi-lo ao destino solicitado, nada acontece.

É isso que aplicativos como [Mozilla FireFox](https://www.mozilla.org/pt-BR/firefox/browsers/what-is-a-browser/), [Google Chrome](https://www.google.pt/intl/pt-PT/chrome/?brand=CHBD&ds_kid=43700076570745610&gad_source=1&gclid=CjwKCAjwx4O4BhAnEiwA42SbVHIwomIZOUbXXWt6MG8skq-cZUMSGZA-Z-RxFMVUrAzi4mHYvNu7zhoCnhsQAvD_BwE&gclsrc=aw.ds), [Microsoft Edge](https://www.microsoft.com/pt-br/edge/download?form=MA13FJ) e [Apple Safari](https://www.apple.com/br/safari/) fazem: eles o conduzem pelo oceano da internet em busca do que você almeja alcançar ou conhecer, fazendo o uso de requisições HTTP ou HTTPS.

##### Como um navegador lida com HTML?
Quando um navegador web encontra um HTML, ele interpreta sua estrutura de cima para baixo. Com base na organização das tags, elementos e atributos usados, definições de estilo e scripts (entre outras coisas), ele renderiza as informações e exibe (imagens, links, parágrafos, vídeos, aúdios, etc) na tela  do computador. Para isso ele conta com um motor (engine), que é responsável por descobrir quais e como renderizar as informações dos arquivos que ele recebeu para que você visualize e interaja com as mesmas.

##### Como tudo funciona?
Como foi dito no exemplo sobre "[O que é um navegador?](#navegadores-o-que-é-um-navegador)", a internet é vasta como um oceano. Ainda assim, quando buscamos por uma URL, vários processos são iniciados com o objetivo final de exibir na tela uma página HTML.

Primeiro o navegador faz uma solicitação para um servidor DNS (Domain Name System) para que a URL seja convertida em um endereço IP. Após isso o navegador estabelece uma conexão com o servidor usando TCP (Transmission Control Protocol).

Com a conexão estabelecida, o navegador começa a fazer requisições HTTP ou HTTPS, pedindo ao servidor acesso aos arquivos necessários para a exibição da página. Em resposta, o servidor começa a enviar de volta os arquivos solicitados. Após todo esse processo, o navegador começa a interpretação e renderização da página.

Voce pode aprender mais sobre HTTP/HTTPS, DNS, TCP nesse link: [Como a Web funciona?: MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/How_the_Web_works)



## Estrutura de um arquivo HTML
Ao criar um novo arquivo ``index.html`` uma mesma estrutura se repete para todos, podendo váriar dependendo do conteúdo que a página planeja oferecer.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Nome da Página</title>
        <!-- Seção de metadados sobre o documento: títulos, links para estilos, scripts... -->

    </head>
    <body>
        <!-- Nesta seção encontra-se toda a parte visual do arquivo: textos, links interativos, imagens, vídeos... -->

    </body>
</html>
```
### !DOCTYPE
Apesar da semelhança, **DOCTYPE** não é uma tag. Na verdade, ``!DOCTYPE html`` é uma **declaração** que diz ao navegador qual a versão do **html** que está sendo usada para a renderização da página.

#### Referências:
- Medium.com: [O que é DOCTYPE e como ele afeta a renderização das páginas?](https://medium.com/@leandrodonascimento/o-que-%C3%A9-doctype-e-como-ele-afeta-a-renderiza%C3%A7%C3%A3o-das-p%C3%A1ginas-ff78f31edf51)