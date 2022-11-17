# Curso de HTML e CSS feliz

Aqui se encontra o projeto realizado pelo [Marco Bruno Dev](https://twitter.com/marcobrunodev) no [_Curso de HTML e CSS feliz_](https://www.youtube.com/playlist?list=PLirko8T4cEmzrH3jIJi7R7ufeqcpXYaLa)

Projeto concluído: https://lannyer.github.io/cursohtmlcssfeliz/

**header:** usada para criar cabeçalhos em uma página. Representa um grupo de suporte de introdução e de naveação.

---

**nav:**: representa a seção de uma página que aponta para outras páginas, como um menu. É a seção de linls de navegação.

---

**lang:** atributo globl usado para indicar a língua que o texto está escrito. Ajuda no SEO e na acessibilidade dos leitores de tela.

~~~html

<html lang="pt-BR">

    <a href="">Sobre</a>
    <a href="">Contato</a>
    <a href="" lang="en"><em lang="en">Download CV</em></a>

</html>

~~~
> Os valores ```pt-BR```, e ```en``` indicam que os textos naquele escopo, daquela tag é português e inglês respectivamente.

---

**Emmet:** é um plugin usado em IDEs e editores de código para facilitar a edição dos códigos. Possúi uma sintaxe própria que agiliza e facilita a edição de códigos _HTML_.

_Ex:_

~~~

header>img+nav>a*5

~~~

- **>** : coloca uma tag dentro da outra.
- **+** : uma tag "ao lado" da outra
- ***** : cria a quantidade definida de tags iguais.

Resultado logo abaixo

~~~html

        <header>
            <img src="assets/img/logo.png" alt="">
            <nav>
                <a href="" lang="en">Skill</a>
                <a href="">Projetos</a>
                <a href="">Sobre</a>
                <a href="">Contato</a>
                <a href="" lang="en"><em lang="en">Download CV</em></a>
            </nav>
        </header>

~~~
> As tags ```img```, ```nav```, ```a```, dentro da tag ```header```, sendo que a tag ```a``` está dentro da tag ```nav``` que por sua vez, está "ao lado" da tag ```img```.

E também é possível criar tags com conteúdo de texto dentro delas.

~~~

a{Lorem}

~~~
> Basta utilizar o atalho **ctrl+espaço** para abrir a caixa de diálogo e em seguida a tecla _Enter_, para se obter oseguinte resultado.

~~~html

<a href="">teste</a>

~~~

---

**em:** serve para dar ênfas a um texto. Dentro de um parágrafo.

~~~html

<p>Esse filme não me trouxe o <em>flow</em> que eu gostaria. </p>

~~~

Pode ser usado, por exemplo, para indicar que um texto pertênce a outra língua.

~~~html

<p>Esse filme não me trouxe o <em lang="en">flow</em> que eu gostaria. </p>

~~~

---

Com o atributo ```color``` temos várias formas de escrever as cores que seram utilizadas no projeto, escrevendo o nome da cor em inglês, o valor hexadecimal e por aí vai. Segue alguns exemplos:

_Ex:_

~~~html

<style> 

p {
    color: white;
    color: #FFFFFF; 
    color: #FFF;
    color: rgb(255,255,255);
    color: #FF00BB;
    color: #F0B;
}

</style>

~~~
> O código de três letras é usada quando os pares de informações são os mesmos como visto nos exemplos. Os pares representam as três cores do padrão RGB em hexadecimal e outra forma de escrever tais cores é exatamente com o código RGB como visto no exemplo.

---

**display:** muda o comportamento do elemento na tela. 

Quase tudo funciona em "caixas", englobando o conteúdo do elemento. Algumas englobam áreas muito grandes, como a tag ```<nav>```, funcionando de uma forma atípica. 

**-** _display: inline_ - mantêm os "blocos" na mesma linha. Não funcionam os atributos _width_ e _height_. O "bloco" ganha comportamento de uma palavra, um elemento pai afeta seu comportamento e o que define o tamanho do "bloco" é o conteúdo. 
**-** _display: block_ - ele ocupa toda a linha por padrão, como o elemento ```<nav>```. Permite definir altura e largura.Por padrão sua largura é a "linha" toda, quem define a largura é o elemento pai. A altura é definida pelo conteúdo, o que define, então, é o comportamento dos elementos filhos. 
**-** _display: inline-block_ - o melhor dos dois mundos. Ele mantém na mesma linha, herda o comportamento por palavra, altera largura e altura e se não forem definidas irá seguir o conteúdo.

[Aulas de a 24-27.](https://www.youtube.com/watch?v=Jam2An2hvaQ&list=PLirko8T4cEmzrH3jIJi7R7ufeqcpXYaLa&index=24)

---

**section:** significa seção e é ezxatamente isso, é o elemento que cria seções na pagina. Todo conteúdo da tag faz parte de uma seção. É como uma loja, onde existe diversas seções com funções diferentes, assim é um site e para isso se utiliza o elemento ```<section>```.

**-** _div_ - cria uma divisão e não possuí valor semântico. É usado para dar suporte, mas deve-se evitar seu uso pois não atrapalha em fatores como SEO e acessibilidade.

**-** _div x section_ - é usdo em conjunto pato para demarcar e agrupar um conteúdo para dar um comportamento visual. Para definir o conteúdo ela não serve, pois como dito anteriormente, ela não possúi valor semantico e com isso não é capaaz de definir o conteúdo, principalmente para leitores de tela.

--- 

**flexbox:** é um método para criação de layouts alinhando e distribuindo os espaços entres os itens de uma seção do site, esses itens possuindo dimensões dinâmicas ou não e até mesmo desconhecidas. A alura possui um artigo bem completo que você pode [ler aqui](https://www.alura.com.br/artigos/css-guia-do-flexbox?utm_term=&utm_campaign=%5Bfundo%5D+teste+performance+max&utm_source=adwords&utm_medium=ppc&hsa_acc=7722097246&hsa_cam=18663119163&hsa_grp=&hsa_ad=&hsa_src=x&hsa_tgt=&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_ver=3). Assim como a Alura, a Rafa Ballerini possui dois vídeos explicando em detalhes, você pode assistir nas [parte 1](https://www.youtube.com/watch?v=KbjLtEgmZ_E) e [parte 2](https://www.youtube.com/watch?v=hjz6ezV9_uc).

--- 

**reset CSS:** serve para limpar os padrões de todos os elementos _HTML_ que ja possuem suas formatações padrões, evitando elementos com valores "fantasmas" nos códigos atrabalhand oa renderização do conteúdo das páginas. Quase tudode quase todos os elementos vira "padrão", como um texo sem formatação, como diz [Thiago Belem](http://blog.thiagobelem.net/css-reset-o-que-e-e-como-usar). Ele ajuda para que as páginas renderizem da mesma forma em todos os navegadores, uma vez que cada um tem sua forma padrão de renderização.

---

**dl:** de _definition list_, lista de definição. Engloba lista de pares de termos e descrições. 

**dt:** de _definition term_, definição de termo. Serve para identificar um termo na lsta de definição

**dd:** de _description details_, descrição de detalhes. Dá uma definição completa do termo definidono elemento ```dt```.

~~~html

<dl>
  <dt>Firefox</dt>
  <dt>Mozilla Firefox</dt>
  <dt>Fx</dt>
  <dd>A free, open source, cross-platform, graphical web browser
      developed by the Mozilla Corporation and hundreds of volunteers.</dd>
</dl>

~~~

---

**progress:** é usado para visualizar o progresso de uma tarefa. sua visualização é definido pelo usuário, geralmente cria uma barra de progresso.

---

componente filho elemento
https://www.youtube.com/watch?v=erRwlu3k1dY&list=PLirko8T4cEmzrH3jIJi7R7ufeqcpXYaLa&index=83

---

.main-title h1
.main-title .second
.main-title.-second 
 https://www.youtube.com/watch?v=EfuzIO9nrzs&list=PLirko8T4cEmzrH3jIJi7R7ufeqcpXYaLa&index=79

---

componente

---

componente elemento modificador
uma palavra elemento, separado por hifen componente

--- 

**"Webkit":** é uma ferramenta usada para implementar rescursos CSS novos ou proprietários antes da sua definição final.

Como existem muito navegadores e cada um deles funciona de uma forma, é necessário adicionar prefixos para que um estilo CSS funcione.

_Ex:_

 Estas são propriedades e em quais navegadores elas funcionam ```-webkit``` para o Chrome e o Safari, ```-moz``` para o Firefox, ```-o``` para o Opera, ```-ms``` para o Internet Explorer

~~~html
<style>
.elementClass {
    -moz-border-radius: 2em;
    -ms-border-radius: 2em;
    -o-border-radius: 2em;
    -webkit-border-radius: 2em;
    border-radius: 2em;
</style>
~~~

---

**article:** representa uma composição independente do documento que é destinado a ser utilizado de forma independente ou reutilizável.

>- Quando um elemento <article> está aninhado, o elemento interior representa um artigo relacionado com o elemento exterior. Por exemplo, os comentários do post de um blog podem ser elementos <article> aninhados em <article> representando o post do blog.
>- Informações sobre o autor de um elemento <article> podem ser fornecidas através do elemento <address> ,mas ele não se aplica aos elementos <article> aninhados.
>- A data e hora de publicação de um elemento <article> pode ser descrita usando o atributo pubdate de um elemento <time>.
>Fonte: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/article

---

**:nth-child():** uma pseudo-classe. Seleciona elementos com base em suas posições em um grupo de elementos irmãos.

_Ex:_ 

~~~html
<style>

:nth-child(4n) {
  color: lime;
}
~~~
>Seleciona um a cada quatro elementos de qualquer grupo de elementos irmãos, começando do quarto elemento (4, 8 12, etc.). 

**-** _Pseudo-classe_: é uma palavra-chave adicionada a seletores que especifica um estado especial do elemento. Pseudo-classes permitem que aplique estilos a um elemento em relação ao conteúdo da árvore do documento, navegação, status do conteúdo, posição do mouse.

---

**figure:** representa conteudo autocontido, que pode conter legenda que é especificada usando o elemento ```figcaption```.
>A figuram sua legenda e seu conteúdo saõ referenciados como uma única unidade.

_Ex:_

~~~html

<!-- Apenas uma imagem -->
<figure>
  <img src="favicon-192x192.png" alt="O lindo logotipo do MDN." />
</figure>

<!-- Imagem com legenda -->
<figure>
  <img src="favicon-192x192.png" alt="O lindo logotipo do MDN." />
  <figcaption>Logotipo MDN</figcaption>
</figure>
    
~~~
>- Normalmente uma <figure> é uma imagem, ilustração, diagrama, trecho de código, etc., que é referenciado no fluxo principal de um documento, mas que pode ser movido para outra parte do documento ou para um apêndice sem afetar o fluxo principal.
>- Uma legenda pode ser associada ao elemento <figure> inserindo um <figcaption> dentro dele (como o primeiro ou o último filho). O primeiro elemento <figcaption> encontrado na figura é apresentado como legenda da figura.
>Fonte: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/figure

---

**Refatoração:** consiste em revisar o código com o intuito de remover redundâncias e incosistências.

---

**box-sizing:** altera as propriedades padrão do _box model_ usado para calcular altura e largura dos elementos. Um de seus valores é o _border-box_.

**-** _border-box_: as propriedades de largura (width) e de altura (height) incluem o tamanho padding size e a propriedade border, mas não incluem a propriedade margin.
>Fonte: https://developer.mozilla.org/pt-BR/docs/Web/CSS/box-sizing

**-** _box model_: é um módulo de CSS que define caixas retangulares incluindo preenchimento e margem.
>Fonte: https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Box_Model

---

transform: 
rotate(90deg) 
translateX(-62%);

---

**content:** é usado para gerar conteúdo em um elemento.
>Fonte: https://developer.mozilla.org/pt-BR/docs/Web/CSS/content

_Ex:_

~~~html
<style>
.button-arrow::before {
    content: '';
    display: block;
    box-sizing: border-box;
    width: 15px;
    height: 15px;
}
</style>
~~~

---

**calc():** é umafunção CSS permite executar cálculos quando especificar os valores das propriedades.

~~~html

<style>
width: calc(100% -80px);
</style>

~~~

---

**footer:** é o elemento usado para criação de rodapé no _sectioning contant_ mais próximo, ou seu parente mais próximo.
>Sectioning contant, ou conteúdo de seção, são os conteúdos que definem o escopo dos cabeçalhos e rodapés.

---

**legend:** representa um rótulo para o contéudo, muito usado para dar títulos a forulários.
