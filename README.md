# 100-days-of-code

# dia 02

O que aprendemos?

- O que significa HTML?

Html é uma linguagem de marcação onde usamos Tags para fazer a estruturação dos nossos sites.

- O que são elementos?

Elementos é um "bloco" de códigos que diz ao browser qual o tipo de conteudo será visivel.

```html:

<h1> Hello Word!</h1> <!--Elemento-->

```

No exemplo acima, h1 é o nome do elemento, e o que está entre o h1 é o nome do conteudo.

- Como adicionar e modificar elementos com css inline?

Podemos modificar os elementos HTML de 3 formas usando CSS.

- inline
- interno
- externo

# dia 03

o que aprendemos?

- Como adicionar cor?

Usamos a propriedade **_color_** onde podemos atribuir 4 tipos de valores.

- Hexadicimal
- Rgb
- Rgba
- Escrita (red,blue)

- Utile o Devtools para debugar e modificar/testar modificações.

- Como adicionar links?

```html:

<a src="google.com">Google Aqui</a>

```

- Esqueleto do HTML.

Dentro de uma estrutura HTML temos duas partes cruciais para o funcionamento de um web-site.

- Head

Tudo que é invisivel para o site, como o titulo da página, links de folha de estilo (css), google-fonts , meta tags.

- Body

Já o body é tudo que está visivel em um site, conteudo, imagens, audio, videos.

- Atalhos Vscode

Dicas de atalhos para usarmos no vscode.

- Use **_Tab_** para identar.
- Use e abuse do Emmet abbreviation
- Mova elementos **_alt + up or down_**

# dia 04

O que aprendemos?

- Como mudar a cor dos links?

```html:

<a src="google.com" style="color:red">Google Aqui</a>

```

Podemos mudar a cor dos links e a forma que ele "age" ao ser clicado , ou quando passamos o mouse por cima, para isso usamos **_hover_**.

- O que são IDs?

Ids são identificadores unicos que podemos adicionar em alguma tag do HTML e que podemos selecionar de forma unica para estilizar com o CSS. (Só podemos ter repetição de id #paragrafo).

- Como importar fontes do google?

Ao trabalharmos com fontes no css, podemos usar as padrões Arial, san-serif ou adicionar fontes direntes do google, mas como fazemos isso?

Escolhemos a fonte que queremos no google fonts, verificamos o peso da font e adicionamos no nosso css via @import ou no nosso html via link.

# dia 05

- Como adicionar Imagens?

Podemos adicionar imagens ou incluir como background (vai ficar embaixo do conteudo).

```html:

<img src="minha-foto.png">Esse sou eu</img>

```

```css:

background-image: url('minha-foto.png')

```

- Como arrendondar uma img?

Podemos arrendondar imagens usando a propriedade **_border-radius:100px_**

- Como organizar os arquivos em pastas.

Podemos fazer um projeto com os arquivos soltos, mas ter uma organização em pasta facilita achar os arquivos e deixa o trabalho mais organizado.

Imagens : Criar uma pasta de imagens
Css : Criar uma pasta com para organizar os arquivos css.

# dia 06

- O que aprendemos?

Listas e tags semanticas, o que são containers, cascata, herança e especificidade e vamos ver tambem um pouco sobre box-model.

- Liver-server

Liver-server é uma extensão do vscode que atualiza nossa aplicação no momento que salvamos as mudanças, assim não precisamos ficar dando reloud na página a cada mudança.

- Como adicionar listas no nosso HTML?

No html temos 2 tipos de listas, as ordernadas e as não ordernadas.

- Lista não ordernada

```html:

<ul>
<li>pasta</li>
<li>bife</li>
<li>feijão</li>
</ul>

```

- Lista ordernada

```html:

<ol>
<li>segunda</li>
<li>terça</li>
<li>quarta</li>
</ol>

```

- O que é herança no css?

Herança é quando aplicamos uma certa mudança no Body por exemplo e ele aplica para todos seus filhos (tudo que está dentro do body) salvo alguns tags (como o link). essas mudanças herdadas são desfeitas quando mudamos especificamente.

```css:

body {
  color:red;
}

p {
  color: blue;
}

```

No exemplo acima, a tag p teria a cor vermelha herdada pelo "pai" body, mas como definimos sua cor especificamente, ela deixa a cor vermelha e passa a ser azul.

- O que é cascata?

No Css as aplicações de estilos são feitas em modo cascata, ou seja de cima para baixo, caso tenhamos 2 mudança em um unico elemento, o que estiver mais abaixo será aplicado.

```css:

p {
  color:red;
}

p {
  color: blue;
/* } a cor azul "vence pela cascata" */

```

- O que é espeficidade?

Quando mais especifico for nossa seleção de elementos mais "pontos" ela terá, e quem tiver mais pontos vence a estilização.

como no exemplo acima, estamos selecionando 2 tags p ( peso 001), que tem o mesmo peso/valor então ganha quem for o ultimo.

No caso da especificade, caso algum desses p tivesse uma classe por exemplo (peso 010) idenpendente da onde a classe estive escrita, a estilização seria aplicada.

# dia 07

- O que aprendemos?

Aprendemos sobre border-box, o que é , como é dividido nossas caixas.

- Border box

- content (conteudo de cada caixa,texto,imagem,audio)
- border (toda caixa tem uma borda, mas so fica visivel se aplicada)
- padding (espaçamento interno entre o content e a borda)
- margin (espaça externo - entre uma caixa e outra)

Obs: ao adicionarmos padding e borda o tamanho/largura passa de um valor x para y, pois ele soma as propriedades da borda e do padding. Para resolvermos isso usamos uma outra propriedade (box-sizing:border-box) que ajusta o tamanho da caixa para suportar o padding e e a borda.

- Layouts

Como desenvolvedores front-end devemos pensar que cada parte dos nossos sites são layouts, e com isso o HTML tem tags semanticas que ajudam a melhor projetar esses layouts.

- header
- nav
- main
- footer
- divs

- Seletores

Podemos selecionar os elementos do HTML para estilizar com o css de diversas formas, tais como:

- tipo: nome da tag (h1,p)
- id : #meuid
- classes : .color
- grupo : div , p

- Combinando Seletores

Tambem podemos combinar seletores para que possa ter uma especifidade maior ou algo mais "exclusivo"

- descendente : li p (estiliza todos os p filho de li)
- filho : h2 > p (estiliza apenas o filho(p) direto de h2)
