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

**Emmet:** é um plugin usado em IDEs e editores de código para facilitar a edição dos códigos. Possúi uma sintaxe própria que agiliza e facilita a edição de códigos _HTML_.

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
> O código de três letras é usada quando os pares de informações são os mesmos como visto nos exemplos. Os pares representam as três cores do padrão RGB em hexadecimal e outra forma de escrever tais cores é exatamente com o código RGB como visto no exemplo.

---

**display:** muda o comportamento do elemento na tela. 

Quase tudo funciona em "caixas", englobando o conteúdo do elemento. Algumas englobam áreas muito grandes, como a tag ```<nav>```, funcionando de uma forma atípica. 

**-** _display: inline_ - mantêm os "blocos" na mesma linha. Não funcionam os atributos _width_ e _height_. O "bloco" ganha comportamento de uma palavra, um elemento pai afeta seu comportamento e o que define o tamanho do "bloco" é o conteúdo. 
**-** _display: block_ - ele ocupa toda a linha por padrão, como o elemento ```<nav>```. Permite definir altura e largura.Por padrão sua largura é a "linha" toda, quem define a largura é o elemento pai. A altura é definida pelo conteúdo, o que define, então, é o comportamento dos elementos filhos. 
**-** _display: inline-block_ - o melhor dos dois mundos. Ele mantém na mesma linha, herda o comportamento por palavra, altera largura e altura e se não forem definidas irá seguir o conteúdo.

https://www.youtube.com/watch?v=caxiggysoB4&list=PLirko8T4cEmzrH3jIJi7R7ufeqcpXYaLa&index=74

24-27

---

**section:** significa seção e é ezxatamente isso, é o elemento que cria seções na pagina. Todo conteúdo da tag faz parte de uma seção. É como uma loja, onde existe diversas seções com funções diferentes, assim é um site e para isso se utiliza o elemento ```<section>```.

**-** _div_ - cria uma divisão e não possuí valor semântico. É usado para dar suporte, mas deve-se evitar seu uso pois não atrapalha em fatores como SEO e acessibilidade.

**-** _div x section_ - é usdo em conjunto pato para demarcar e agrupar um conteúdo para dar um comportamento visual. Para definir o conteúdo ela não serve, pois como dito anteriormente, ela não possúi valor semantico e com isso não é capaaz de definir o conteúdo, principalmente para leitores de tela.

--- 

**flexbox:** é um método para criação de layouts alinhando e distribuindo os espaços entres os itens de uma seção do site, esses itens possuindo dimensões dinâmicas ou não e até mesmo desconhecidas. A alura possui um artigo bem completo que você pode [ler aqui](https://www.alura.com.br/artigos/css-guia-do-flexbox?utm_term=&utm_campaign=%5Bfundo%5D+teste+performance+max&utm_source=adwords&utm_medium=ppc&hsa_acc=7722097246&hsa_cam=18663119163&hsa_grp=&hsa_ad=&hsa_src=x&hsa_tgt=&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_ver=3). Assim como a Alura, a Rafa Ballerini possui dois vídeos explicando em detalhes, você pode assistir nas [parte 1](https://www.youtube.com/watch?v=KbjLtEgmZ_E) e [parte 2](https://www.youtube.com/watch?v=hjz6ezV9_uc).

--- 

**reset CSS:** serve para limpar os padrões de todos os elementos _HTML_ que ja possuem suas formatações padrões, evitando elementos com valores "fantasmas" nos códigos atrabalhand oa renderização do conteúdo das páginas. Quase tudode quase todos os elementos vira "padrão", como um texo sem formatação, como diz [Thiago Belem](http://blog.thiagobelem.net/css-reset-o-que-e-e-como-usar). Ele ajuda para que as páginas renderizem da mesma forma em todos os navegadores, uma vez que cada um tem sua forma padrão de renderização.

---

dl
dt
dd

---

progress

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
https://www.youtube.com/watch?v=EfuzIO9nrzs&list=PLirko8T4cEmzrH3jIJi7R7ufeqcpXYaLa&index=79

--- 

webkit moz

---

article

---

:nth-child()

---

figure

---

fatoração

---

box-sizing: 
border-box;

---

transform: 
rotate(90deg) 
translateX(-62%);

---

content: '';

---


