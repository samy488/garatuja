# ia26-webdesign

esta materia foca em desenvolvimento de habilidades para criar sites desde sua estrutura(html) até sua interface(css) focando principalmente em criar habilidades do zero para futuros sites.

## HTML - HyperText Markup Language (Linguagem de Marcação de Hipertexto)

html é uma linguagem de marcação, mas mais do que isso é uma linguagem da estrutura de um site, como texto, estilo e até oque cada parte significa para o computador e para todo tipo de pessoa com suas marcaçoes. O html usa diversas ferramentas para representar oque cada parte estrutura de um site, `<h1>` por exemplo é usado para titulos principais , `<p>` para parágrafos, `<a>` para links, entre outros. O HTML também permite incluir atributos para suas marcaçoes representadas por tags para fornecer informações adicionais sobre os elementos, como `class`, `id`, `src`, etc.

em editores de textos comuns costuma-se usar ferramentas que permitem mudar ou destacar partes do texto deixando em negrito, italico ou em qualquer fonte possivel, O HTML é a linguagem que permite isso acontecer usando das tags para indicar a mundança desejada, sendo que a construsão é composta por tags (etiquetas) de abertura e fechamento, a etiqueta de abertura é representadapor colchtes fechados abertos e fechados`< >` e a etiqueta de fechamento é escrita da mesma forma, mas com uma barra `/` antes do nome da tag. Por exemplo, para criar um parágrafo em HTML, você usaria a tag `<p>` para abrir o parágrafo e `</p>` para fechá-lo. O conteúdo do parágrafo seria colocado entre essas duas tags.



vamos usar a frase `eu amo roxo mais doque tudo` como exemplo 

1. para destacar uma palavra em negrito em html deve se usar a tag `strong` usando `<strong>`pra abrir `</strong>` indicando que entre  elas sera em negrito, assim deve-se colocar a palavra ou frase especifica entre essas tags como a seguir `<strong>eu amo</strong> roxo mais doque tudo` para deixar apenas `eu amo`em destaque
2. usando o texto anterior podemos usar marcaçoes diferentes para marcar partes diferentes de um mesmo texto, o italico é uma delas, para indicar que algo está em italico em um texto de `html` deve se usar a tag `em` usando `<em>` para abrir  `</em>` para fechar e depois colocar a parte do texto que quer como a seguir `<strong>eu amo</strong> roxo mais <em>doque tudo</em>` assim apenas `eu amo`está em negrito e `doque tudo` em italico.
3. agora ira selecionar uam parte da frase e destacar em roxo
  -para fazer isso em html deve pegar uma terceira tag que não tem uma função especifaca como `span`ou `div`para essa função e dentro dela aplicar `style="color: purple;"` e aplicar em sua palavra, dessa forma: `<strong> eu amo</strong><span style="color:purple;">roxo mais</span><em>doque tudo</em>`tag `<span>` é usada para aplicar estilos específicos a um trecho de texto, e o atributo `style` é usado para definir a cor do texto como roxo.

> **⚠️ Nota:**
>
> O HTML é uma linguagem de marcação, e seu principal objetivo é estruturar o conteúdo de uma página web. Caso pesquise na internet, notará que existem outras tags para aplicar formatações como negrito e itálico, como `<b>` e `<i>`, respectivamente. No entanto, as tags `<strong>` e `<em>` são consideradas mais semânticas, pois indicam a importância do texto, enquanto as tags `<b>` e `<i>` são puramente de formatação visual. Portanto, é recomendado usar as tags semânticas para melhorar a acessibilidade e a compreensão do conteúdo.
>
> `<strong>` e `<em>` fazem sentido tanto para leitores sem deficiência quanto para leitores com deficiência, pois indicam a importância do texto, enquanto `<b>` e `<i>` são puramente de formatação visual e podem não ser interpretados corretamente por leitores de tela ou outros dispositivos assistivos.

Esta é a sintaxe básica do HTML, e existem muitas outras tags e atributos que podem ser usados para criar páginas web mais complexas e interativas. A sugestão de como aprender HTML é desenhar a estrutura de uma página web em um papel, identificando os diferentes elementos e suas relações, sempre se perguntando qual tag HTML seria mais adequada para representar cada elemento. Em seguida, você pode começar a escrever o código HTML correspondente, usando as tags apropriadas para estruturar o conteúdo da página. Lembre-se de que a prática é fundamental para aprender HTML, então experimente criar diferentes tipos de páginas web e explore as diversas tags e atributos disponíveis.

