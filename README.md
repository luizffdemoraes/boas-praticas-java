

<br/>Java e refatoração: melhorando códigos com boas práticas<br/>
=================

A aplicação será integrada com uma API externa, que será a responsável por salvar pets e abrigos da aplicação console,
assim como retorná-los quando fizermos a requisição através da aplicação console. Essa API está incluída no formato 
.jar no nosso projeto que vamos utilizar para o curso. E para testar a aplicação console precisamos iniciar o arquivo .jar. 

Para isso, podemos usar o seguinte comando:

java -jar api.jar

## 01. Refatoração

### Nesta aula:
* Aprendemos a extrair código em métodos, com o intuito de melhorar a legibilidade do nosso código, facilitando assim sua manutenção;
* Entendemos o problema do código duplicado e como resolvê-lo para evitar inconsistências no código, caso haja alteração em um ponto do código duplicado e no outro não;
* Vimos que o ideal para resolver o código duplicado é aplicar a reutilização de código, em que o código fica presente em apenas um local e referenciá-lo ao utilizá-lo. Dessa forma, toda manutenção será feita em apenas um local.

## 02. SOLID

* Aprendemos que o S do acrônimo SOLID significa Single Responsability Principle, em português, princípio da responsabilidade única, ou seja, uma classe deve ter um, e somente um, motivo para mudar;
* Separamos nosso código em classes para que ficassem coesas e com apenas uma responsabilidade;
* Criamos classes de configurações para reaproveitá-las nas classes de serviço, evitando assim código duplicado.

## 03. Criando Dominios

* Aprendemos a criar classes de domínio, que são classes que representam "coisas" do mundo real;
* Conhecemos a biblioteca Jackson, que auxilia na serialização e deserialização de objetos fornecendo recursos para transformar um objeto Json em um objeto Java e vice-versa;
* Testamos nossa aplicação, após todas as refatorações, para garantir que a mesma continua funcional.


## 04. Testes Automatizados

* Aprendemos o que são testes automatizados e o quanto eles podem auxiliar no feedback da aplicação, bem como na validação dos cenários;
* Criamos um teste de unidade, que valida o retorno do método listarAbrigo;
* Conhecemos a biblioteca junit, que fornece recursos para criarmos testes de unidade e a biblioteca mockito, que fornece recursos para simulação de objetos.

## 05. Padrões de Projetos

* Aprendemos o padrão Command, que visa encapsular uma solicitação como um objeto, o que lhe permite parametrizar outros objetos com diferentes solicitações.
* Melhoramos nosso código usando o switch expressions, permitindo trocar os if’s e else’s que tornavam a classe AdopetConsoleApplication difícil de ler.