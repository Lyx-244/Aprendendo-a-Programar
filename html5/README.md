# Aprendendo HTML5

Aqui encontra-se anotações pessoais sobre html5. Tentarei atualizar esse repositório com tudo de novo que eu conseguir aprender, e sempre reformulando os arquivos README.md para trazer a maior coesão possível.

**ATENÇÃO:** Não iremos focar em questões históricas, embora possamos em algum momento mencionar algo relacionado. A inteção é construir uma base que sirva de referêcia.

**Documentação Oficial:** [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)

#### Listagem de conteúdo
1. [O que é HTML?](#o-que-é-html?)
2. [Estrutura de um arquivo HTML](#estrutura-de-um-arquivo-html)


## O que é HTML?

Em termos simples, HTML é uma Linguagem de Marcação Hipertextual (HyperText Markup Language). Diferentemente do JavaScript ou Python, o HTML **não é conciderado** como uma linguagem de programação, pois não possui a mesma lógica (loops, condicionais, etc). 

Para compreender melhor, acompanhe o exemplo tirado do [ChatGPT](chatgpt.com):

"HTML pode ser comparado à estrutura de uma casa, definindo onde estão as paredes, portas e janelas, enquanto JavaScript é como os móveis e a decoração que dão vida a esse espaço. Sem HTML, não teríamos uma base organizada, mas, sem JavaScript, essa estrutura ficaria vazia e sem interatividade. Juntos, eles criam uma experiência web completa, onde a estrutura é essencial, mas a funcionalidade é o que realmente torna tudo dinâmico e envolvente."

#### Referências:
- Devmedia.com.br: [O que é o HTML5](https://www.devmedia.com.br/o-que-e-o-html5/25820)

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