### Estrutura básica de um documento HTML

Outro ponto importante a ser abordado é a estrutura básica de um documento HTML. Todo documento HTML deve começar com a declaração do tipo de documento `<!DOCTYPE html>`, que informa ao navegador que o documento é um arquivo HTML5. Em seguida, o documento é estruturado em duas partes principais: o `<head>` e o `<body>`.

O `<head>` é a seção do documento onde são incluídas informações sobre a página, como o título, links para arquivos CSS, scripts JavaScript, meta tags (metainformações), entre outros. O conteúdo do `<head>` não é exibido diretamente na página ouseja usarios comuns não teram acesso a essa estrutura, mas é essencial para o funcionamento e a aparência da página web.

O `<body>` é a seção do documento onde o conteúdo visível da página é colocado. É aqui que você adiciona os elementos HTML que compõem a estrutura e o conteúdo da página, como títulos, parágrafos, imagens, links etc. O conteúdo do `<body>` é o que os usuários veem quando acessam a página web.

# charset, lang e title 
esses atrubutos inicam o tipo de lingua que o html deve usar, assim ele entende que tipos de letras e de simbulos deve ter acesso, `charset="UTF-8" tem acesso a todos os characteres mundiais e lang="pt-BR" e lang="pt-BR"> significa a linguagem principal de um texto. por ultimo title é o nome pagina em uma aba de computador.


A estrutura básica de um documento HTML pode ser representada da seguinte forma:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <title>Título da Página</title>
   <!-- Links para arquivos CSS e scripts JavaScript podem ser adicionados aqui -->
</head>
<body>
   <!-- Conteúdo visível da página é adicionado aqui -->
</body>
</html>
```

### Atributos HTML

Os atributos HTML são usados para fornecer informações adicionais sobre os elementos HTML. Eles são escritos dentro da tag de abertura de um elemento e consistem em um nome e um valor, separados por um sinal de igual `=`. Os atributos podem ser usados para definir propriedades específicas de um elemento, como sua aparência, comportamento ou funcionalidade. Por exemplo, o atributo `href` é usado em uma tag `<a>` para especificar o URL de destino de um link, enquanto o atributo `src` é usado em uma tag `<img>` para especificar a fonte da imagem. Os atributos são essenciais para personalizar e controlar o comportamento dos elementos HTML, permitindo que você crie páginas web mais interativas e dinâmicas.

Imagine que temos a necessidade de criar um link para o site do Google em uma página web. Para isso, podemos usar a tag `<a>` (âncora) e o atributo `href` para especificar o URL do Google. O código HTML correspondente seria:

```html
<a href="https://www.google.com">Visite o Google</a>
```

O que resultaria em um link clicável com o texto "Visite o Google". Quando o usuário clicar nesse link, ele será redirecionado para a página do Google. O atributo `href` é fundamental para criar links em HTML, e seu valor deve ser um URL válido para garantir que o link funcione corretamente, como é possível ver no resultado abaixo:

