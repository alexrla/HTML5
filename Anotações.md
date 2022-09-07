# HTML
- **Linguagem de Marcação de HiperTexto (HyperText Markup Language);**

- **Define o significado e a estrutura do conteúdo da web;**

- **Extensão: `.html`;**

- **Exemplo de código:**

  ```html
  <!DOCTYPE html>
  <html lang="pt-BR">
      <head>
          <meta charset="UTF-8">
          <meta http-equiv="X-UA-Compatible" content="IE=edge">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>Título da página</title>
      </head>
      <body>
          <h1>Cabeçalho - Nível 1</h1>
          <p>Meu primeiro parágrafo!</p>
      </body>
  </html>
  ```

- **Hipertexto faz referência aos links que conectam as páginas (podemos ir de uma página para outra);**

- **O HTML é uma linguagem de marcação porque trabalha com rótulos (tags);**

- **Elemento HTML: **

  ```html
  <identificador_da_tag>Conteúdo</identificador_da_tag>
  ```

  **Tudo que vai da tag inicial (ou de abertura), pegando o conteúdo, até a tag final (ou de fechamento);**

- **Tags indicam ao navegador, o tipo de conteúdo que ele deve mostrar;**

  

### Estrutura básica

- **`<DOCTYPE html>`: instrução que informa ao navegador, a versão do HTML (nesse caso, temos o HTML5);**
- **`<html>`: envolve todo o conteúdo do arquivo (representa a raiz do arquivo HTML);**
- **`<head>`: envolve quase que todas as informações que não ficam visíveis para o usuário ("cabeça da página)";**
- **`<title>`: corresponde ao título da página (que fica localizado na guia do navegador);**
- **`<body>`: envolve o conteúdo que fica visível ao usuário: textos, imagens, etc. ("corpo da página");**



### Meta tags, cabeçalhos e parágrafos

- **As metas tags correspondem aos metadados, que são informações lidas somente pelos navegadores;**
- **` lang`: atributo que indica o idioma da página;**
- **`<meta charset="UTF-8">`: indica o tipo de codificação de caracteres a ser utilizado (UTF-8). A partir do tipo UTF-8, podemos representar uma grande quantidade de caracteres, incluindo caracteres que apresentam acento e o próprio cedilha;**
- **`<meta http-equiv="X-UA-Compatible" content="IE=edge">`: utilizada para a compatibilidade com o Internet Explorer;**
- **` <meta name="viewport" content="width=device-width, initial-scale=1.0">`: configura a janela de visualização da página, para se adptar a tela do dispositivo do usuário (notebook, smartphone, tablet, etc.);**
- **Outras meta tags:**
  - **`<meta name="description" content="Descrição do site">`: informa a descrição do site;**
  - **`meta name="keywords" content="palavras-chave">`: informamos as palavras-chaves, relacionadas ao conteúdo do nosso site;**
  - **`<meta name="author" content="Nome do autor"`: informa o nome do criador do site/da página;**
- **Tags de cabeçalhos, são tags usadas para títulos;**
- **Existem 6 "níveis" de título: `<h1>...<h6>` (o `<h1>` é o mais importante, enquanto o `h6` é o título de menos importância);**
- **No nosso arquivo `.hthml`, devemos ter apenas uma tag `<h1>`;**
- **Parágrafos são definidos a partir da tag `<p>`;**
- **Os navegadores removem espaços e quebras de linha, aplicados no conteúdo de uma tag `<p>`, de forma automática;**



### Formatação de texto

- **Para deixarmos o texto em negrito, podemos utilizar as tags: `<b>` ou `<strong>`;**
- **A tag `<b>`, apenas marca um trecho em negrito. Já tag `<strong>`, ela é utilizada quando além de marca um trecho em negrito, queremos dar importância aquele trecho (dizemos que aquele trecho é importante);**

- **Para dividir contéudos, separar seções da nossa página, podemos usar a tag `<hr>` (horizontal rules);**
- **Para quebra/pular uma linha, usamos a tag `br` (break row);**
- **Para deixar o texto em itálico, podemos utilizar as tags: `i` ou `em`;**
- **A tag `<i>` aplica o estilo itálico ao conteúdo textual desejável, enquanto a tag `<em>` deve ser utilizada para, além de aplicar o estilo itálico, dar enfâse ao texto;**
- **Para aplicar o efeito sublinhado em um texto, usamos a tag: `<u>`;**
- **A tag `<small>` deixa o texto em um tamanho de fonte menor, em relação ao tamanho que foi definido;**
- **A tag `<del>` aplica o efeito riscado/taxado, em um texto (usada para declarar que aquele texto foi deletado/excluído);**
- **A tag `<sup>` diminui o tamanho da fonte e eleva o texto acima da linha de base (um texto sobrescrito);**
- **Já a tag `sub`, também diminui o tamanho da fonte, mas agora faz com que o texto fique abaixo da linha de base (texto subscrito);**
- **Para deixar um texto em destaque, podemos usar a tag `<mark>` (semelhante a um trecho de texto, quando escrevemos a mão e aplicamos uma marcador de texto, para deixar aquele trecho em destaque);**



### Elementos de citação

- **Para representar abreviações, podemos usar a tag `<abbr>` (usado em conjunto com ela, temos o atributo `title`, que contém a descrição da abreviação e assim, ao passarmos o mouse sobre o conteúdo da tag `abbr`, conseguimos ver a descrição);**
- **A tag `<address>`, é utilizada quando queremos fornecer informações de contato (e-mail, telefone, mídias sociais,...) ou endereço (endereço físico). O conteúdo da tag `address` acaba sendo renderizado em itálico e ganha espaçamento (uma linha), acima e abaixo;**
- **A tag `<cite>` é utilizada quando mecionamos títulos de obras/trabalhos (o texto acaba sendo renderizado em itálico);**
- **A tag `<q>` é utilizada para citações curtas (geralmente, é adicionado aspas, ao redor da citação);**
- **Para citações longas, ou ainda, citações de fontes externas, podemos usar a tag `<bockquote>` (em conjunto com ela, usamos o atributo `cite`, que é onde especificamos a fonte, do qual aquela citação foi retirada);**
- **Se quisermos alterar a direção do texto, podemos utilizar a tag `<bdo>`. Em conjunto com ela, usamos o atributo `dir`, onde podemos passar os valores: `ltr` (valor padrão, da esquerda para direita) ou `rlt` (da direita para esquerda);**



### Comentários

- **Os comentários em HTML, são inseridos a partir da seguinte estrutura:**

  ```html
  <!-- Isso é um comentário em HTML -->
  ```

  **Comentários não são exibidos para os usuários e normalmente, são utilizados para documentar o código ou para "desativar" trechos do código;**



### Links

- **Para criar um _link_, utilizamos a tag `<a>`;**
- **Junto da tag `<a>`, utilizamos o atributo `href`, que é onde indicamos o destino do  link (o que iremos acessar ao clicar naquele link);**
- **Para podermos clicar em um _link_, e o destino daquele link (uma outra página), ser aberto em uma nova guia, podemos utilizar o atributo `target`, com o valor `_blank`;**
- **Utilizando o atributo `download`, podemos criar um _link de download_, ao invés de um _link de navegação_. Com isso, no atributo `href`, informamos o arquivo que será baixado e no atributo `download`, podemos passar ou não um valor (o valor passado corresponderá ao nome do arquivo a ser baixado, renomeamos o arquivo);**
- **Através de links, podemos navegar por seções da nossa página. Para isso, definimos um `id` (um atributo) para o elemento HTML que queremos ser redirecionado e na tag `<a>`, passamos no atributo `href`, um cerquilha (#) seguido pelo valor do atributo `id`, definido para o elemento HTML, que queremos ser redirecionado;**
- **Para criar um link que abra um programa de e-mail, no atributo `href`, passamos a informação `mailto:`, seguida pelo endereço de e-mail do destinatário;**

#### Caminho absoluto (URL absoluta)

- **Quando indicamos o caminho completo para uma outra página;**

#### Caminho relativo (URL relativa)

- **Quando indicamos o caminho para uma página dentro do nosso próprio projeto;**



### Imagens

- **Para definirmos uma imagem na nossa página, utilizamos a tag `<img>`;**

- **Junto a ela, temos o atributo `src`, que é onde passamos o caminho para a imagem;**

- **Além do atributo `src`, também temos o atributo `alt`, onde informamos um texto alternativo (que descreva imagem). Isso acaba sendo útil para o caso das imagens "quebrarem" (esse texto acabará sendo exibido) e para o caso dos usuários que fazem uso de leitores de tela;**

- **A tag `<img>` não possui conteúdo e consequentemento, não possui uma tag de fechamento (acaba sendo um elemento vazio);**

- **Para adicionarmos um _favicon_ na nossa página (uma imagem que fica localizada na barra de título do navegador), temos o seguinte elemento HTML:**

  ```html
  <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
  
  <!--
  	É comum, para um favicon, termos um arquivo favicon.ico
  -->
  
  <!--
  	A tag <link> é declarada dentro do elemento <head>
  -->
  
  <!--
  	Imagens podem ser utilizadas como links (a tag <a> acaba
  	envolvendo a tag <img>) 
  -->
  ```



### Tabelas

- **Para criarmos tabelas, utilizamos a tag `<table>`;**
- **A tag `<tr>` define uma linha da tabela;**
- **Já uma célula da tabela, é determinada a partir da tag `<td>`;**
- **Para definirmos o cabeçalho, o corpo e o rodapé de uma tabela, usamos as tags: `<thead>`, `<tbody>`, e `<tfoot>`, respectivamente;**
- **Para o cabeçalho das tabelas, ao invés de tags `<td>`, utilizamos tags `<th>` para definirmos as células do cabeçalhos (as tags `<th>` acabam "aplicando um estilo negrito", nos seus "conteúdos" e os alinhando ao centro);**
- **Em tabelas, podemos utilizar os atributos `colspan` (que indica quantas colunas a célula irá ocupar) e `rowspan` (que indica quantas linhas a célula irá se estender);**
- **Podemos criar legendas (que servem como cabeçalho para toda a tabela), através da tag `<caption>` (essa tag deve ser inserida após a tag `<table>` - tag de abertura);**



### Listas

- **Para criarmos listas não ordenadas, utilizamos a tag `<ul>`;**
- **Já para criarmos listas ordenadas, utilizamos a tag `<ol>` (na lista ordenada, é exibida uma contagem sequencial dos itens);**
- **Já para criarmos os itens da lista, em ambas as listas, ordenada ou não ordenada, utilizamos a tag `<li>`;**
- **Existem ainda, as listas de descrição, definidas a partir da tag `<dl>`;**
- **Em listas de descrição, ainda temos a tag `<dt>`, onde definimos o termo e temos a tag `<dd>`, que é onde descrevemos esse termo;**
- **Ainda, para as listas ordenadas, podemos altera o tipo de marcador, através do atributo `type`:**
  - **`type="1"`: define números, como marcadores (valor padrão);**
  - **`type="A"`: define letras maiúsculas, como marcadores;**
  - **`type="a"`: define letras minúsculas, como marcadores;**
  - **`type="I"`: define números romanos (com as letras em maiúsculo), como marcadores;**
  - **`type="i"`: define números romanos (com as letras em miniúsculo), como marcadores;**




### Iframes

- **A partir de _iframes_ (elemento `<iframe>`), podemos exibir uma página, dentro de outra;**
- **Em conjunto com a tag `<iframe>`, temos o atributo `title`, que é onde descrevemos o conteúdo do nosso _iframe_ (usado em leitores de tela);**
- **O atributo `frameborder`, também utilizado em conjunto com a tag `<iframe>`, possui dois valores: 1 (valor padrão - uma borda é desenhado ao redor do _iframe_) e 0 (informa que a bordas não devem ser desenhadas);**



### Formulários

- **Para criar um formulário, utilizamos a tag `<form>`;**
- **No atributo `action`  da tag `<form>`, informamos para onde serão enviados os dados do formulário;**
- **Já no atributo `method`, também da tag `<form>`, informamos o método que será utilizado para enviar os dados do formulários (`post`/`get`);**
  - **OBS.: o método `get` é considerado inseguro pois ao enviar o formulário/ao enviar os dados do formulário, esses dados acabam sendo anexados ao final URL da página de destino dos dados;**

- **O elemento que mais vemos em um formulário, é o elemento `<input>` (elemento de entrada);**
- **O elemento `<input>` possui diferentes `types` (atributo que define o tipo do _input_):**
  - **`text`: campo de entrada do tipo texto;**
  - **`email`: campo de entrada do tipo e-mail;**
  - **`password`: campo de entrada do tipo senha;**
  - **`submit`: campo de enviar formulário (cria um botão);**
  - **`radio`: campo de escolha única;**
  - **`checkbox`: campo de múltipla escolha;**
  - **`reset`: restaura os campos do formulário para o seus valores padrões (cria um botão);**
  - **`tel`: campo de entrada utilizado para a inserção de um número de telefone;**
  - **`date`: campo de entrada utilizado para a inserção de uma data (sem horário);**
  - **`datetime`: campo de entrada utilizado para a inserção de data e horário;**
  - **`number`: campo de entrada para inserção de números;**
- **O elemento `<label>` especifica uma legenda/rótulo para um outro elemento HTML. No elemento `<label>`, especificamos para quê "serve" aquele campo;**
- **Em conjunto com o elemento `<label>`, usamos o atributo `for` que conecta o seu valor, ao `id` do outro elemento HTML, ao qual o elemento `<label>` está sendo aplicado como rótulo (isso possibilita que ao clicarmos no _label_ em uma página, o campo ao qual o _label_ foi conectado, fique "focado"/"ativado");**
- **O atributo `placeholder`, utilizados em campos de entrada como o _input_, corresponde a um dica a qual adicionamos ao _input_, para ajudar o usuário no preechimento dos dados no formulários;**
- **O atributo `autocomplete`, é utilizado para o autopreenchimento de um campo do formulário. Ele possui dois valores: `off` (o usuário deve informar os dado para o campo) e `on` (o navegador completa de forma automática o campo, com base nos valores já inseridos pelo usuário);**
- **O atributo `required`, torna o preenchimento de um campo de formulário, obrigatório;**
- **O atributo `autofocus`, possibilita que um campo, somente um, "esteja focado"/"seja ativado", quando a página é carregada;**
- **Junto do _input_ do tipo _radio_ , usamos o atributo `value` para definir o valor a ser enviado no formulário (o mesmo vale para outros elementos de formulário);**
- **Os _inputs_ do tipo _radio_ que o possuem o mesmo valor para o atributo `name`, ficam/pertencem ao mesmo "grupo de escolha" (o atributo `name` é utilizado para identificar os campos no formulário) ;**
- **Podemos usar o atributo `checked`, em "campos de escolha", para definirmos um item que já vem selecionado, por padrão;**
- **Além do elemento `<ìnput>` (um elemento de formulário), temos o elemento `<select>`. O elemento `<select>` permite a criação de um menus de opções, que podem ser selecionadas;**
- **As opções desse menu, criado a partir do elemento `<select>`, são definidas a partir do elemento `<option>` e podem ser agrupadas através do elemento `<optgroup>`;**
- **Podemos usar o atributo `selected` em algum elemento `<option>`, para deixarmos uma opção já selecionada, por padrão;**
- **Com o atributo `disabled`, podemos desabilitar/desativar algum elemento de formulário (algum _input_, alguma opção do _select_, algum botão, etc.);**
- **O elemento `<textarea>`, cria um campo de entrada de texto, de várias linhas;**
- **Através dos atributos `rows` (altura a altura - quantidade de linhas - do campo) e `cols` (altera a largura - número de colunas - do campo), podemos aumentar/diminuir, o campo criado a partir do elemento `<textarea>`;**
- **Os atributo `minlength` e `maxlength`, determinam o número mínimo e máximo, respectivamente, de caracteres, de elementos _input_  (que trabalham com texto) e _textarea_;**
- **Os atributos `min` e `max`, determinam um valor mínimo e máximo (aceito/válido), respectivamente, para campos que trabalham com números;**
- **Podemos utilizar expressões regulares, para aplicar validações nos campos, através do atributo `pattern`;**
- **A tag `<button>`, também é utilizada para criar botões (neste caso, podemos criar botões genéricos, que não servem apenas para enviar dados de um formulário);**
- **O elemento `<fieldset>`, é utilizado para agrupar elementos, relacionados, em um formulário (uma "caixa" é "desenhada", ao redor dos campos do formulário);**
  - **A tag `<legend>` é utilizada para definirmos uma legenda para um _fieldset_;**




### Aúdio

- **Para aplicar um espaço entre elementos HTML, usamos a entidade HTML, `&nbsp;`;**

- **Para escrever código HTML, sem que esse códgio seja interpretado pelo navegador, utilizamos as entidades HTML , `&lt;` e `&gt;`:**

  ```html
  &lt;p&gt;Este é um parágrafo&lt;/p&gt;
  
  <!-- Saída -->
  <p>Este é um parágrafo</p>
  ```

- **Para reproduzirmos arquivos de aúdio na nossa página, usamos o elemento HTML `<audio>`;**

- **No elemento `<audio>`, aplicamos o elemento `<source>`, que é onde especificamos o nosso arquivo de aúdio, através do atributo `src` (podemos aplicar vários arquivos de diferentes tipos e o primeiro tipo/formato a ser reconhecido pelo navegador, que o navegador oferece suporte, é o que será exibido na página);**

- **Além do atributo `src`, no elemento `<source>` também usamos o atributo `type`, para especificar o tipo do arquivo (tipo de mídia);**

- **Agora, para podermos ver o arquivo de áudio na nossa página, devemos atribuito no elemento `<audio>`, o atributo `controls` (que exibe os controles de aúdio);**

- **O conteúdo existente no elemento HTML, só será exibido em navegadores que não oferecem suporte ao elemento HTML `<audio>`;**

- **Podemos iniciar um arquivo de aúdio de forma automática, aplicando o atributo `autoplay` no elemento HTML `<audio>`;**

- **Para remover a opção de download do aúdio, em que em alguns navegadores é ofertado, aplicamos o atributo `controlsList`, com o valor `nodownload`, no elemento HTML `<audio>`;**

- **OBS.: Podemos reproduzir arquivos de aúdio na nossa página, usando simplesmente o elemento HTML `<audio>`, e no mesmo, utilizando o atributo `src`, para especificar o nosso arquivo de aúdio;**

- **Formatos de áudio e seus respectivos `type` (tipos de mídia):**
  - **MP3 - audio/mpeg;**
  - **OGG - audio/ogg**
  - **WAV - audio/wav**



### Vídeo

- **Para reproduzir um arquivo de vídeo na nossa página, usamos o elemento HTML, `<video>`;**
- **Algumas coisas que se aplicam ao elemento `<audio>`, também se aplicam ao elemento `<video>`, como por exemplo: o elemento `<source>` para podermos especificar o nosso arquivo, o fato do conteúdo do elemento `<video>` só poder ser exibido, caso o navegador não ofereça suporte ao elemento, e os atributos `controls`, `autoplay` e `controlsList`, agora aplicados no elemento `<video>`;**
- **Para podermos usar uma imagem de _thumbnail_ do nosso vídeo, utilizamos o atributo `poster`, e indicamos o caminho da imagem;**
- **Para desativar a opção "picture in picture", podemos usar o atributo `disabledpictureinpicture`;**
- **Para desabilitar a opção de "fullscreen", no atributo `controlsList`, passamos o valor `nofullscreen`;**
- **Podemos inicializar um vídeo de forma automática e silenciado, adicionando o atributo `muted`, após o atributo `autoplay` (o atributo `muted` também é aplicável ao elemento `<audio>`);**
- **Ainda, temos o atributo `loop`, que reinicia o vídeo, sempre que o mesmo acaba, de forma indeterminada (ele também é aplicado ao elemento `<audio>`);**
- **OBS.: Também podemos reproduzir arquivos de vídeo na nossa página, usando simplesmente o elemento HTML `<video>`, e no mesmo, utilizando o atributo `src`, para especificar o nosso arquivo de vídeo;**
- **Formatos de vídeo e seus respectivos `type` (tipos de mídia):**
  - **MP4 - video/mp4;**
  - **WebM - video/webm**
  - **Ogg - video/ogg**



### Div

- **A tag `<div>` é utilizada para definir uma seção da página, acaba criando um contêiner genérico, utilizado para agrupar outros elementos HTML (podemos colocar qualquer tipo de conteúdo, em uma _div_);**



### Span

- **A tag `<span>` é utilizada para "marcar" algum trecho de um conteúdo textual e assim como a tag `<div>`, cria um contêiner genérico;**
- **Se diferencia da `div` pelo fato de ser um elemento _inline_, enquanto a `div` é um elemento _block_;**



### HTML semântico

- **O HTML semântico, consiste em descrever o significado do conteúdo presente no nosso arquivo HTML, de modo que esse conteúdo fique mais claro tanto para os programadores, como para o browsers (que processam esse conteúdo);**
- **Elementos semânticos:**
  - **`<header>`: utilizado para o cabeçalho da página;**
  - **`<section>`: representa uma seção da página;**
  - **`<article>`: representa um conteúdo que não depende de outro, para fazer sentido;**
  - **`<nav>`: utilizado para agrupar links (normalmente, menus de navegação);**
  - **`<footer>`: utilizado para o rodapé da página;**
  - **`<aside>`: define um conteúdo além do conteúdo principal (geralmente, barras laterais);**
    - **O conteúdo do elemento `<aside>` deve estar indiretamente ligado, ao conteúdo principal;**
  - **`<main>`: especifica o conteúdo principal da página (de maior importância);**
  - **`<figure>`: especifíca um conteúdo independente da página, que pode ser movido para outras página, sem alterar o fluxo principal;**
    - **Esse conteúdo independente, normalmente são ilustrações, fotos, ou diagramas;**
    - **Dentro do elemento `<figure>`, passamos uma tag `<img>`, onde definimos a ilustração e ptambém passamos uma tag  `<figcaption>`, onde definimos uma legenda para o elemento `<figure>`;**