### Biblioteca


A biblioteca normalmente é uma implementação real das regras de uma API. Portanto ela é mais concreta. Assim como a API, você não precisa saber os detalhes da implementação para usá-la. A biblioteca precisa respeitar as regras da API sempre, mas não precisa ter sua implementação estável. A biblioteca costuma ser autossuficiente.

Uma biblioteca pode conter implementações públicas que não fazem parte da API. Usá-las pode trazer risco.

Você chama uma biblioteca. É uma ferramenta. Você usa o que precisa.

Até o momento nenhuma resposta tratou do termo biblioteca como forma de organização de códigos binários para o uso com aplicações. Uma biblioteca também é um arquivo executável contendo um conjunto de funções para executar diversas tarefas. .dll ou .so são arquivos de biblioteca para ligação dinâmica na aplicação. .lib ou .a são arquivos de biblioteca para ligação estática na aplicação.

Você pode ter uma biblioteca de manipulação strings, de expressões regulares, de coleções de dados, de manipulação de arquivos, acesso a um banco de dados, manipulação de imagens, etc.

As bibliotecas podem ser externas, que é o caso de serviços web. Esta é uma forma comum hoje em dia para evitar pirataria, já que muitas aplicações são web. Pode ter algumas vantagens, mas também possui muitas desvantagens.

### Framework


Um framework normalmente é um conjunto de bibliotecas para conseguir executar uma operação maior. É comum um framework encapsular os comportamentos da API em implementações mais complexas, permitindo o seu uso de forma mais flexível, frequentemente através de extensões, configurações e inversões de controle. Como pode ser considerada uma camada em cima da API eventualmente pode simplificá-la em certo sentido. Ele costuma dar consistência a um conjunto de bibliotecas (pena que acontece o oposto em alguns casos).

O framework costuma "tomar conta" da sua aplicação deixando "portas" para você acessar, o que é importante para o seu objetivo. É comum ter uma grande interdependência entre seus componentes. Por estas duas razões, o framework pode se tornar um fardo quando ele não é bem feito, ou não é adequado ao que o programador precisa, ou quando o programador não sabe bem como usá-lo. O que é muito comum acontecer uma ou mais dessas situações.

Um framework chama você. É um estilo de vida. Seu projeto se compromete com ele.

Frameworks podem ser entendidos como plataformas de desenvolvimento. Eles possuem lacunas que devem ser preenchidas pelo programador para funcionar conforme sua necessidade. Pode ser visto como um esqueleto de uma aplicação. Frequentemente são confundidos, de forma certa ou errada, como um conjunto de classes.

Algumas vezes o termo é usado para determinar um conjunto de arquivos de bibliotecas de códigos binários, ou fontes, ou até outros recursos para a aplicação que são relacionados.

Exemplos são os sistemas de GUI, de operações web, alguns ORMs, um conjunto de bibliotecas padrão de uma linguagem de programação, implementação de um padrão MVC, etc.

Algumas vezes uma biblioteca é ou se torna tão complexa que acaba virando um framework. Se isto é bom ou ruim deixo para você decidir.