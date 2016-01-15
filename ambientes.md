Ambientes
=========
 
Siga esse estudo dirigido para aprender mais sobre os ambientes que a CJR para desenvolver e manter sua aplicação, e como esses são versioandos no GitHub e no Heroku.

Antes de tudo, vamos verificar seus conhecimentos em Git.

Caso tenha alguma dúvida ou não tenha experiência nisso, os links abaixam podem ajudá-lo.

+ [http://rogerdudler.github.io/git-guide/](http://rogerdudler.github.io/git-guide/)
+ [http://git-scm.com/book/en/v2](http://git-scm.com/book/en/v2)

> 1) Em Git, como eu adiciono ao commit um arquivo "person_model.rb"?

Resposta: 

> 2) Em Git, como eu faço um commit com a seguinte mensagem: "Views transformadas para Slim"?

Resposta: 

> 3) Em Git, como eu crio um branch com o nome "feature-authentication"?

Resposta: 

> 4) Em Git, como eu faço um pull com o branch da questão anterior?

Resposta:

... (add mais perguntas)

Agora é importante que você entenda como colocar uma aplicação rails no Heroku. Siga esse [tutorial](https://devcenter.heroku.com/articles/getting-started-with-ruby#introduction) e coloque a aplicação `apps/blog/.` no ar.

Sabendo colocar uma aplicação rails no heroku, temos que nos preocupar como nossa aplicação será versionada. Para isso vamos supor que você está gerenciando um projeto que tem as seguintes histórias de usuários no backlog.

+ Usuário cadastra um produto
+ Admin bloquei um usuário
+ Usuário cadastra uma categoria
+ Usuário compra um produto
+ Usuário vende um produto

Para desenvolvermos essas histórias, no GitHub, criaremos um branch para cada uma das histórias, seguindo a tabela a baixo:

| 						       Branch | 		História de Usuário   |
|-------------------------------------|-------------------------------| 
| feature_usuario_cadastra_produto    | Usuário cadastra um produto   |
| feature_admin_bloquei_usuario       | Admin bloquei um usuário      |
| feature_usuario_cadastra_catergoria | Usuário cadastra um categoria |
| feature_usuario_compra_produto	  | Usuário compra um produto     |
| feature_usuario_vende_produto		  | Usuário vende um produto	  |

Assim, esses branch terão apenas um desenvolvedor responsável. Além disso, pode-se criar um branch para funcionalidades gerais como implementar o devise ou mudar de bootstrap para materialize.
Esses branchs tem como objetivo evoluir o projeto e portanto são muito instáveis já que os desenvolvedores estão desenvolvendo nesses branchs.
Porém, o branch master deve estar estável com o que ele possui. Todos os branchs de feature são unidos no master e o objetivo é manter a master estável depois de todos os merges.
Todos os branchs definem o ambiente de desenvolvimento e teste.
Mas antes:

**Ambiente de desenvolvimente**: onde o projeto é desenvolvido e são realizados os testes não automatizados. O banco de dados é mantido pelo desenvolvedor.

**Ambiente de testes**: onde o projeto tem seus testes automatizados executados. A cada ciclo de execução dos testes, o banco é inilizado, os testes são executados e depois o banco é apagado.

**Ambiente de produção**: é onde os clientes acessam o sistema e não deve conter erros. Caso um erro aconteça, ele mostrado para cliente como um erro 400, 404, 405 entre outros, dependendo do erro do rails. Seguem alguns exemplos de erros que são mostrados em uma aplicação rails.

• ActionController::RoutingError-“hdhNotFound”
• AbstractController::ActionNotFound-“hdhNotFound”
• ActionController::MethodNotAllowed - “hdi Method Not Al- lowed”
• ActionController::NotImplemented-“ideNotImplemented”
• ActionController::UnknownFormat-“hdjNotAcceptable”
• ActionController::InvalidAuthenticityToken - “hff Unproces- sable Entity”
• ActionController::BadRequest-“hddBadRequest”
• ActiveRecord::RecordNotFound-“hdhNotFound”
• ActiveRecord::RecordInvalid-“hffUnprocessableEntity”

Caso o cliente queria manter o que foi desenvolvido em produção, o branch master do heroku deve ser a forma mais estável do projeto e preparada para receber clientes. Além disso, o remote do Heroku deve ter outro branch de homologação. Isso é o local onde o cliente vê a aplicação e passa os feedbacks.

Caso o cliente não queria, o próprio branch master pode ser usado para homologação enquanto o projeto está sendo desenvolvido e depois é colocado para a produção.