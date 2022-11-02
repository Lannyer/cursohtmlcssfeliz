# Curso de HTML e CSS feliz


Lorem ipsum dolor sit amet...


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

**Emmet:** é um plugin usado em IDEs e editores de código para facilitar a edição dos códigos. Possúi uma sintaxe própria que agiliza e facilita a edição de códigos HTML.

_Ex:_

~~~html
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

~~~html
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
> O código de trÊs letras é usada quando os pares de informações são os mesmos como visto nos exemplos. Os pares representam as três cores do padrão RGB em hexadecimal e outra forma de escrever tais cores é exatamente com o código RGB como visto no exemplo.

--- 

**reset CSS:**

---

**display:** muda o comportamento do elemento na tela. 

Quase tudo funciona em "caixas", englobando o conteúdo do elemento. Algumas englobam áreas muito grandes, como a tag ```<nav>```, funcionando de uma forma atípica. 

**-** _display: inline_ - mantêm os "blocos" na mesma linha. Não funcionam os atributos _width_ e _height_. O "bloco" ganha comportamento de uma palavra, um elemento pai afeta seu comportamento e o que define o tamanho do "bloco" é o conteúdo. 
**-** _display: block_ - ele ocupa toda a linha por padrão, como o elemento ```<nav>```. Permite definir altura e largura.Por padrão sua largura é a "linha" toda, quem define a largura é o elemento pai. A altura é definida pelo conteúdo, o que define, então, é o comportamento dos elementos filhos. 
**-** _display: inline-block_ - o melhor dos dois mundos. Ele mantém na mesma linha, herda o comportamento por palavra, altera largura e altura e se não forem definidas irá seguir o conteúdo.

---

**section:** significa seção e é ezxatamente isso, é o elemento que cria seções na pagina. Todo conteúdo da tag faz parte de uma seção. É como uma loja, onde existe diversas seções com funções diferentes, assim é um site e para isso se utiliza o elemento ```<section>```.

**-** _div_ - cria uma divisão e não possuí valor semântico. É usado para dar suporte, mas deve-se evitar seu uso pois não atrapalha em fatores como SEO e acessibilidade.

**-** _div x section_ - é usdo em conjunto pato para demarcar e agrupar um conteúdo para dar um comportamento visual. Para definir o conteúdo ela não serve, pois como dito anteriormente, ela não possúi valor semantico e com isso não é capaaz de definir o conteúdo, principalmente para leitores de tela.

--- 


