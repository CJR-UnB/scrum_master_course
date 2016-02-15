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