[Visite o Google](https://www.google.com)

### Lista de todas as tags HTML

Nestes links, você pode encontrar uma lista completa de todas as tags HTML, juntamente com suas descrições e exemplos de uso: [MDN Web Docs - Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element) ou [W3Schools - HTML Tags](https://www.w3schools.com/TAGS/default.asp).

## CSS - Cascading Style Sheets (Folhas de Estilo em Cascata)

O CSS é uma linguagem de estilo usada para controlar a aparência e o layout de uma página web. Ele permite que você defina regras de estilo para os elementos HTML, como cores, fontes, margens, espaçamento, entre outros. O CSS é separado do HTML, o que significa que você pode manter a estrutura do conteúdo (HTML) separada da apresentação visual (CSS). Isso torna o código mais organizado e facilita a manutenção do site. O CSS é composto por seletores e declarações. Os seletores são usados para selecionar os elementos HTML aos quais as regras de estilo serão aplicadas, enquanto as declarações definem as propriedades de estilo e seus valores. Veja o exemplo abaixo:

Considere o seguinte código HTML:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <title>Exemplo de CSS</title>
   <link rel="stylesheet" href="styles.css">
</head>
<body>
   <h1>Olá, Mundo!</h1>
   <p>Este é um exemplo de CSS.</p>
</body>
</html>
```

Neste exemplo, temos um documento HTML básico com um título e um parágrafo. O arquivo CSS externo `styles.css` é vinculado ao documento HTML usando a tag `<link>` no `<head>`. O conteúdo do arquivo `styles.css` pode ser o seguinte:

```css
/* styles.css */
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: #333333;
  text-align: center;
}

p {
  color: #666666;
  font-size: 18px;
  margin: 20px;
}
```

> **⚠️ Nota:**
>
> No exemplo acima, o CSS é aplicado ao HTML, pois o arquivo `styles.css` está vinculado ao documento HTML usando a tag `<link>` no `<head>`. O CSS define o estilo para o elemento `<body>`, o título `<h1>` e o parágrafo `<p>`, controlando a aparência da página web. O CSS é uma parte essencial do desenvolvimento web, pois permite que você crie páginas visualmente atraentes e responsivas, melhorando a experiência do usuário.

O resultado do exemplo acima seria uma página web com um fundo cinza claro, um título centralizado em cor escura e um parágrafo com uma cor mais clara, tamanho de fonte maior e margens ao redor do texto. O CSS é uma ferramenta poderosa para personalizar a aparência de uma página web e criar designs únicos e atraentes.

![CSS Aplicado](docs/image-css.png)

Sem o CSS, a página web seria exibida com o estilo padrão do navegador, que pode variar dependendo do navegador e do sistema operacional. Chamamos isso de `user agent stylesheet`, que é o estilo padrão aplicado pelo navegador aos elementos HTML. O CSS permite que você substitua esse estilo padrão e crie uma aparência personalizada para a sua página web, controlando aspectos como cores, fontes, layout, espaçamento, entre outros. Sem o CSS, a página web seria exibida de forma básica e sem formatação, o que pode resultar em uma experiência de usuário menos atraente e menos profissional.

Sem o CSS que escrevemos, teríamos o seguinte resultado:

![Sem CSS](docs/image-css-none.png)

### Sintaxe do CSS

A sintaxe do CSS é composta por regras de estilo, onde cada regra é formada por um seletor e um bloco de declarações. O seletor é usado para selecionar os elementos HTML aos quais as regras de estilo serão aplicadas, enquanto o bloco de declarações define as propriedades de estilo e seus valores. A sintaxe básica do CSS pode ser representada da seguinte forma:

```css
seletor {
  propriedade: valor;
  propriedade: valor;
  /* ... */
}
```

> **⚠️ Nota:**
>
> O seletor pode ser um nome de elemento HTML, uma classe, um ID ou uma combinação desses. As propriedades de estilo são palavras-chave que definem o aspecto visual dos elementos, como `color`, `font-size`, `background-color` etc. Os valores são atribuídos às propriedades para especificar o estilo desejado, como `red`, `16px`, `#f0f0f0` etc. Cada declaração dentro do bloco de declarações deve ser separada por um ponto e vírgula `;`, e o bloco de declarações deve ser encerrado com uma chave `}`.

### Seletores CSS

Os seletores CSS são usados para selecionar os elementos HTML aos quais as regras de estilo serão aplicadas. A lógica dos seletores é baseada na estrutura do documento HTML (seguindo a hierarquia de elementos, por isso o nome "cascading" — em cascata), e eles permitem que você aplique estilos a elementos específicos ou a grupos de elementos com base em suas características, como tipo, classe, ID, atributos, entre outros.

Considere o seguinte código HTML:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <title>Exemplo de Seletores CSS</title>
   <link rel="stylesheet" href="styles.css">
</head>
<body>
   <h1 class="titulo">Título Principal</h1>
   <p id="paragrafo1">Este é o primeiro parágrafo.</p>
   <p id="paragrafo2">Este é o segundo parágrafo.</p>
   <a href="#" class="link">Este é um link</a>
</body>
</html>
```

Para aplicar estilos a esses elementos usando CSS, podemos usar diferentes tipos de seletores. Por exemplo:

1. Seletor de tipo: para selecionar todos os elementos de um determinado tipo, como `<h1>`, `<p>`, `<a>` etc. Exemplo: `h1 { color: blue; }` aplicaria a cor azul a todos os elementos `<h1>` na página.
2. Seletor de classe: para selecionar elementos com uma classe específica. Exemplo: `.titulo { font-size: 24px; }` aplicaria um tamanho de fonte de 24 pixels a todos os elementos com a classe "titulo".
3. Seletor de ID: para selecionar um elemento com um ID específico. Exemplo: `#paragrafo1 { color: red; }` aplicaria a cor vermelha apenas ao elemento com o ID "paragrafo1".
4. Seletor de atributo: para selecionar elementos com um atributo específico ou um valor de atributo específico. Exemplo: `a[href="#"] { text-decoration: none; }` removeria o sublinhado de todos os links que têm um atributo `href` com o valor "#".
5. Pseudo-classes: para selecionar elementos com base em seu estado ou posição na hierarquia do documento. Exemplo: `p:first-child { font-weight: bold; }` aplicaria negrito ao primeiro parágrafo dentro de seu elemento pai.

Como dito, a hierarquia dos elementos HTML é fundamental para entender como os seletores CSS funcionam, pois eles seguem a estrutura do documento para aplicar estilos. Considere um parágrafo que, por sua vez, está dentro de uma seção, que, por sua vez, está dentro do conteúdo principal da página. No HTML, isso seria algo como:

```html
<main>
  <section>
   <p>Este é um parágrafo dentro de uma seção...</p>
  </section>
</main>
```

Para selecionar e estilizar os parágrafos dentro dessa estrutura, você poderia usar um seletor de descendente como `main section p { color: green; }`, que aplicaria a cor verde a todos os parágrafos que estão dentro de uma seção, que, por sua vez, está dentro do elemento principal `<main>`. Isso demonstra como os seletores CSS seguem a hierarquia dos elementos HTML para aplicar estilos de forma específica e direcionada.

> **⚠️ Nota:**
>
> Os espaços entre os seletores indicam uma relação de descendência, ou seja, o seletor `main section p` seleciona todos os elementos `<p>` que são descendentes de um elemento `<section>`, que por sua vez é um descendente de um elemento `<main>`. Isso permite que você aplique estilos de forma mais específica, garantindo que apenas os elementos desejados sejam afetados pelas regras de estilo, tambem pode se representar por caixinhas onde o `main` seria uma caixa com outra caixa `section` dentro teria uma menor ainda que seria o `p`. 

Se, no HTML que usamos de exemplo, tivéssemos um parágrafo fora da seção, como:

```html
<main>
  <section>
   <p>Este é um parágrafo dentro de uma seção...</p>
  </section>
  <p>Este é um parágrafo fora da seção...</p>
</main>
```

O seletor `main section p` aplicaria a cor verde apenas ao parágrafo dentro da seção, enquanto o parágrafo fora da seção não seria afetado por essa regra de estilo. Isso demonstra como os seletores CSS permitem que você controle a aplicação de estilos com base na hierarquia dos elementos HTML, garantindo que apenas os elementos desejados sejam estilizados de acordo com as regras definidas.

Resultando em algo como:

![Seletores CSS](docs/image-css-selectors.png)

### Tipos de Seletores CSS

Existem vários tipos de seletores CSS que permitem selecionar elementos HTML de diferentes maneiras. Abaixo está uma tabela com alguns dos tipos de seletores mais comuns. Esta tabela tem o intuito de servir como um guia rápido para entender os diferentes tipos de seletores CSS e como eles funcionam. No entanto, existem muitos outros tipos de seletores CSS; abordaremos esses outros tipos em conteúdos futuros. Por enquanto, foque em entender os tipos de seletores mais comuns listados abaixo, pois eles são os mais utilizados e fundamentais para o aprendizado do CSS.

| Tipo de Seletor               | Exemplo&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Descrição |
|------------------------------ | -------------------------------- | --------- |
| Seletor de Tipo               | `nome_elemento { }`              | Seleciona todos os elementos de um determinado tipo. Exemplo: `p { color: blue; }` seleciona todos os parágrafos e aplica a cor azul. |
| Seletor de Classe             | `.nome_classe { }`               | Seleciona elementos com uma classe específica. Exemplo: `.titulo { font-size: 24px; }` seleciona todos os elementos com a classe "titulo" e aplica um tamanho de fonte de 24 pixels. |
| Seletor de ID                 | `#nome_id { }`                   | Seleciona um elemento com um ID específico. Exemplo: `#paragrafo1 { color: red; }` seleciona o elemento com o ID "paragrafo1" e aplica a cor vermelha. |
| Seletor de Atributo           | `elemento[atributo="valor"] { }` | Seleciona elementos com um atributo específico ou um valor de atributo específico. Exemplo: `a[href="#"] { text-decoration: none; }` seleciona todos os links que têm um atributo `href` com o valor "#" e remove o sublinhado. |
| Pseudo-classes                | `elemento:pseudo-classe { }`     | Seleciona elementos com base em seu estado ou posição na hierarquia do documento. Exemplo: `p:first-child { font-weight: bold; }` seleciona o primeiro parágrafo dentro de seu elemento pai e aplica negrito. |

