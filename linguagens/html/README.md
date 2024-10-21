# Aprendendo HTML5
**ATENÇÃO:** Não iremos focar em questões históricas. Embora possamos em algum momento mencionar algo relacionado, a inteção é construir uma base que sirva de referêcia. Não sou o melhor escrítor, então se indentificar erros ortográficos, peço desculpas.

Aqui encontra-se anotações pessoais sobre HTML5. Tentarei atualizar esse repositório com tudo de novo que eu conseguir aprender, e sempre reformulando os arquivos **README.md** para trazer a maior coesão possível.

**Documentação Oficial:** [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)

----

#### Listagem de conteúdo
Aqui você pode clicar rápidamente nos link abaixo e ir para alguma dessas seções.

1. [O que é HTML?](#o-que-é-html?)
2. [Navegadores: O que é?](#navegadores-o-que-é)
    - [Como um navegador lida com HTML?](#como-um-navegador-lida-com-html)
    - [Como tudo funciona?](#como-tudo-funciona)
3. [Estrutura de um arquivo HTML](#estrutura-de-um-arquivo-html)
    - [Estrutura base](#estrutura-base)
4. [Componentes do HTML](#componetes-do-html)
    - [Estrutura do documento](#estrutura-do-documento)
        - [!DOCTYPE](#doctype)
        - [HTML](#html)
        - [HEAD](#head)
        - [BODY](#body)

# O que é HTML?

Em termos simples, HTML é uma Linguagem de Marcação Hipertextual (HyperText Markup Language). Diferentemente do JavaScript ou Python, o HTML **não é considerado** como uma linguagem de programação, pois não possui a mesma lógica (loops, condicionais, etc). 

> "HTML pode ser comparado à estrutura de uma casa, definindo onde estão as paredes, portas e janelas, enquanto JavaScript é como os móveis e a decoração que dão vida a esse espaço. Sem HTML, não teríamos uma base organizada, mas, sem JavaScript, essa estrutura ficaria vazia e sem interatividade. Juntos, eles criam uma experiência web completa, onde a estrutura é essencial, mas a funcionalidade é o que realmente torna tudo dinâmico e envolvente."
> *Fonte: [ChatGPT](chatgpt.com)*

# Navegadores: O que é?
Primeiro, imagine-se como um navio cargueiro: você possui vários containers a bordo (dúvidas, necessidades, interesses, etc), mas se você não possuir alguém para conduzi-lo ao destino solicitado, nada acontece.

É isso que aplicativos como [Mozilla FireFox](https://www.mozilla.org/pt-BR/firefox/browsers/what-is-a-browser/), [Google Chrome](https://www.google.pt/intl/pt-PT/chrome/?brand=CHBD&ds_kid=43700076570745610&gad_source=1&gclid=CjwKCAjwx4O4BhAnEiwA42SbVHIwomIZOUbXXWt6MG8skq-cZUMSGZA-Z-RxFMVUrAzi4mHYvNu7zhoCnhsQAvD_BwE&gclsrc=aw.ds), [Microsoft Edge](https://www.microsoft.com/pt-br/edge/download?form=MA13FJ) e [Apple Safari](https://www.apple.com/br/safari/) fazem: eles o conduzem pelo oceano da internet em busca do que você almeja alcançar ou conhecer, fazendo o uso de requisições HTTP ou HTTPS.

## Como um navegador lida com HTML?
Quando um navegador web encontra um HTML, ele interpreta sua estrutura de cima para baixo. Com base na organização das tags, elementos e atributos usados, definições de estilo e scripts (entre outras coisas), ele renderiza as informações e exibe (imagens, links, parágrafos, vídeos, aúdios, etc) na tela  do computador. Para isso ele conta com um motor (engine), que é responsável por descobrir quais e como renderizar as informações dos arquivos que ele recebeu para que você visualize e interaja com as mesmas.

## Como tudo funciona?
Como foi dito no exemplo sobre "[O que é um navegador?](#navegadores-o-que-é-um-navegador)", a internet é vasta como um oceano. Ainda assim, quando buscamos por uma URL, vários processos são iniciados com o objetivo final de exibir na tela uma página HTML.

Primeiro o navegador faz uma solicitação para um servidor DNS (Domain Name System) para que a URL seja convertida em um endereço IP. Após isso o navegador estabelece uma conexão com o servidor usando TCP (Transmission Control Protocol).

Com a conexão estabelecida, o navegador começa a fazer requisições HTTP ou HTTPS, pedindo ao servidor acesso aos arquivos necessários para a exibição da página. Em resposta, o servidor começa a enviar de volta os arquivos solicitados. Após todo esse processo, o navegador começa a interpretação e renderização da página.

Voce pode aprender mais sobre HTTP/HTTPS, DNS, TCP nesse link: [Como a Web funciona?: MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/How_the_Web_works)



# Estrutura de um arquivo HTML
A estrutura de um arquivo HTML é simples como um esqueleto, onde cada osso tem seu lugar e função. Ainda assim, o que permanece no topo é o crânio, mas o que poderia ser o crânio de um ``index.html``?

#### Estrutura base:

Por mais que a base seja apenas:
```html
<!DOCTYPE html>
<html>
    <head>
        <!-- Metadados -->
    </head>
    <body>
        <!-- Conteúdo -->
    </body>
</html>
```

Geralmente você irá escrever:

```html
<!DOCTYPE html>     <!-- Indica o tipo do documento e a versão do HTML, nesse caso HTML5 -->
<html lang="pt-br"> <!-- Idioma ao qual está sendo escrito -->
    <head>
        <meta charset="UTF-8">  <!-- Usada para exibir a codificação de caractesres na página: sem isso caracteres especiais (acentos, emojis, letras de outros alfabetos) podem sofrer com erros de exibição -->
        <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Usado para responsívidade em diferentes telas, principalmente em telas mobile -->
        <link rel="stylesheet" href="seu-arquivo.css"> <!-- Usado para linkar uma folha de estilo (css) a página  -->

        <title>Nome da página</title> <!-- Isso será exibido na guia do seu navegador -->
        <!--
        Aqui se encontra metadados sobre a página, contendo conteúdo e informações que será usado, mas não exibido explicitamente na interface do usuário:
        <title>, <meta>, <link>, <script>, <syle>, <base>..
         -->

    </head>
    <body>
        <!--
        Aqui vai todo conteúdo que será visível na página:
        links, imagens, vídeos, textos, cores..
         -->
    </body>
</html>
```
# Componetes do HTML
**Atenção:** Quando encontrar ``<!-- comentário -->`` no exemplo de código, significa que você está lendo um comentário em HTML. Um comentário é uma linha que não é exibida no navegador, servindo para auxiliar desenvolvedores que possam trabalhar no mesmo projeto, podendo ser úteis tanto para você mesmo quanto para outra pessoa.

Agora vamos nos aprofundar um pouco mais. Falaremos a respeito de tags, atributos, como funciona e como se usa.

## Estrutura do documento

#### !DOCTYPE
Assim como eu costumava pensar, muitos acreditam que ``doctype`` é uma tag, quando na verdade, ela é uma declaração que serve para dizer ao navegador a versão do HTML em que o tipo de arquivo está sendo executado.

Atualmente, desde 2014 quando o HTML5 foi desenvolvido, as versões anteriores teem sido descontinuadas por possuirem uma sintaxe mais complexa. A versão cinco do html veio com o próposito de simplificar a linguagem e tornala mais intuitiva, pois antes disso existiam diferentes versões do html e diferentes formas de escrever a mesma declaração.

```html
<!DOCTYPE html> <!-- Arquivo: .html; Versão: HTML5 -->

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"> <!-- Arquivo: .html; Versão: HTML 4.01 Strict -->

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"> <!-- Arquivo: .html; Versão: HTML 4.01 Transitional -->

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd"> <!-- Arquivo: .html; Versão: HTML 4.01 Frameset -->

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2//EN"> <!-- Arquivo: .html; Versão: HTML 3.2 -->

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd"> <!-- Arquivo: .html; Versão: XHTML 1.0 Strict -->

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> <!-- Arquivo: .html; Versão: XHTML 1.0 Transitional -->

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd"> <!-- Arquivo: .html; Versão: XHTML 1.0 Frameset -->

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd"> <!-- Arquivo: .html; Versão: XHTML 1.1 -->

```
Como pôde observar, ``doctype`` no HTML5 é o mais simples de todas as declarações, sem falar que hoje em dia todos usam a versão cinco do html. Sinceramente, estou agradecido por ter começado meu estudo de html após a sua quinta versão. 😊😊😊

#### Sintaxe:
Sempre que você for desenvolver uma página HTML, precisarar declarar ``doctype`` no topo do arquivo. Isso deve ser feito antes de qualquer tag, mas como?

Para declarar ``doctype``, escreva sem seu arquivo da seguinte forma:

```html
<!DOCTYPE html>
```
Lembrando que ``doctype`` é **case sensitivity**, então não importa se você escrever com maiúscula, minúscula ou as duas formas juntas, vai funcionar da mesma forma.

```html
<!DOCTYPE html>
<!doctype HTML>
<!DOCTYPE HTML>
<!doctype html>
```

A exclamação em ``doctype`` serve para indicar ao navegador que o que se segue é uma declaração de tipo de documento, facilitando a identificação imediata.

---

#### HTML
Após inserir ``doctype`` no seu arquivo, será necessário colocar obrigatoriamente três tags para que possamos começar a desenvolver a página. Assim, podemos dizer que, após declarar que trata-se de um ``index.html`` na versão cinco, ``<html></html>`` é o primordio de seu arquivo, explicitando, através da tag de abertura e fechamento, onde sua página começa e termina.

Mas o que seria uma tag de abertura e fechamento? Vamos aprender neste momento, e não se preocupe, é mais simples que um jogo de xadrez.

#### Sintaxe:
Para escrever a primeira e mais importanto tag do html, basta digitar ``html`` entre o sinal de menor que (<) e maior que (>):

```html
<html>  <!-- Tag de abertura -->
```
Essa é uma tag de abertura, mas para que ela funcione corretamente, é necessário fecha-la com uma tag de fechamento. Para isso, basta escrever a mesma tag de abertura, com a exceção de que deve-se colocar uma ``/`` antes do nome do elemento:

```html
<html></html>   <!-- Tag de fechamento -->
```

---

#### Boas práticas:
Assim como qualquer elemento, ``html`` pode ter atributos. A única diferença é que algumas tags não tem uma obrigação restrita em relação a isso, enquanto outras precisam de um atributo específico para seu total funcionamento.

``html`` possui três atributos, mas apenas um é utilizado, enqaunto outro é mais específico para idiomas que são lidos da direita para esquerda. O último não é mais necessário no HTML5.

```html
<html lang="pt-br"></html>  <!-- Usado para SEO (Search Engine Optimization); muito útil para a tradução autommática do navegador. -->

<html dir="rtl"></html>     <!-- Usado para especificar a direção em que o texto deve ser organizado e lido. -->

<html xmlns="http://www.w3.org/1999/xhtml"></html>     <!-- Desnecessário no HTML5-->
```

---

#### HEAD
O ``head`` é o cabeçalho do seu ``index.html``. A tradução literal de head para português é **cabeça**, e em um contexto de escrita e línguagem, pode ser interpretado como **cabeçalho**.

Em outras palavras, o ``head`` é a cabeça do seu arquivo, onde os "pensamentos e ideias" costumam ficar, diferente do body que está mais associado ao movimento e realização em si. Mas o que seria esses "pensamentos"?

Os pensamentos que podem residir no ``head`` são metadados que fazem o seu arquivo funcionar de uma forma mais refinada. Esse metadados não são visíveis no navegador (títulos, links para css e scripts, fontes tipográficas, servidores), mas etão lá com toda certeza. Você pode usar a função "inspecionar" (DevTools) do seu navegador e ver o ``head`` de algum site que você visita com frequência.

Por exemplo:

```html
<meta charset="UTF-8">  <!-- Função: auxiliar o navegador na interpretação de caracteres especiais. -->
```

O ``meta`` pode ser usados de outras formas, mas nesse caso em específico, ela fornece ao navegador auxílio para que ele interprete caracteres especiais de maneira correta. Alguns exemplos: ã, á, ê, ç, etc.

É como se ``meta charset="UTF-8"`` estivesse ao lado do navegador dizendo o que é cada um dos caracteres especiais. Sem isso a palavra "ação" poderia ser exibida dessa forma: Ã§Ã£o

Mas isso é algo que depende muito. O ponto é que sem ``meta charset="UTF-8"``, a exibição não é garantida, podendo funcionar bem para nós mesmo, e incorretamente para outra pessoa.

---

#### BODY
Diferentemente do ``head``, o ``body`` lida com tudo que será exibido no corpo do navegador. Não é à toa que **corpo** é a tradução literal de body para português.

> Em outras palavras, o ``head`` é a cabeça do seu arquivo, onde os "pensamentos e ideias" costumam ficar, diferente do body que está mais associado ao movimento e realização em si.
>*Fonte: [Head](#head)*

Sendo assim, mesmo que não seja uma tag escrita corretamente, qualquer coisa que você coloque será exibido na tela, desde que você siga a [estrutura base](#estrutura-base) do HTML:

```html
<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <title>Escrevendo no body</title>
    </head>
    <body>
        Aqui vai sua mensagem!
        <p>Não precisa escrever uma tag para textos simples.</p>

        <div>
            Ainda assim, existem exceções.
            Uma div não será visível, a menos que você mude o background com CSS ou usando style.

            Falaremos sobre divs mais para frente.

            <style>
                /* A tag style pode ser usada tanto no head quanto no body, ou até mesmo como um atributo, mas isso é assunto para outro momento. */
                div {
                    background-color: blue;
                }
            </style>
        </div>

        Pode copiar o código se quiser visualizar como fica no navegador.
    </body>
</html>
```
Um peqeuno exercício prático: [Crie a estrutura básica](#estrutura-de-um-arquivo-html) do HTML, depois crie no ``body`` o ``h1`` e ``p`` seguindo a lógica de abertura e fechamento falado na [sintaxe do html](#html). Faça sem ver a resposta, e quando terminar, acesse essa documentão sobre [h1](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Heading_Elements) e [p](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/p).

Você deve visualizar algo assim:
![Imagem de exemplo](images/image-1.png)