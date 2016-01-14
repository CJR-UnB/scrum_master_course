Clean Code
==========

Já falamos de vários tópicos sobre Clean Code. SOLID, TDD, XP entre outros geram um código de boa qualidade. Porém é importante mostrar uma referência para se atualizar sobre como fazer um código de qualidade e boas práticas de código em sua raiz.

Conheça o [Uncle Bob](https://cleancoders.com/category/clean-code). Ele é referência e seu site tem muito material.

Na CJR, podemos descatar alguns pontos que são importantes que o Scrum Master sempre esteja atento a qualidade.

É importante que o código feito por um desenvolvedor seja comunicativo, legivel e claro, e é dever do Scrum Master cobrar que os desenvolvedores estejam fazendo isso.

*Okay! Mas como manter meu código saúdavel?*

Vamos explicitar alguns pontos que merecem atenção.

**Indentação:** na CJR, devemos usar sempre tab para indentar o código feito. Para todas as linguagens(HTML, CSS, Javascript, Yaml) devem usar um tab de **tamanho 4**. A linguagem Ruby e suas derividas (Slim, por exemplo) devem tem um tab de **tamanho 2**. Caso você esteja usando o Sublime Text, acesse "the easy way" nesse [link](http://mlo.io/blog/2012/08/23/language-specific-indents-sublime.html) para saber como configurar um tamanho de tab especifico para uma linguagem.

**Critérios Gerais**

+ Posicionamento
+ Densidade

**Nomeclatura**

+ Objetivo Claro
+ Sem gracinha

**Classes**

+ São nomes
+ Single Responsibility Principle

**Funções**

+ São verbos
+ Faz bem apenas uma coisa
+ DRY
+ Sem efeitos colaterais

**Comentários**

Explicam sucintamentamente algo que o código em si não pode dizer. Sempre comentar o porquê daquele trecho de código de código.

**Lei de Demeter**

Para um método *F* em uma classe *C*, *F* deve apenas chamar:

+ Métodos de *C*
+ Objetos por criados por *F*
+ Objetos passados como argumento
+ Atributos de *C*

