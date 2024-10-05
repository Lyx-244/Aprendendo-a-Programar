# Aprendendo HTML5

Aqui encontra-se anotações pessoais sobre html5. Tentarei atualizar esse repositório com tudo de novo que eu conseguir aprender, e sempre reformulando os arquivos README.md para trazer a maior coesão possível.

**ATENÇÃO:** Não iremos focar em questões históricas, embora possamos em algum momento mencionar algo relacionado. A inteção é construir uma base que sirva de referêcia.

**Documentação Oficial:** [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)

#### Listagem de conteúdo
1. [O que é HTML?](#o-que-é-html?)
2. [Navegadores: O que é? Como eles lidam com HTML?](#navegadores-o-que-é-como-eles-lidam-com-html)
    - [O que é HTTP e HTTPS?](#o-que-http-e-https)
    - [Como eles lidam com o HTML?](#como-eles-lidam-com-o-html)
3. [Estrutura de um arquivo HTML](#estrutura-de-um-arquivo-html)


## O que é HTML?

Em termos simples, HTML é uma Linguagem de Marcação Hipertextual (HyperText Markup Language). Diferentemente do JavaScript ou Python, o HTML **não é conciderado** como uma linguagem de programação, pois não possui a mesma lógica (loops, condicionais, etc). 

> "HTML pode ser comparado à estrutura de uma casa, definindo onde estão as paredes, portas e janelas, enquanto JavaScript é como os móveis e a decoração que dão vida a esse espaço. Sem HTML, não teríamos uma base organizada, mas, sem JavaScript, essa estrutura ficaria vazia e sem interatividade. Juntos, eles criam uma experiência web completa, onde a estrutura é essencial, mas a funcionalidade é o que realmente torna tudo dinâmico e envolvente."
> Fonte: [ChatGPT](chatgpt.com)

## Navegadores: O que é? Como eles lidam com HTML?
Imagine um que você é um barco. Você possui espaço para/e carga para levar para um destino, mas sem um condutor para o leme nada acontece, pois você é apenas um barco. Não vai chegar a lugar algum sozinho.

É isso que aplicativos como [Mozilla FireFox](https://www.mozilla.org/pt-BR/firefox/browsers/what-is-a-browser/), [Google Chrome](https://www.google.pt/intl/pt-PT/chrome/?brand=CHBD&ds_kid=43700076570745610&gad_source=1&gclid=CjwKCAjwx4O4BhAnEiwA42SbVHIwomIZOUbXXWt6MG8skq-cZUMSGZA-Z-RxFMVUrAzi4mHYvNu7zhoCnhsQAvD_BwE&gclsrc=aw.ds), [Microsoft Edge](https://www.microsoft.com/pt-br/edge/download?form=MA13FJ) e [Apple Safari](https://www.apple.com/br/safari/) fazem, eles conduzem para aquilo que você almeja alcançar ou conhecer, fazendo o uso de requisições HTTP ou HTTPS.

#### O que HTTP e HTTPS?
Quando falamos de *HyperText Transfer Protocol* (HTTP), queremos dizer **Protocolo de Transferência de Hipertexto**; quando falos de *HyperText Transfer Protocol Secure* (HTTPS), queremos dizer **Protocolo de Transferência de Hipertexto Seguro**.

> "O protocolo de transferência de hipertexto (HTTP) é um protocolo ou conjunto de regras de comunicação para comunicação entre cliente e servidor. Quando você visita um site, o navegador envia uma solicitação HTTP ao servidor Web, que responde com uma resposta HTTP. O servidor Web e o navegador trocam dados como texto simples. Resumindo, o protocolo HTTP é a tecnologia subjacente que alimenta a comunicação de rede. Como o nome sugere, o protocolo de transferência de hipertexto seguro (HTTPS) é uma versão mais segura ou uma extensão do HTTP. No HTTPS, o navegador e o servidor estabelecem uma conexão segura e criptografada antes de transferir dados."
> Fonte: [aws.amazon.com](https://aws.amazon.com/pt/compare/the-difference-between-https-and-http/#:~:text=O%20protocolo%20de%20transfer%C3%AAncia%20de,responde%20com%20uma%20resposta%20HTTP.)

#### Como eles lidam com o HTML?
Quando um navegador web encontra um HTML, ele interpreta sua estrutura de cima para baixo. Com base na organização das tags, elementos e atributos usados, definições de estilo e scripts (entre outras coisas), ele renderiza as informações e exibe (imagens, links, parágrafos, vídeos, aúdios, etc) na tela  do computador. Para isso ele conta com um motor (engine), que é responsável por descobrir quais e como renderizar as informações dos arquivos que ele recebeu para que você visualize e interaja com as mesmas.

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