Desenvolvimento Ágil
====================

### O que é desenvolvimento ágil?

Desenvolvimento ágil é um novo modelo de desenvolvimento que procurar principalemnte gerar mais valor para o cliente atravez de uma comunicação mais eficiente do que um contrato fixo.
Esse modelo de desenvolvimento foi criado depois da frustação de vários desenvolvedores e gerentes com seus projeto a partir do manifesto ágil. Caso deseje ler mais sobre isso, acesse o [link](http://www.manifestoagil.com.br/).
Ao longo desse capítulo você poderá descobrir como o desenvolvimento funciona dentro da CJR.

### Good Programmming Practices

Primeiramente, vamos começar com o básico. Respondá o estudo dirigido `/chapter_2/exercise_2.md` para continuar sua jornada pelo conhecimento.

Agora você já está preparado, vamos ao que interessa.

Vamos começar pelo principios SOLID. Existem 5 principios que melhoram a qualidade das classes feitas pelos programadores.
Obs: a partir de agora, você encontrará o termo entidade de softwate, ou somente entidade, que significa um classe, módulo, função, etc

***Single Responsibility Principle***

**REVISAR!**
Robert C. Martin afirma que "uma classe deve ter um, e apenas um, motivo para mudar". Ou seja, Uma classe ou módulo deve ter apenas uma responsabilidade sobre uma funcionalidade do sistema e essa responsabilidade deve estar encapsulada dentro da classe. E ainda é imporantante que todos os serviços providos por ela sejam coerentes com o contexto da classe.

***Open Closed Principle***
Esse principio afirma "classes devem ser abertas à extensão, mas fechadas a alteração". Isso está muito relacionado com encapsulamente, onde não devemos nos preocupar com tal funcionalidade está implementada, porém devemos ser capazes de mudar seu funcionamento para algo ainda coerente no contexto daquela entidade conforme as entradas usadas.

***Liskov Substituition Principle***
O principio de Substituição de Barbara Liskov está intimamente ligado com as heranças, afirmando que uma classe S que herda T em uma aplicação qualquer, S sempre pode substituir T sem nenhuma perda de corretude ou performace.

***Interface Segregation Principle***
O principio de segregação de interfaces afirma que um cliente não precisa utilizar nenhuma funcionalidade interna de um módulo para que ele faça bom uso daquelas funcionalidades disponíveis pela interface.

***Dependency Inversion Principle***
"Dependa de Abstrações. Do not depend upon concretions" é a frase que resumo esse principio, que podemos quebrar em duas expressões:

+ Módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações
+ Abstrações não devem depender de detalhes. Detalhes devem depender de abstrações.

Concluindo, nossas classes não podem quebrar caso desejemos mudar as classes de baixo nível que funcionam com elas.

Além disso, existem outros principios que devem ser seguidos pelo Scrum Master afim de manter a qualidade de software ótima e ser um exemplo para seus desenvolvedores.

***"Nada de janelas quabradas"***

Quando um desenvolvedor deixa um código sem cobertura testes, por exemplo, o próximo desenvolvedor tem essa sensação que não houve zelo por aquele código, e cria um novo método, deixando-o sem testar também. Com o tempo será possível notar uma grande queda na cobertura de testes, tanto que talvez se torne muito difícil para a equipe reverter o cenário. O mesmo poderia valer para código deixado sem refatorar, ou qualquer outra má prática de desenvolvimento.
Mas o contrário também pode acontecer. Se boas práticas são feitas dentro do ambiente, todos os desenvolvedores criam maior resistência a manter essa práticas e a não quebrá-las.

### XP - eXtremming Programming

***Propriedade Coletiva do Código***


***Programação em Par***

Um programador pode levar horas para encontrar um problema se estiver trabalhando a muito tempo, cansado ou até mesmo não conhecer algum detalhe do objeto de estudo. Portanto, como é apenas um computador, o novato é que fica à frente fazendo a codificação, e o instrutor acompanha ajudando a desenvolver suas habilidades. Desta forma o programa sempre é revisto por duas pessoas, evitando e diminuindo assim a possibilidade de defeitos. Com isto busca-se sempre a evolução da equipe, melhorando a qualidade do código fonte gerado.

***Small Realeases***

A liberação de pequenas versões funcionais do projeto auxilia muito no processo de aceitação por parte do cliente, que já pode testar uma parte do sistema que está comprando. As versões chegam a ser ainda menores que as produzidas por outras metodologias incrementais.

***TDD***

TDD, ou Test Driven Development, é uma prática de XP que faz com que os desenvolvedores tenham que escrever teste antes mesmo de fazer o próprio código. Essa pratica de programação funciona com o seguinte fluxo:

+ 1) Adicione um teste rapidamente
+ 2) Execute todos os testes e observe o novo teste falhar
+ 3) Faça uma pequena mudança para fazer o teste passar
+ 4) Execute todos os teste e observe que foram bem sucedidos
+ 5) Refatore

![fluxo_tdd](../images/chapter_2/tdd.png)

As gemas que facilitam o processo de TDD em rails são:

+ [Rspec-rails](https://rubygems.org/gems/rspec-rails) -> para testes de unidade
+ [Capybara](https://rubygems.org/gems/capybara) -> para teste de integração

**Exercícios:**

> 1) O que é um teste de unidade?

Resposta:

> 2) O que é um teste de integração?

Resposta:


Caso deseje praticar TDD com Rails e conhecer as gemas que facilitam esse processo, faça esse [tutorial](http://tutorials.jumpstartlab.com/projects/contact_manager.html).

***Refatoração***

É um processo que permite a melhoria continua da programação, com o mínimo de introdução de erros e mantendo a compatibilidade com o código já existente. Refabricar melhora a clareza (leitura) do código, divide-o em módulos mais coesos e de maior reaproveitamento, evitando a duplicação de código-fonte.

### SCRUM

