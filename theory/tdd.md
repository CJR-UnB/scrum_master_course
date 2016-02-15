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

Caso deseje praticar TDD com Rails e conhecer as gemas que facilitam esse processo, faça esse [tutorial](http://tutorials.jumpstartlab.com/projects/contact_manager.html).

***Refatoração***

É um processo que permite a melhoria continua da programação, com o mínimo de introdução de erros e mantendo a compatibilidade com o código já existente. Refabricar melhora a clareza (leitura) do código, divide-o em módulos mais coesos e de maior reaproveitamento, evitando a duplicação de código-fonte.